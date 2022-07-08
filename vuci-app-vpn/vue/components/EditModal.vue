<template>
  <div>
    <a-modal :visible="isVisible">
    <h1>{{title}}</h1>
    </a-modal>
  </div>
</template>

<script>
export default {
  name: 'EditModal',
  props: ['isVisible'],
  data () {
    return {
      title: 'modal from component'
    }
  }
}
</script>

<style scoped>

</style>
