<template>
  <div>
    <section class="speciality-area">
      <div class="container">
        <div v-if="viewPaper" class="main-paper-header p-2">
          <div class="article-header">
            <h4>{{ mainPageObj.title }}</h4>
            <button
              type="submit"
              @click="openPaperDetails"
              class="viewArticlebtn p-2"
            >
              View Article
            </button>
          </div>
          <div>
            <h6>{{ mainPageObj.name }}</h6>
            <p><b>Organized By : </b>{{ mainPageObj.conductedBy }}</p>
            <p><b>Conference Date : </b>{{ mainPageObj.conferenceDate }}</p>
          </div>
        </div>
        <div v-if="!viewPaper && paperpage">
          <div class="header-title p-2 mb-4">
            <h4>2024 | Volume 4 - Issue 3 | REACT'24</h4>
          </div>
          <div
            v-for="items in paperDetails"
            :key="items.id"
            class="paper-container p-2 mb-3"
          >
            <div class="flex sub-header-title">
              <div>
                <h4>{{ items.title }}</h4>
              </div>

              <div>
                <button type="button" class="download-pdf p-2" @click="downloadPdf">
                  Download PDF
                </button>
              </div>
            </div>
            <div>
              <p><b>Author: </b>{{ items.author }}</p>
              <p><b>Article Type: </b>{{ items.articleType }}</p>
              <p><b>Pages: </b>{{ items.pages }}</p>
            </div>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
import React24 from "../../../util/conference-react24";
export default {
  data() {
    return {
      viewPaper: true,
      paperpage:false,
      paperDetails: React24.papersList,
      mainPageObj: {
        title: "REACT-2024",
        name: "Recent Advances in Civil Engineering and Technology-2024",
        conductedBy: "Vidya Academy of Science and Technology, Kerala, India",
        conferenceDate: "19 & 20 June2024",
      },
    };
  },
  methods: {
    openPaperDetails() {
      this.$router.push({ path: "conference", query: { id: "react23" } });
      this.viewPaper = false;
      this.paperpage = true 
    },
    downloadPdf(){
        console.log('download')
    }
  },
  watch:{
    $route: function(){
        if('id' in this.$route.query){
            this.paperpage= true
            this.viewPaper = false
        } else{
            this.paperpage= false
            this.viewPaper = true
        }
    }
  }
};
</script>
<style scoped>
.download-pdf {
  border: 1px solid #d1a614;
  color: #d1a614;
  background: transparent;
  font-weight: 600;
  border-radius: 5px;
}
.download-pdf:hover{
    color:#fff;
    background-color: #d1a614;
}
.header-title {
  border-radius: 5px;
  text-align: center;
  box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
}
.paper-container {
  box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
  border-radius: 5px;
}
.sub-header-title {
  display: flex;
  justify-content: space-between;
}
.viewArticlebtn {
  border: 1px solid #d1a614;
  color: #d1a614;
  background: transparent;
  font-weight: 600;
  border-radius: 5px;
}
.viewArticlebtn:hover{
    color:#fff;
    background-color: #d1a614;
}
.article-header{
    display: flex;
    justify-content: space-between;
}
.main-paper-header{
    box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
    border-radius: 5px;
}
</style>
