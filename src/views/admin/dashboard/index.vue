<template>
  <page-container>
    <template #header>
      <h1>{{ $t('hello') }}</h1>
    </template>
    <el-calendar v-model="date" />
  </page-container>
</template>

<script>
export default {
  inject: ['@adminContainer'],
  data() {
    return {
      date: new Date()
    }
  }
}
</script>
