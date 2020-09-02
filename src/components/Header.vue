<template>
  <div class>
    <HeaderTop />
    <HeaderProfile />
  </div>
</template>

<script>
import HeaderTop from "@/components/HeaderTop";
import HeaderProfile from "@/components/HeaderProfile";
export default {
  name: "Header",
  components: {
    HeaderTop,
    HeaderProfile,
  },
};
</script>

<style lang="scss" scoped>
</style>
