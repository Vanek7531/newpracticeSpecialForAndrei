<script setup>
const someFunction = () => {
    console.log('123',);
}
</script>
<template>
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
