<template>
  <div class="balabala" ref="balabala">
    <a-image
            :width="200"
            :preview="previewType"
            src="https://zos.alipayobjects.com/rmsportal/jkjgkEfvpUPVyRjUImniVslZfWPnJuuZ.png"
    />
  </div>
</template>
<script lang="ts">
    import { defineComponent,h ,computed,ref} from "vue";

    export default defineComponent({
        name: "AppAvailable",
        setup(props, context) {
            const balabala = ref(null)

            const previewType = {
                getContainer:balabala.value
            }

            return {
                balabala,previewType
            }
        }
    });

</script>

<style lang="less">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
