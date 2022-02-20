<template>
    <div id="t-base-upsell">
        <div id="t-upsell-container">
            <!-- intro -->
            <base-intro/>

            <!-- graphic -->
            <div id="t-upsell-graphic">

            </div>
        </div>
    </div>
</template>

<script>
import BaseIntro from '../../components/base/BaseIntro.vue';

export default {
    components: {
        BaseIntro,

    }
}
</script>

<style scoped>
@import url('../../style/base/upsell.css');
</style>