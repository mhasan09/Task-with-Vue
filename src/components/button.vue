<template>
    <button @click="onClick()" :style="{background: color}" class="btn" id="add_task_button" >{{text}}</button>
</template>

<script>
export default {
    name: "Button",
    props: {
        text: String,
        color: String
    },
    methods: {
        onClick(){
            this.$emit('btn-click')
        }
    }
}
</script>
