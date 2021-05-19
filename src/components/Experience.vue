<template>
  <v-card flat color="transparent" class="has-anchor">
    <v-subheader class="text-h4">
      <v-text class="text-none teal--text text--accent-1 text-h5 pr-3">
        02.
      </v-text>
      Experience
      <div class="horizontal-bar ml-5" />
    </v-subheader>

    <div class="experience-content-container">
      <div class="tab-list">
        <v-btn
          text
          id="tab-item-0"
          class="tab-list-btn text-none rounded-sm"
          @click="tab0 = !tab0"
        >
          <v-text class="text--grey"> Tab-0 </v-text>
        </v-btn>
        <v-btn
          text
          id="tab-item-1"
          class="tab-list-btn text-none rounded-sm"
          @click="tab1 = !tab1"
        >
          <v-text class="text--grey"> onomatopoeia </v-text>
        </v-btn>
        <v-btn
          text
          id="tab-item-2"
          class="tab-list-btn text-none rounded-sm"
          @click="tab2 = !tab2"
        >
          <v-text class="text--grey"> Tab-2 </v-text>
        </v-btn>
        <v-btn
          text
          id="tab-item-3"
          class="tab-list-btn text-none rounded-sm"
          @click="tab3 = !tab3"
        >
          <v-text class="text--grey"> Tab-3 </v-text>
        </v-btn>
      </div>

      <v-card-text class="tab-textbox text-body-1 grey--text" v-show="tab0">
        Exp0 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
        eiusmod tempor incididunt ut labore et dolore magna aliqua. Faucibus
        pulvinar elementum integer enim. At elementum eu facilisis sed odio
        morbi quis commodo odio. Sed faucibus turpis in eu mi bibendum neque
        egestas. Tincidunt tortor aliquam nulla facilisi cras fermentum odio eu.
        Eget nullam non nisi est. Nibh nisl condimentum id venenatis a. Egestas
        pretium aenean pharetra magna ac placerat vestibulum. Quis hendrerit
        dolor magna eget est. Sit amet nulla facilisi morbi tempus iaculis urna
        id. Scelerisque viverra mauris in aliquam sem fringilla ut. Bibendum
        neque egestas congue quisque egestas diam in. Felis bibendum ut
        tristique et egestas quis.
      </v-card-text>
      <v-card-text class="tab-textbox text-body-1 grey--text" v-show="tab1">
        Exp1 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
        eiusmod tempor incididunt ut labore et dolore magna aliqua. Faucibus
        pulvinar elementum integer enim. At elementum eu facilisis sed odio
        morbi quis commodo odio. Sed faucibus turpis in eu mi bibendum neque
        egestas. Tincidunt tortor aliquam nulla facilisi cras fermentum odio eu.
        Eget nullam non nisi est. Nibh nisl condimentum id venenatis a. Egestas
        pretium aenean pharetra magna ac placerat vestibulum. Quis hendrerit
        dolor magna eget est. Sit amet nulla facilisi morbi tempus iaculis urna
        id. Scelerisque viverra mauris in aliquam sem fringilla ut. Bibendum
        neque egestas congue quisque egestas diam in. Felis bibendum ut
        tristique et egestas quis.
      </v-card-text>
      <v-card-text class="tab-textbox text-body-1 grey--text" v-show="tab2">
        Exp2 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
        eiusmod tempor incididunt ut labore et dolore magna aliqua. Faucibus
        pulvinar elementum integer enim. At elementum eu facilisis sed odio
        morbi quis commodo odio. Sed faucibus turpis in eu mi bibendum neque
        egestas. Tincidunt tortor aliquam nulla facilisi cras fermentum odio eu.
        Eget nullam non nisi est. Nibh nisl condimentum id venenatis a. Egestas
        pretium aenean pharetra magna ac placerat vestibulum. Quis hendrerit
        dolor magna eget est. Sit amet nulla facilisi morbi tempus iaculis urna
        id. Scelerisque viverra mauris in aliquam sem fringilla ut. Bibendum
        neque egestas congue quisque egestas diam in. Felis bibendum ut
        tristique et egestas quis.
      </v-card-text>
      <v-card-text class="tab-textbox text-body-1 grey--text" v-show="tab3">
        Exp3 Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
        eiusmod tempor incididunt ut labore et dolore magna aliqua. Faucibus
        pulvinar elementum integer enim. At elementum eu facilisis sed odio
        morbi quis commodo odio. Sed faucibus turpis in eu mi bibendum neque
        egestas. Tincidunt tortor aliquam nulla facilisi cras fermentum odio eu.
        Eget nullam non nisi est. Nibh nisl condimentum id venenatis a. Egestas
        pretium aenean pharetra magna ac placerat vestibulum. Quis hendrerit
        dolor magna eget est. Sit amet nulla facilisi morbi tempus iaculis urna
        id. Scelerisque viverra mauris in aliquam sem fringilla ut. Bibendum
        neque egestas congue quisque egestas diam in. Felis bibendum ut
        tristique et egestas quis.
      </v-card-text>
    </div>
  </v-card>
</template>

<script>
export default {
  data: () => {
    return {
      tab0: true,
      tab1: false,
      tab2: false,
      tab3: false,
    };
  },
};
</script>
