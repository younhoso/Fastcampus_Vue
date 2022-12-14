<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
    components: {},
    data() {
        return{
            message: 'hello',
            active: false
        };
    },
    setup() {},
    created() {},
    mounted() {},
    unmounted() {},
    methods: {
    }
}
</script>

<template>
  <div class="msg" v-bind:class="{'active': active}">
    {{message}}
  </div>
  <div>
    <a href="https://vitejs.dev" target="_blank">
      <img src="/vite.svg" class="logo" alt="Vite logo" />
    </a>
    <a href="https://vuejs.org/" target="_blank">
      <img src="./assets/vue.svg" class="logo vue" alt="Vue logo" />
    </a>
  </div>
  <HelloWorld msg="Vite + Vue" />
</template>

<style scoped>
.msg.active { color: red;}
</style>
