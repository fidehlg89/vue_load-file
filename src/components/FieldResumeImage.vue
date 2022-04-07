<template>
  <div class="d-sm-inline-flex w-100">
    <div>
      <img :src="image" />
    </div>
    <div class="align-self-center pl-sm-3 pt-3 pt-sm-0">
      <input type="file" @change="onImageChange($event)" />
    </div>
  </div>
</template>

<script>
export default {
  name: "FieldResumeImage",

  data() {
    return {
      image: require("../assets/logo.png"),
    };
  },

  methods: {
    onImageChange(e) {
      console.log("Imagen Cargada" + e);
    },
  },
};
</script>

<style scoped>
img {
  width: 100px;
  height: 100px;
  border-radius: 50%;
}
</style>
