<template>
    <button @click="onClick()" :style="{ background: 'green'}" class='btn'> QUOTE! </button>
</template>

<script>

export default {
    name: 'Button',
    methods: {
        OnClick(){
            this.$emit('btn-click')
        }
    }

}
</script>
