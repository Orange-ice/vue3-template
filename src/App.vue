<script lang="tsx">
import { defineComponent } from 'vue';
import Icon from './components/icon.vue';

export default defineComponent({
  setup: (props, context) => {
    return () => (
      <div class="title">
        Hello, This is Vue3 Template!
        <Icon name="vue" />
      </div>
  )
 }
})

</script>

<style scoped lang="scss">
.title {
  height: 6em;
  padding: 1.5em;
  color: #007acc;
}
</style>
