<template>
  <div class="container pt-24">
    <hr class="my-4" />
    <div class="mt-8 mb-4 space-y-2">
      <MH1 text="Mihailo Pantović" />
      <h2 class="text-xl">Front-End Developer</h2>
      <address class="not-italic">
        <p class="text-brand font-bold underline">
          <a href="mailto:pantovic.mihailo@gmail.com">
            pantovic.mihailo@gmail.com
          </a>
        </p>
      </address>
    </div>
    <div class="flex flex-wrap -mx-2">
      <div class="w-full sm:w-2/3 px-2">
        <main>
          <hr class="my-4" />
          <MH3 :text="$t('experience.title')" />
          <m-card
            :title="$t('experience.helbiz.title')"
            link="https://helbiz.com"
            :date="$t('experience.helbiz.duration')"
          >
            <p
              class="text-sm"
              v-text="$t('experience.helbiz.desc')"
            />
          </m-card>

          <m-card
            :title="$t('experience.yamba.title')"
            link="https://yamba.com"
            :date="$t('experience.yamba.duration')"
          >
            <p
              class="text-sm"
              v-text="$t('experience.yamba.desc')"
            />
          </m-card>
          <m-card
            :title="$t('experience.presta.title')"
            link="https://wearepresta.com"
            :date="$t('experience.presta.duration')"
          >
            <p
              class="text-sm"
              v-text="$t('experience.presta.desc')"
            />
          </m-card>
          <hr class="my-4" />
          <MH3 :text="$t('education.title')" />
          <div class="card my-8">
            <m-card
              :title="$t('education.fon.title')"
              :date="$t('education.fon.duration')"
            />
          </div>
        </main>
      </div>
      <div class="w-full sm:w-1/3 px-2">
        <m-sidebar />
      </div>
    </div>
  </div>
</template>

<script>
import MSidebar from "~/components/MSidebar.vue";
import MCard from "~/components/UI/MCard.vue";
import MH1 from "~/components/UI/MH1.vue";
import MH3 from "~/components/UI/MH3.vue";
export default {
  components: {
    MSidebar,
    MCard,
    MH1,
    MH3
  }
};
</script>

<style></style>
