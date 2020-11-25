<template v-slot:[tree.key]>
    <component :is="tree.name" :slot="tree.key">
        <Demo v-for="item in tree.children" :key="item.key" :tree="item"></Demo>
    </component>
</template>
<script>

import AA from './aa'
import BB from './bb'
import CC from './cc'

export default {
    name: 'Demo',
    props: {tree: Object},
    components: {AA, BB, CC},
    data() {
        return {

        }
    },
    mounted() {
        console.log("tree:::", this.tree)
    },
    computed: {
    },
    methods: {
    }
}
</script>

<style lang="less" scoped>
</style>
