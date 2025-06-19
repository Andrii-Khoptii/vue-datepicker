<template>
    <div class="wrapper">
        <Datepicker v-model="selectedDate" range :multi-calendars="{ solo: true, orderCalendars: true, autoReselect: true }" auto-apply placeholder="Select Date" />
    </div>
</template>

<script lang="ts" setup>
    import { ref } from 'vue';
    import Datepicker from '../src/VueDatePicker/VueDatePicker.vue';

    const selectedDate = ref();
</script>

<style lang="scss">
    .wrapper {
        padding: 200px;
    }
</style>
