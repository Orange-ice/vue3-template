<script lang="tsx">
import { defineComponent } from 'vue';

export default defineComponent({
  setup: (props, context) => {
    return () => (
      <div class="title">Hello, This is Vue3 Template!</div>
  )
 }
})

</script>

<style scoped lang="scss">
.title {
  height: 6em;
  padding: 1.5em;
  will-change: filter;
  color: #007acc;
}
</style>
