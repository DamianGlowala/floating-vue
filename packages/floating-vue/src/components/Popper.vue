<script lang="ts">
import Popper from './Popper'

export default {
  extends: Popper(),
}
</script>

<template>
  <div
    ref="reference"
    class="v-popper"
    v-bind="$attrs"
    :class="{
      'v-popper--shown': slotData.isShown,
    }"
  >
    <slot
      v-bind="slotData"
    />
  </div>
</template>
