<script>
import { GSCarousel, GSLayoutDefault } from "gitart-scroll-carousel/bundled";
import "gitart-scroll-carousel/dist/index.css";
import "gitart-scroll-carousel/dist/GSArrow.css";
import "gitart-scroll-carousel/dist/ExampleLayoutDefault.css";
export default defineComponent({
  components: {
    GSCarousel,
  },
  setup() {
    return {
      items: [0, 1, 2, 3, 4],
      GSLayoutDefault,
    };
  },
});
</script>
<template>
  <GSCarousel
    :items="items"
    item-gap="16"
    :items-to-show="2"
    :layout="GSLayoutDefault"
    :layout-props="{
      disableArrows: true,
    }"
  >
    <template #item="{ data }">
      <div class="slide">
        {{ data }}
      </div>
    </template>
  </GSCarousel>
</template>
<style scoped>
.slide {
  box-shadow: 0 6px 15px -3px rgb(0 0 0/0.3);
  padding: 25px;
  border-radius: 5px;
  background: rgb(202, 202, 202);
  color: #000;
}
</style>
