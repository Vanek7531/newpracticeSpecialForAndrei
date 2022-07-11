<script setup>
import { defineProps } from 'vue'




const props = defineProps({
    itemValue: {
        type: Number, default: null
    },

})

const someFunction = () => {
    console.log('123', props.itemValue);
}

</script>

<template>
    {{ itemValue }} 1231
    <div class="slot" @contextmenu.prevent="someFunction">
        <slot> </slot>
    </div>
</template>

<style lang="css">
.slot {
    color: red;
    cursor: pointer;
}
</style>
