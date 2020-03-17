<template>
    <div id="app">
        <Header v-if="showAll === true"/>
        <Table v-if="showAll === true"/>
        <Button v-if="showAll === true" v-on:deleteAll="removeAllComponents()"/>
    </div>
</template>

<script>
    import Header from './components/Header.vue';
    import Table from './components/Table';
    import Button from './components/Button';

    export default {
        name: 'App',
        data: () => ({
            showAll: true
        }),
        components: {
            Header,
            Table,
            Button
        },
        methods: {
            removeAllComponents: function () {
                this.showAll = false
            }
        }
    }
</script>

<style>
    #app {
        max-width: 800px;
        margin: 0 auto;
        padding: 20px;
        min-width: 320px;
    }
</style>
