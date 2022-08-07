<template>
  <q-page class="flex flex-center">
   <div @click="goto">tes</div>
  </q-page>
</template>

<script>
import { defineComponent } from 'vue';
import  { useRouter } from 'vue-router'
export default defineComponent({
  name: 'PageIndex',
  setup(){
    const router = useRouter()
    const goto = () => {
      router.push({
        name: 'tes'
      })
    }
    return {
      goto
    }
  }
})
</script>
