<script>
import AppTabs from "../components/AppTabs.vue";
export default {
  components: {
    AppTabs,
  },

  data() {
    return {
      tabList: ["Discover A", "Discover B", "Discover C", "Discover D"],
    };
  },
};
</script>

<template>
  <div class="discover" id="discover">
    <img src="../assets/presentation.png" alt="presentation" class="logo" />
    <h2 class="title">DISCOVER</h2>
    <h2 class="sub-title">BOOKED TOOL</h2>
    <img src="../assets/monitor.jpg" alt="monitor" class="monitor" />
    <div class="tab">
      <app-tabs :tabList="tabList">
        <template v-slot:tabPanel-1>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Cum fugit
          tempora molestiae dolor adipisci exercitationem, nemo eveniet quia
          dolorem itaque modi officiis quidem ab veniam animi quod obcaecati
          temporibus est?
        </template>
        <template v-slot:tabPanel-2>
          There was something beautiful in his hate. It wasn't the hate itself
          as it was a disgusting display of racism and intolerance. It was what
          propelled the hate and the fact that although he had this hate, he
          didn't understand where it came from. It was at that moment that she
          realized that there was hope in changing him.
        </template>
        <template v-slot:tabPanel-3>
          The coin hovered in the air, spinning over and over again. It reached
          its peak and began to descend. Both boys were pleading with it to land
          a certain way but the coin had already made up its mind on what it was
          going to do.
        </template>
        <template v-slot:tabPanel-4
          >Don't be scared. The things out there that are unknown aren't scary
          in themselves. They are just unknown at the moment. Take the time to
          know them before you list them as scary. Then the world will be a much
          less scary place for you.</template
        >
      </app-tabs>
    </div>
  </div>
</template>

<style scoped>
.discover {
  padding: 48px 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  height: fit-content;
}

.monitor {
  margin-top: 20px;
  height: 400px;
  border-radius: 12px;
}

.sub-title {
  font-weight: 300;
}
.tab {
  width: 40%;
}

.tab > app-tabs > template {
  color: red;
}
@media only screen and (max-width: 950px) {
  .monitor {
    height: 200px;
    width: auto;
  }
}
</style>
