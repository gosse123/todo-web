<template>
    <input type="checkbox" @change="onChange">
    {{ label }}
</template>

<script setup>
defineProps({
    label:String
})
const emits = defineEmits(["check","uncheck"])
const onChange = (event)=>{
    if(event.currentTarget.checked){
        emits('check',currentTarget)
    }else{
        emits('uncheck',currentTarget)
    }
}
</script>