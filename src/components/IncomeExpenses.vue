<template>
    <div class="inc-exp-container">
        <div>
            <h4>Income</h4>
            <p id="money-plus" class="money plus">+${{ incomeBal }}</p>
        </div>
        <div>
            <h4>Expense</h4>
            <p id="money-minus" class="money minus">${{ expensesBal }}</p>
        </div>
    </div>
</template>

<script setup>
import { defineProps } from 'vue';

const props = defineProps({
    expensesBal: {
        type: Number,
        required:true
    },
    incomeBal: {
        type: Number,
        required:true
    },
})
</script>