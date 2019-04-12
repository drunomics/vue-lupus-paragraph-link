<template>
  <div class="paragraph paragraph--link">
    <slot name="title" />
    <slot :name="$slots.link ? 'link': 'default'" />
  </div>
</template>
<script>
  export default {
    name: 'PgLink'
  };
</script>
