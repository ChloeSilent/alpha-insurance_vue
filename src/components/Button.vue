<template>
    <div class="button-container">
        <button type="button" @click="deleteAll">Стереть</button>
    </div>
</template>

<script>
    export default {
        name: 'Button',
        methods: {
            deleteAll: function () {
                this.$emit('deleteAll');
            }
        }
    }
</script>

<style>
    .button-container {
        padding-top: 10px;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    button {
        background-color: #008CBA;
        border: none;
        padding: 5px 7px;
        transition: background-color 1s ease-in;
    }

    button:hover {
        background-color: #f44336;
    }
</style>
