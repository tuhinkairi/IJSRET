<template>
  <div class="paperdetails-container" v-if="paperPage">
    <div class=" paperBox mb-4 p-3">
      <div class="header-container  handelPaperDetails">
        <h1 style=" max-width: 400px;">{{ paperDetails.paper_title }}</h1>
        <div class="">
          <b-button 
          style="margin-top:24px ;"
            variant="outline-primary"
            @click="downloadPDF(paperDetails.paper_url)"
            >Download PDF</b-button
          >
        </div>
      </div>
      <div class="details-container mt-4 p-3">
        <p class="pb-3"><b>Author(s) : </b>{{ paperDetails.paper_author }}</p>
        <p class="pb-3">
          <b>Submission-Year,Month : </b>{{ paperDetails.year }},
          {{ paperDetails.month }}
        </p>
        <p class="pb-3"><b>Pages : </b>{{ paperDetails.paper_pages }}</p>
        <p class="pb-3">
          <b>Article Type : </b>{{ paperDetails.paper_articletype }}
        </p>
        <p class="pb-3"><b>DOI : </b>{{ paperDetails.paper_doi }}</p>
      </div>
    </div>
    <div class="row p-3 paperBox">
      <h4 class="mb-2">Abstract</h4>
      <p class="abstract-details">{{ paperDetails.paper_abstract }}</p>
    </div>
  </div>
</template>

<script>
export default {
  namee: "PaperDetailsComponent",
  props: {
    paperDetails: Object,
    paperPage: Boolean,
  },
  methods: {
    downloadPDF(paperURL) {
      window.open(paperURL, "_blank");
    },
  },
  mounted() {
    console.log(
      "Paper details received in PaperDetailsComponent:",
      this.paperDetails
    );
  },
};
</script>
<style scoped>
.rowSize {
  width: 97%;
}
.issueButton {
  cursor: pointer;
}
.box {
  background: #d1a614;
  border-radius: 8px;
}
.box p {
  color: #fff;

  text-align: center;
  padding: 6px;
}

.btn-outline-primary {
  color: #d1a614;
  border-color: #d1a614;
}

.btn-outline-primary:hover {
  color: #fff;
  border-color: #d1a614;
  background: #d1a614;
}

.databox {
  background-color: #d1a614;
  border-radius: 5px;
  cursor: pointer;
}
.databox p {
  color: #fff;
  padding: 10px;
}
.paperBox {
  /* border: 2px solid #EEEDE7; */

  border-radius: 10px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
}
.paperHeading {
  display: flex;
  justify-content: center;
}
p {
  margin-bottom: 5px;
  text-align: left;
}
h5 {
  margin-bottom: 5px;
  margin-top: 5px;
}
h6 {
  margin-bottom: 5px;
  margin-top: 5px;
}
.abstract-details {
  white-space: pre-wrap;
}
@media screen and (max-width: 991px) {
  .btn-sm {
    font-size: 12px !important;
  }
}
@media screen and (max-width: 512px) {
  .btn-sm {
    font-size: 10px !important;
  }
}
@keyframes blink {
  0% {
    opacity: 1;
  }

  50% {
    opacity: 0;
  }

  100% {
    opacity: 1;
  }
}

.blink {
  animation: blink 0.5s infinite;
  background-color: #d1a614;
  border-radius: 5px;
  color: #fff;
  font-weight: bold;
  padding: 5px;
}

.shadow-effect {
  box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
  padding: 8px;
  border-radius: 5px;
}
.image-container {
  display: flex;
  flex-wrap: wrap;
  box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
  padding: 2px;
}

.image-wrapper {
  flex: 0 0 50%;
  /* Each image takes up 50% of the row, so 2 images per row */
  box-sizing: border-box;
  /* Ensures padding and border are included in the width */
  padding: 5px;
  /* Adjust padding as needed */
  display: flex;
  justify-content: center;
  align-items: center;
}

.image-wrapper img {
  max-width: 100%;
  /* Ensures images are responsive */
  height: auto;
  /* Maintains aspect ratio */
  margin-bottom: 10px;
}
@media screen and (max-width: 1000px) {
  .left-side-container {
    display: none;
  }
  .right-side-container {
    display: none;
  }
}
.handelPaperDetails {
  display: flex;
  flex-direction: row; /* Default to row layout */
  justify-content: space-between;
}


@media (max-width: 721px) {
  .handelPaperDetails {
    flex-direction: column; /* Switch to column layout on smaller screens */
  }
}
</style>
