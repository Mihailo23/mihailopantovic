<template>
  <ul class="flex text-gray-800 items-center h-10 py-1">
    <li>
      <NavigationItem
        to="/"
        exact
        class="mr-2"
        :text="$t('links.home')"
      />
    </li>
    <li>
      <NavigationItem
        to="/projects"
        :text="$t('links.projects')"
      />
    </li>
    <li class="ml-auto">
      <client-only>
        <LanguageChanger />
      </client-only>
    </li>
  </ul>
</template>

<script>
import NavigationItem from "./NavigationItem.vue";
import LanguageChanger from "~/components/UI/LanguageChanger.vue";
export default {
  components: {
    NavigationItem,
    LanguageChanger
  }
};
</script>

<style lang="scss" scoped></style>
