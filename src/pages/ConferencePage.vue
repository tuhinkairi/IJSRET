<template>
    <div>
      <TopHeader />
      <MenuStyle1 />
      <PageHeader pageTitle="Conference" parentPage="Pages" />
      <Conference/>
      <Footer />
    </div>
  </template>
  
  <script>
  import TopHeader from "@/components/layout/TopHeader";
  import MenuStyle1 from "@/components/layout/MenuStyle1";
  import Conference from "@/components/page_components/conference/Conference.vue"
  import PageHeader from "@/components/layout/PageHeader";
  import Footer from "@/components/layout/Footer";
  
  export default {
    name: "Career",
    components: {
      TopHeader,
      MenuStyle1,
      Conference,
      PageHeader,
      Footer,
    },
  };
  </script>
  
  <style scoped>
  </style>
  