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
        <v-tabs background-color="transparent ml-4" vertical>
          <template background-color="transparent" v-for="tab in tabs">
            <v-tab class="text-none" :key="tab.company + 'company'">
              {{ tab.company }}
            </v-tab>
            <v-tab-item class="pt-3 pl-7" :key="tab.company + 'content'">
              <h3>
                {{ tab.position }}
                <span class="company"> @ {{ tab.company }} </span>
              </h3>
              {{ tab.content }}
            </v-tab-item>
          </template>
        </v-tabs>
      </div>
    </div>
  </v-card>
</template>

<script>
export default {
  data: () => {
    return {
      tabs: [
        {
          company: "Home Depot",
          position: "Team Member",
          date: "May 31, 2021",
          content: "Content-0",
        },
        {
          company: "Onomatopoiea",
          position: "Team Member",
          date: "May 31, 2021",
          content: "Content-1",
        },
        {
          company: "Tab-2",
          position: "Team Member",
          date: "May 31, 2021",
          content: "Content-2",
        },
        {
          company: "Tab-3",
          position: "Team Member",
          date: "May 31, 2021",
          content: "Content-3",
        },
      ],
    };
  },
};
</script>
