<template>
  <div>
    <h1>{{title}}</h1>
    <button @click="openModal(true)"></button>
    <edit-modal isVisible="isVisible"/>
  </div>
</template>

<script>
import EditModal from './components/EditModal.vue'
export default {
components: {
  EditModal
},
  data () {
    return {
      title: 'OpenVPN',
      isVisible: false
    }
  },
  methods: {
    openModal (boolean) {
      this.isVisible = boolean
    }
  }
}
</script>

<style scoped>

</style>
