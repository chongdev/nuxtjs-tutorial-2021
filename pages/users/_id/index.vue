<template>
  <div>
      This user id:{{$route.params.id}}
  </div>
</template>

<script>
export default {
    validate(data){
        return /^\d+$/.test(data.params.id)
    }
}
</script>