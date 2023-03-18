<template>
  <button class="l-button"
    :class="{[`theme-${theme}`]: theme}"
  >
    <slot />
  </button>
</template>

<script lang="ts">
export default{
  inheritAttrs: false,
  props: {
    theme:{
      type:String,
      default:'button'
    }
  },
  setup(props, context) {
    const { size, ...rest } = context.attrs;
    return { size, rest };
  },
}
</script>
