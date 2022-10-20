<script lang="tsx">
import { defineComponent, PropType } from 'vue';

const Icon = defineComponent({
  name: 'Icon',
  props: {
    name: {
      type: String as PropType<string>,
      required: true
    },
    onClick: {
      type: Function as PropType<() => void>,
    }
  },
  setup(props) {
    return () => (
      <svg class="icon" onClick={props.onClick}>
        <use xlinkHref={`#${props.name}`} />
      </svg>
    );
  }
});

export default Icon;
</script>

<style lang="scss" scoped>
.icon {
  width: 1.2em;
  height: 1.2em;
}
</style>