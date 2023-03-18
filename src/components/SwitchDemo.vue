<template>
  <div>
    <Switch v-mode:value="y" />
  </div>
</template>


<script lang="ts">
import { ref } from 'vue'
import Switch from '../lib/Switch.vue'
export default{
  components:{Switch},
  setup(){
    const y = ref(false)
    return {y}
  }
}
</script>
