<template>
  <Details>
    <template v-slot:Header>
      <Header :imgSrc="imgSrc" />
    </template>
    <template v-slot:Body>
      <p>{{ $t("protection") }}</p>
    </template>
  </Details>
</template>
<script>
import Details from "../components/details";
import Header from "../components/header";
export default {
  components: {
    Details,
    Header
  },
  props: {
    imgSrc: {
      type: String,
      default: `${process.env.BASE_URL}img/icons/how-to-protect-head.svg`
    }
  }
};
</script>
