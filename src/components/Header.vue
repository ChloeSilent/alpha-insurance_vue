<template>
    <div class="header">
        <div>Menu</div>
        <ul class="items-container">
            <li class="item">Item</li>
            <li class="item">Item</li>
            <li class="item">Item</li>
            <li class="item">Item</li>
            <li class="item">Item</li>
        </ul>
    </div>
</template>

<script>

    export default {
        name: 'Header',
    }
</script>

<style>
    .items-container {
        list-style: none;
        display: flex;
        justify-content: space-between;
        border-style: solid;
        border-color: black;
        border-width: 1px 0 0 1px;
        margin: 0 0 10px 0;
        padding: 0;
    }

    .item{
        text-align: left;
        border: 1px solid black;
        width: 100%;
        margin:-1px 0 0 -1px;
        width: 100%;
    }

</style>
