<template>
  <div class="paragraph paragraph--link">
    <div class="paragraph__field-link">
      <slot name="field_link">
        <a
          class="paragraph__link"
          v-for="link in linksComputed"
          :href="link.uri"
        >
          {{ link.title }}
        </a>
      </slot>
      <slot/>
    </div>
  </div>
</template>
<script>
  export default {
    name: 'PgLink',
    props: {
      dataLinks: { type: String, default: () => '[]' },
    },
    computed: {
      linksComputed() {
        return JSON.parse(this.dataLinks);
      },
    }
  };
</script>
