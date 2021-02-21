<template>
  <div>
    <div class="text-xl bg-blue-500">hello</div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  mounted() {
    browser.runtime.sendMessage({})
  },
  computed: {
    defaultText() {
      return browser.i18n.getMessage('extName')
    },
  },
}
</script>

<style scoped>
p {
  font-size: 20px;
}
</style>
