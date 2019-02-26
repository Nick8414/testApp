<template>

    <td>
            {{ value }}
            <slot></slot>
        </td>

        
</template>

<script>
export default {
    props: {
        value: String
    }
    
}
</script>

<style>

</style>

