<template>
    <div id="t-base-card">
        <div id="t-card-container">
            <!-- content -->
            <div id="t-card-content">
                <div class="t-card-icon" v-if="showIcon"></div>
                <h2 class="t-card-title">{{title}}</h2>
                <div class="t-card-text">{{text}}</div>
                <div 
                    class="t-card-button t-button"
                    :class="{'t-border-btn' : btnStyle}"
                >{{buttonName}}</div>
            </div>

            <!-- image -->
            <div id="t-card-image">
                <img :src="require(`@/assets/imgs/${imgName}`)"/>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        showIcon: {
            type: Boolean,
            default: false
        },
        imgName: {
            type: String,
            default: 'Rectangle9.png'
        },
        title: {
            type: String,
            default: 'Claim a Free Limited NFT'
        },
        text: {
            type: String,
            default: 'New members who sign up between 3/5 and 3/11 can claim a free NFT by creator Cyle Sim.'
        },
        buttonName: {
            type: String,
            default: 'Claim Now'
        },
        btnStyle: {
            type: Boolean,
            default: true
        },

    }
}
</script>

<style scoped>
@import url('../../style/base/card.css');
</style>