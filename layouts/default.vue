<template>
  <div class="layout">
    <Nav></Nav>
    <div class="content">
      <Nuxt />
    </div>
  </div>
</template>

<script>
import Nav from '@/components/nav.vue'

export default {

}
</script>

<style lang="scss" scoped>
.content{
  padding-top:50px;
  overflow: auto;
}
</style>
