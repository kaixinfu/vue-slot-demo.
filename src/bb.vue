<template>
    <div class="bb">
        <!-- <div>b1:<slot>c1</slot></div>
        <div>b2:<slot>c2</slot></div> -->
        
        <div>b1:<slot name="c1">c1</slot></div>
        <div>b2:<slot name="c2">c2</slot></div>
    </div>
</template>

<script>
export default {
    name: "bb"
}
</script>

<style scoped>

</style>
