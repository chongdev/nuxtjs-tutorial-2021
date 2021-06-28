<template>
    <div>
        <nav-bar></nav-bar>
        <h1> This User </h1>

        <nuxt-child />
    </div>
</template>

<script>
import NavBar from '~/components/NavBar.vue'
export default {
    components: [NavBar],
}
</script>