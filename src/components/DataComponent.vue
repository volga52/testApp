<template>
    <div>
        content
        <input v-model="inputValue">
        {{ inputValue.toUpperCase() }}
        <hr>
    </div>
</template>

<script>
export default{
  data: () => ({
      inputValue: ''
  }),
  watch: {
      inputValue() {
          if (this.inputValue.length > 9) {
              console.log('Слишком длинное слово');
          }
      }
  }
}
</script>