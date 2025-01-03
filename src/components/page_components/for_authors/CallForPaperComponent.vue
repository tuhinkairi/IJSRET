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
          <h3>Call for Papers:</h3>
          <div class="callForPaperContent">
            <p>
              International Journal Of Scientific Research In Engineering And
              Technology (IJSREAT) has ISSN: 2583-1240 (online), Bi-Monthly
              international journal by Fifth Dimension Research Publication.
            </p>
            <p>
              It is an academic, online, open access, Double - Blind,
              Peer-reviewed international journal. It aims to publish original,
              theoretical, and practical advances in Computer Science &
              Engineering, Information Technology, Electrical and Electronics
              Engineering, Electronics and Telecommunication, Mechanical
              Engineering, Civil Engineering, Textile Engineering, and all
              interdisciplinary streams of Engineering Sciences. The board of
              committee of IJSREAT (International Journal Of Scientific Research
              In Engineering And Technology) will review all submitted papers.
            </p>
            <p>
              International Journal Papers  for the regular issues of the Journal can be submitted,
              around the year, electronically at editorinchief@ijsreat.com.
              After the final acceptance of the paper, based upon the detailed
              review process, it will immediately be published online. However,
              the assignment of the report to a specific Volume / Issue (see
              archive) of the Journal will be taken up by the Editorial Board
              later; and the author will be intimated consequently. For Theme
              Based Special Issues, time-bound Special Calls for Papers will be
              informed, and the same will only apply to that specific issue.
            </p>
          </div>
          <div class="callForPaperContent">
            <h6>
              For the author’s convenience, we strongly follow the following
              steps.
            </h6>
            <p>
              <b
                >Last Date for Manuscript Submission: 25th of every Bimonthly
                (Feb,Apr,Jun,Aug,Oct,Dec)
              </b>
            </p>
            <div class="paperList">
              <ul>
                <li>
                  <p>The response will be given within 12 hours.</p>
                </li>
                <li>
                  <p>The paper will be reviewed within Two days.</p>
                </li>
                <li>
                  <p>
                    The author will get their Acceptance/Rejection Notification
                    within three days of submitting the paper.
                  </p>
                </li>
                <li>
                  <p>
                    All the accepted papers will be open and accessible with a
                    full PDF download.
                  </p>
                </li>
                <li>
                  <p>
                    All Authors will get a Soft copy of the certificate,
                    acceptance letter, and reviewer evaluation grading.
                  </p>
                </li>
              </ul>
            </div>
            <h6>
              Submit your article:<i>editorinchief@ijsreat.com</i> (or)Online
              submission
            </h6>
          </div>
        </div>
      </div>
      <div style="width: 200px;" class="right-side-container ml-2"
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
  methods:{
    getManuScript: function (getUrl) {
      window.open(getUrl, "_blank");
    },
    getCopyRightForm: function (getForm) {
      window.open(getForm, "_blank");
    },
  }
};
</script>

<style scoped>
h6 {
  font-family: "Rubik", sans-serif;
}
p {
  font-size: 16px;
  font-family: "Rubik", sans-serif;
  color: rgb(100, 117, 137);
  text-align: justify;
  text-justify: inter-word;
}
h3 {
  font-family: "Rubik", sans-serif;
  padding-bottom: 20px;
  font-size: 24px;
}
.callForPaperContent {
  padding-bottom: 10px;
}
.paperList {
  margin-left: -20px;
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