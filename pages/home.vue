<template>
  <main>
    <section class="banner-sec">
      <div class="container">
        <h2 class="display-3 mb-4">{{title}}</h2>
        <p class="lead mb-2">{{subTitle}}</p>
        <p class="description mb-5">{{description}}</p>
        <nuxt-link class="btn btnx btn-lg text-dark" to="/product" role="button">Know more</nuxt-link>
      </div>

      <!--blade section-->
    </section>

    <div class="container">
      <Card />
    </div>
  </main>
</template>

<script>
import Card from "./card";
export default {
  components: {
    Card
  },
  data() {
    return {
      title: "WELCOME",
      subTitle:
        "Our Store Present Some New Technological And Powerful Blades Which Will Gives You Long Last And Durability.",
      description:
        "Check Our Newest and Amazing Blades Which Are Newly Comes In Our Store .................."
    };
  }
};
</script>

<style scoped>
.fw h3,
h4 {
  font-weight: bold;
}
.btnx {
  background-color: coral;
}
.banner-sec {
  background: url('~assets/images/top-banner.jpg');
  background-size: 100%;
  padding: 90px 0;
  background-size: cover;
}
.banner-sec h2 {
  color: #fff;
  padding-bottom: 10px;
}
.banner-sec p {
  color: #fff;
}
.lead {
  font-size: 20px;
  font-weight: 300;
}
.description {
  font-weight: 400;
}
</style>
