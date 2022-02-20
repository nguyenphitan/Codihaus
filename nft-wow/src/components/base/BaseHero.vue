<template>
    <div id="t-base-hero">
        <div id="t-hero-container">
            <!-- intro -->
            <base-intro/>

            <!-- testimonial -->
            <div id="t-hero-testimonial">
                <!-- Left -->
                <div class="t-testimonial-left"></div>
                <!-- Right -->
                <div class="t-testimonial-right">
                    <div class="t-testimonial-user">Jess Young</div>
                    <p class="t-testimonial-text">“NFTwow helped me to turn my art from earning the odd $20, to earning over seven figures a year.”</p>
                </div>
            </div>

            <!-- image -->
            <div id="t-hero-image"></div>
            <!-- <div id="t-hero-cre">OctopusGame by NFTGame</div> -->
            <div id="t-hero-background"></div>
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
@import url('../../style/base/hero.css');
</style>