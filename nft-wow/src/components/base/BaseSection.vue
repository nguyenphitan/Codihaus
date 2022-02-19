<template>
    <div id="t-base-section">
        <div id="t-section-container">
            <!-- Left -->
            <div id="t-section-left">
                <div class="t-section-title">{{title}}</div>
                <div class="t-section-paragraph">{{paragraph}}</div>
            </div>

            <!-- Right -->
            <div id="t-section-right">
                <div class="t-section-button t-button">{{buttonName}}</div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'base-section',
    props: {
        title: {
            type: String,
            default: "Upcoming Drops"
        },
        paragraph: {
            type: String,
            default: "Be the first to get your hands on limited NFT drops, exclusive to NFTwow."
        },
        buttonName: {
            type: String,
            default: "Explore"
        },

    },
    data() {
        return {
            
        }
    },
}
</script>

<style scoped>
@import url('../../style/base/section.css');
</style>