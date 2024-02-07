<template>
    <fwb-tabs v-model="activeTab" variant="pills" class="">
      <fwb-tab name="first" title="First">
        Lorem ipsum dolor...1
      </fwb-tab>
      <fwb-tab name="second" title="Second">
        Lorem ipsum dolor...2
      </fwb-tab>
      <fwb-tab name="third" title="Third">
        Lorem ipsum dolor...3
      </fwb-tab>
      <fwb-tab name="fourth" title="Fourth" disabled>
        Lorem ipsum dolor...4
      </fwb-tab>
    </fwb-tabs>
  </template>
  
  <script setup>
  import { ref } from 'vue'
  import { FwbTab, FwbTabs } from 'flowbite-vue'
  
  const activeTab = ref('first')
  </script>
