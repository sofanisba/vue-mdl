<template>
  <a class="mdl-button mdl-js-button"
     :class="cssClasses"
     :disabled="disabled"
    >
    <slot>
      <i class="material-icons" v-if="isIconSpecified" >{{ icon }}</i>
    </slot>
  </a>
</template>

<script>
import button from './mixins/button'

export default {
  mixins: [button]
}
</script>
