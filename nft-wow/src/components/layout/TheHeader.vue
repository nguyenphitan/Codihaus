<template>
    <div id="t-the-header">
        <div id="t-header-container">
            <!-- Control -->
            <div id="t-header-control"></div>
            
            <!-- Header -->
            <base-header/>

        </div>
    </div>
</template>

<script>
import BaseHeader from '../base/BaseHeader.vue';

export default {
    name: 'the-header',
    components: {
        BaseHeader,
    }

}
</script>

<style scoped>
@import url('../../style/layout/header.css');
</style>