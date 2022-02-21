<template>
    <div id="t-base-trend">
        <div id="t-trend-container">
            <!-- Section header -->
            <base-section
                :title="title"
                :paragraph="paragraph"
                :buttonName="buttonName"
            />

            <!-- List -->
            <div id="t-trend-list">
                <div v-for="(item,index) in arrInfo" :key="index">
                    <base-item 
                        :imgName="item.imgName"
                        :name="item.name"
                        :lowestPrice="item.lowestPrice"
                        :mobilize="item.mobilize"
                        :price="item.price"
                    />
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import BaseSection from './BaseSection.vue';
import BaseItem from './BaseItem.vue';

export default {
    name: 'base-trend',
    components: {
        BaseSection,
        BaseItem,
    },
    props: {
        title: {
            type: String,
            default: "Top & Trending"
        },
        paragraph: {
            type: String,
            default: "See what’s hot in the world of non-fungibles."
        },
        buttonName: {
            type: String,
            default: "Explore"
        },
        arrInfo: {
            type: Array,
            default: new Array
        }
    },
}
</script>

<style scoped>
@import url('../../style/base/trend.css');
</style>