<template>
  <div>
      <nav-bar></nav-bar>
      <div>This user id:{{$route.params.id}}</div>
  </div>
</template>

<script>
import NavBar from '~/components/NavBar.vue'
export default {
     components: [NavBar],
    validate(data){
        return /^\d+$/.test(data.params.id)
    }
}
</script>