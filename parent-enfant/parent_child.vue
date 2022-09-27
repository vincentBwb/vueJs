
<template>
    <div class="parent-component">
        <!-- c est le v-bind qui fait que le parent et l enfant est lié :message -> v-bin:message.  -->
        <ChildComponent :message="truc"></ChildComponent>
    </div>
</template>

<script>
    import ChildComponent from "@/parent-enfant/ChildComponent.vue";

    export default {
        name: "parentComponent",
        data() {
            return {
                truc: "message du parent",
            };
        },
        components: {
            ChildComponent
        },
    };
</script>