<template>
  <v-card flat color="transparent" class="has-anchor">
    <v-subheader class="text-h4">
      <span class="text-none teal--text text--accent-1 text-h5 pr-3">
        02.
      </span>
      Experience
      <div class="horizontal-bar ml-5" />
    </v-subheader>

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
              <p class="range main-color">{{ tab.date }}</p>
              <ul>
                <li class="tab-content-list main-color">
                  {{ tab.content1 }}
                </li>
                <li class="tab-content-list main-color">
                  {{ tab.content2 }}
                </li>
                <li class="tab-content-list main-color">
                  {{ tab.content3 }}
                </li>
                <li class="tab-content-list main-color">
                  {{ tab.content4 }}
                </li>
              </ul>
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
          position: "Pro Associate",
          date: "May 31, 2021 - Present",
          content1:
            "Pro Associates are primarily responsible for outstanding customer service and ensuring transactions are handled quickly and accurately.",
          content2:
            "The Pro Associate will drive customer acquisition by asking probing project questions and be knowledgeable about Pro loyalty programs.",
          content3:
            "This position will utilize Pro benefits to drive sales by using bulk pricing, Pro Xtra, credit solutions, etc.",
          content4:
            "They will work at the Pro desk responding to general questions, and will transition Managed Account customers and quote building tasks to the PASA.",
        },
        {
          company: "Auntie Anne's",
          position: "Team Member",
          date: "October 2020 - January 2021",
          content1:
            "Follow and implement step by step instructions on the preparation, production, and distribution of goods.",
          content2: "Process customer orders in a fast-paced environment.",
          content3: "Assist customers and report to management daily.",
          content4:
            "Work in a team environment to solve and complete problems in a short time frame.",
        },
        {
          company: "Shanna Erdman",
          position: "Babysitter",
          date: "September 2020 - January 2021",
          content1:
            "Successfully balanced work and academics by simultaneously engaging and ensuring the safety of two children under the age of 10, while amassing a 3.71 GPA for the final semester.",
          content2:
            "Aided children in completing and understanding coursework while they were participating in virtual classes during the pandemic.",
          content3:
            "Conducted a daily report on the behavior and achievements of the children.",
          content4:
            "Frequently settled disputes with compromise and reasoning.",
        },
        {
          company: "Non-Existent",
          position: "Nothing",
          date: "January 2017 - January 2018",
          content1:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Porttitor massa id neque aliquam vestibulum morbi. Adipiscing elit ut aliquam purus sit amet. Dolor sit amet consectetur adipiscing elit ut aliquam purus. Arcu felis bibendum ut tristique et egestas quis. Sit amet porttitor eget dolor morbi. Proin nibh nisl condimentum id venenatis a condimentum vitae. Ut pharetra sit amet aliquam id diam maecenas u",
          content2:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Porttitor massa id neque aliquam vestibulum morbi. Adipiscing elit ut aliquam purus sit amet. Dolor sit amet consectetur adipiscing elit ut aliquam purus. Arcu felis bibendum ut tristique et egestas quis. Sit amet porttitor eget dolor morbi. Proin nibh nisl condimentum id venenatis a condimentum vitae. Ut pharetra sit amet aliquam id diam maecenas u",
          content3:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Porttitor massa id neque aliquam vestibulum morbi. Adipiscing elit ut aliquam purus sit amet. Dolor sit amet consectetur adipiscing elit ut aliquam purus. Arcu felis bibendum ut tristique et egestas quis. Sit amet porttitor eget dolor morbi. Proin nibh nisl condimentum id venenatis a condimentum vitae. Ut pharetra sit amet aliquam id diam maecenas u",
          content4:
            "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Porttitor massa id neque aliquam vestibulum morbi. Adipiscing elit ut aliquam purus sit amet. Dolor sit amet consectetur adipiscing elit ut aliquam purus. Arcu felis bibendum ut tristique et egestas quis. Sit amet porttitor eget dolor morbi. Proin nibh nisl condimentum id venenatis a condimentum vitae. Ut pharetra sit amet aliquam id diam maecenas u",
        },
      ],
    };
  },
};
</script>
