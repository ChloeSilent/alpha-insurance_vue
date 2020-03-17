<template>
    <div class="table">
        <div class="row head-row">
            <div>1h</div>
            <div>2h</div>
            <div>3h</div>
            <div>4h</div>
        </div>
        <div class="row">
            <div>1</div>
            <div>2</div>
            <div>3</div>
            <div>4</div>
        </div>
        <div class="row">
            <div>1</div>
            <div>2</div>
            <div>3</div>
            <div>4</div>
        </div>
        <div class="row">
            <div>1</div>
            <div>2</div>
            <div>3</div>
            <div>4</div>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Table',
    }
</script>

<style>
    .table {
        border-style: solid;
        border-color: red;
        border-width: 1px 0 0 1px;
    }

    .row {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
    }

    .row div {
        text-align: left;
        border: 1px solid red;
        width: 100%;
        margin:-1px 0 0 -1px;
    }

    .head-row {
        background-color: gray;
    }

    @media (max-width: 480px) {
        .table {
            display: flex;
            flex-direction: row;
        }

        .row {
            flex-direction: column;
            width: 100%;
        }

        .head-row {
            background-color: unset;
        }

    }

</style>
