<template>
    <div id="t-base-intro">
        <div id="t-hero-intro">
            <div id="t-intro-container">
                <div id="t-intro-welcome">{{welcome}}</div>
                <h1 id="t-intro-title">{{title}}</h1>
                <h2 id="t-intro-description">{{description}}</h2>
                <div id="t-intro-button">
                    <div class="t-intro-explore t-button">{{button1}}</div>
                    <div class="t-intro-create t-button">{{button2}}</div>
                </div>
            </div>
        </div>
        <div id="t-intro-rectangle"></div>
        <div id="t-intro-rectangle"></div>
    </div>
</template>

<script>
export default {
    props: {
        welcome: {
            type: String,
            default: 'welcome'
        },
        title: {
            type: String,
            default: 'Trade NFTs with zero fees'
        },
        description: {
            type: String,
            default: 'We are the world’s highest-rated online marketplace'
        },
        button1: {
            type: String,
            default: 'Explore NFTs'
        },
        button2: {
            type: String,
            default: 'Create Your Own'
        }
    }
}
</script>

<style scoped>
@import url('../../style/base/intro.css');
</style>