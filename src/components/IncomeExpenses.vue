<template>
        <div class="inc-exp-container">
            <div>
                <h4>INCOME</h4>
                <P id="money-plus" class="money plus">+${{ income }}</P>
            </div>
            <div>
                <h4>EXPENSE</h4>
                <P id="money-minus" class="money minus">+${{expenses}}</P>
            </div>
        </div>
</template>

<script setup>
    import {defineProps} from 'vue';

    const props = defineProps({
        income: {
            type: Number,
            required:true
        },
        expenses: {
            type: Number,
            required:true
        },
    })
</script>