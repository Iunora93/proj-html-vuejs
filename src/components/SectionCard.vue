<script>
import AppCard from "./AppCard.vue";
export default {
  name: "SectionCard",
  components:{
    AppCard,
  },
  data() {
    return {
      cards: [
        {
            src: "./src/assets/imgSpa/Layer-1-new.jpg",
            titolo: "Hydrotherapy",
            info: "Vestibulum nec velit ante.Praesent dignissim interdum est,in lacinia elit pretium nec.Aliquam erat volutpat.Fusce laoreet mi leo",
            titoloHover: "Hydrotherapy",
        },
        {
            src: "./src/assets/imgSpa/Layer-2-new.jpg",
            titolo: "Massage",
            info: "Vestibulum nec velit ante.Praesent dignissim interdum est,in lacinia elit pretium nec.Aliquam erat volutpat.Fusce laoreet mi leo",
            titoloHover: "Massage",
        },
        {
            src: "./src/assets/imgSpa/Layer-3-new.jpg",
            titolo: "Aromatherapy",
            info: "Vestibulum nec velit ante.Praesent dignissim interdum est,in lacinia elit pretium nec.Aliquam erat volutpat.Fusce laoreet mi leo",
            titoloHover: "Aromatherapy",
        },
        {
            src: "./src/assets/imgSpa/Layer-4-new.jpg",
            titolo: "Heat Therapy",
            info: "Vestibulum nec velit ante.Praesent dignissim interdum est,in lacinia elit pretium nec.Aliquam erat volutpat.Fusce laoreet mi leo",
            titoloHover: "Heat Therapy",
        },
        {
            src: "./src/assets/imgSpa/Layer-5-new.jpg",
            titolo: "Skin Care",
            info: "Vestibulum nec velit ante.Praesent dignissim interdum est,in lacinia elit pretium nec.Aliquam erat volutpat.Fusce laoreet mi leo",
            titoloHover: "Skin Care",
        },
        {
            src: "./src/assets/imgSpa/Layer-6-new.jpg",
            titolo: "Spa Days",
            info: "Vestibulum nec velit ante.Praesent dignissim interdum est,in lacinia elit pretium nec.Aliquam erat volutpat.Fusce laoreet mi leo",
            titoloHover: "Spa Days",
        },
        {
            src: "./src/assets/imgSpa/layer8-new.jpg",
            titolo: "Beauty Treatments",
            info: "Vestibulum nec velit ante.Praesent dignissim interdum est,in lacinia elit pretium nec.Aliquam erat volutpat.Fusce laoreet mi leo",
            titoloHover: "Beauty Treatments",
        },
        {
            src: "./src/assets/imgSpa/Layer-7-new.jpg",
            titolo: "Residential",
            info: "Vestibulum nec velit ante.Praesent dignissim interdum est,in lacinia elit pretium nec.Aliquam erat volutpat.Fusce laoreet mi leo",
            titoloHover: "Residential",
        },
         
      ],
      
    };
  },
};
</script>

<template>
  <div>
    <AppCard
        class="cards"
        v-for="card in cards"
        :img="card.src"
        :title="card.titolo"
        :info="card.info"
        :hover="card.titoloHover"
      />
  </div>
</template>

<style lang="scss" scoped>
div{
  display: flex;
  flex-wrap: wrap;
}

</style>