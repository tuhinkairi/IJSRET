<template>
  <div>
    <section class="speciality-area">
      <div style="display: flex;justify-content: space-around;">
        <div style="width: 200px;" class="left-side-container mr-2"
        >
          <p class="blink mb-5"> <a href="http://editorial.fdrpjournals.org/login?journal=2" style="color: #fff;">Submit
              Research Paper</a> </p>
          <div class="shadow-effect mb-5">
            <h6>Downloads :</h6>
            <p style="cursor: pointer;"
              @click="getManuScript('https://fdrpjournals.s3.ap-south-1.amazonaws.com/main/3/manuscripttemplate/IJSREAT-Manuscript-Template.docx')">

              Manuscript Template
            </p>
            <p style="cursor: pointer;"
              @click="getCopyRightForm('https://fdrpjournals.s3.ap-south-1.amazonaws.com/main/3/copyrightform/IJSREAT_Registration+%26Copyright-Form.pdf')">
              Copyright Form
            </p>
          </div>
          <div class="shadow-effect mb-5">
            <img alt="image" src="../../../assets/Images/isn.jpg" height="90" width="200" />
          </div>
          <div class="shadow-effect mb-5">
            <img alt="image" src="../../../assets/Images/cc.jpg" height="90" width="180" />
            <p>All research Article published on this website are licensed under Creative Commons Attribution-ShareAlike
              4.0
              International License, and all rights belong to their respective authors/researchers.
            </p>
          </div>
          <div>
            <IndexingSideDesign />
          </div>
        </div>
        <div class="container" style="max-width: 1000px !important; margin: 0">
          <div class="row justify-content-between">
            <h3>AIM & SCOPE:</h3>
            <div class="missionContent">
              <h5>Aim</h5>
              <p>
                The International Journal Of Scientific Research in Engineering &
                Technology (IJSREAT) is an international journal dedicated to the
                latest advancements in engineering and technology. This journal
                aims to provide a platform for scientists and academicians
                worldwide to promote, share, and discuss various new issues and
                developments in different areas of engineering and technologies.
              </p>
            </div>
            <div>
              <h5>Scope</h5>
              <p>
                The journal's scope is to provide an academic medium and an
                essential reference for advancing and disseminating research
                results that support high-level learning, teaching, and research
                in engineering & technology. We bring together scientists,
                academicians, engineers, scholars, and students of related fields.
              </p>
              <p>
                The International Journal of Scientific Research in Engineering
                and Technology (IJSREAT) is an open-access, peer-reviewed
                multidisciplinary publication that offers authors a worldwide
                platform to share their research articles online. IJSREAT adheres
                to an open-access paradigm that allows for the unrestricted
                sharing of research papers to the global community via the
                internet. All articles released under open access can be viewed
                freely.
              </p>
            </div>
          </div>
        </div>
        <div style="width: 200px;" class="left-side-container mr-2"
        >
          <div class="mb-5">
            <router-link to="/editorial-board">
              <p class="blink">Join As A reviewer</p>
            </router-link>
          </div>
          <div class="shadow-effect mb-5">
            <img alt="image" src="../../../assets/Images/tur.jpg" height="90" width="180" />
            <p>Plagiarism is checked by the leading plagiarism checker</p>
          </div>
          <div class="shadow-effect mb-5">
            <img alt="image" src="../../../assets/Images/doi.jpg" height="90" width="180" />
            <p>CrossRef DOI is assigned to research Article published in our journal.
              IJIRE DOI prefix is10.59256/ijire
            </p>
          </div>
          <div class="shadow-effect mb-5">
            <h4>For Authors</h4>
            <router-link to="topics">
              <p>Topics</p>
            </router-link>
            <router-link to="call-for-papers">
              <p>Call For Papers</p>
            </router-link>
            <router-link to="instruction-for-author">
              <p>Instruction For Authors</p>
            </router-link>
            <p><a href="http://editorial.fdrpjournals.org/login?journal=2" style="color:rgb(100, 117, 137)">Manuscript
                Submission</a></p>
            <router-link to="guidance-for-ems">
              <p>Guidance For EMS</p>
            </router-link>
            <router-link to="article-processing-charges">
              <p>Article Processing Charges</p>
            </router-link>
            <router-link to="downloads">
              <p>Downloads</p>
            </router-link>
            <router-link to="paper-status">
              <p>Paper Status</p>
            </router-link>
          </div>
          <div class="shadow-effect">
            <h4>Policies</h4>
            <router-link to="ethics">
              <p>Ethics And Policies</p>
            </router-link>
            <router-link to="peer-review-policy">
              <p>Peer Review Policy</p>
            </router-link>
            <router-link to="publication-ethics-policy">
              <p>Publication Ethics Policy</p>
            </router-link>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
import IndexingSideDesign from '@/components/common/IndexingSideDesign.vue'

export default {
  components: {
    IndexingSideDesign
  },
  methods: {
    getManuScript: function (getUrl) {
      window.open(getUrl, "_blank");
    },
    getCopyRightForm: function (getForm) {
      window.open(getForm, "_blank");
    },
  },
};
</script>

<style scoped>
h3 {
  padding-bottom: 20px;
  font-family: "Rubik", sans-serif;
  font-size: 24px;
}

h5 {
  font-family: "Rubik", sans-serif;
  padding-bottom: 10px;
  font-size: 18px;
}

p {
  font-size: 16px;
  font-family: "Rubik", sans-serif;
  color: rgb(100, 117, 137);
  text-align: justify;
  text-justify: inter-word;
}

.missionList {
  margin-left: -20px;
}

.missionContent {
  padding-bottom: 20px;
}
.inr-content {
  color: #D1A614;
  font-weight: bold;
} 

.shadow-effect {
  box-shadow: rgba(99, 99, 99, 0.2) 0px 2px 8px 0px;
  padding: 8px;
  border-radius: 5px;
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
  background-color: #D1A614;
  border-radius: 5px;
  color: #fff;
  font-weight: bold;
  padding: 5px;
}

.editorialBox {
  /* border: 2px solid #EEEDE7; */
  border-radius: 10px;
  box-shadow: rgba(100, 100, 111, 0.2) 0px 7px 29px 0px;
  width: 85%;
}
</style>