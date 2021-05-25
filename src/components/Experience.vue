<template>
  <v-card flat color="transparent" class="has-anchor">
    <v-subheader class="text-h4">
      <v-text class="text-none teal--text text--accent-1 text-h5 pr-3">
        02.
      </v-text>
      Experience
      <div class="horizontal-bar ml-5" />
    </v-subheader>

    <!-- <div class="experience-content-container">
      <div class="tab-list">
        <v-btn
          text
          id="tab-item-0"
          class="tab-list-btn text-none rounded-sm"
          @click="activeTab = 0"
        >
          <v-text class="text--grey"> Tab-0 </v-text>
        </v-btn>
        <v-btn
          text
          id="tab-item-1"
          class="tab-list-btn text-none rounded-sm"
          @click="activeTab = 1"
        >
          <v-text class="text--grey"> onomatopoeia </v-text>
        </v-btn>
        <v-btn
          text
          id="tab-item-2"
          class="tab-list-btn text-none rounded-sm"
          @click="activeTab = 2"
        >
          <v-text class="text--grey"> Tab-2 </v-text>
        </v-btn>
        <v-btn
          text
          id="tab-item-3"
          class="tab-list-btn text-none rounded-sm"
          @click="activeTab = 3"
        >
          <v-text class="text--grey"> Tab-3 </v-text>
        </v-btn>
      </div> 
    </div> -->

    <div class="tabs experience-content-container">
      <div class="tab-list">
        <v-btn
          text
          class="tab-list-btn text-none"
          v-for="item in tabs"
          :key="item.title"
        >
          {{ item.title }}
        </v-btn>
      </div>
    </div>
  </v-card>
</template>

<script>
export default {
  data: () => {
    return {
      tabs: [
        { title: "Tab-0", content: "Content-0" },
        { title: "Tab-1", content: "Content-1" },
        { title: "Tab-2", content: "Content-2" },
        { title: "Tab-3", content: "Content-3" },
      ],
    };
  },
};
</script>
