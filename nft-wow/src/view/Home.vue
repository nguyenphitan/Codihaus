<template>
    <div id="t-home">
        <div id="t-home-container">

            <!-- The header -->
            <the-header/>
            <!-- End header -->

            <!-- The content -->
            <the-content/>
            <!-- End content -->

            
        </div>
    </div>
</template>

<script>
import TheHeader from '../components/layout/TheHeader.vue';
import TheContent from '../components/layout/TheContent.vue';

export default {
    name: 'home-page',
    components: {
        TheHeader,
        TheContent,

    }
}
</script>

<style scoped>
#t-home {
    position: relative;
    padding-top: 56px;
}

#t-home-container {
    margin: 0 64px;
}
</style>