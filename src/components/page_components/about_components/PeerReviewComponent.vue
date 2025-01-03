<template>
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
            <div class="row">
              <div class="col-lg-12 col-md-9">
                <div class="row gy-4 px-4 peer-review-policy">
                  <div>
                    <h3 class="pt-4 headingThree">Peer Review Policy:</h3>
                    <div class="ps-3">
                      <p>
                        International Journal of Scientific Research in Engineering
                        and Technology (IJSREAT) (Online), a bi-monthly worldwide
                        journal developed by academics, educators, engineers, and
                        business leaders to publish innovative ideas. International
                        Journal of Scientific Research in Engineering and
                        Technology, diverse engineering disciplines, and so on are
                        all components of the research outcomes and fundamental
                        progress. IJSREAT is a scholarly, open, accessible, Double
                        Blind Peer Review Journal that assists academics and
                        students. IJSREAT allows academics and industries to propose
                        innovative research and applications in various engineering
                        disciplines and advanced technologies.
                      </p>
                      <P>
                        The role of reviewers in scholarly publishing is crucial.
                        IJSREAT (International Journal of Scientific Research in
                        Engineering & Technology) employs a double-blind peer review
                        procedure, which means that the identities of the
                        reviewer(s) and author(s) are kept a secret throughout the
                        review process. As a result, neither the author(s) nor the
                        reviewer(s) of the paper will be able to determine the
                        identity of the other (s). Peer review enhances networking
                        opportunities within research communities and assists in
                        validating research by establishing a framework for its
                        evaluation. Despite its detractors, peer review remains the
                        only widely accepted method of research validation. All
                        submitted papers will be subjected to a double-blind peer
                        review process, which may take up to three weeks from the
                        submission date. We recommend that all authors refrain from
                        submitting the same International Journal Paper to multiple
                        journals. It would be best if you waited for the paper's
                        review status.
                      </P>
                    </div>

                    <div>
                      <h6 class="pb-2 pt-3">
                        IJSREAT is committed to expediting the evaluation and
                        publication of entirely accepted papers. All submissions are
                        subjected to a strict review process to ensure a
                        high-quality publication. The following are the
                        characteristics of the peer review process:
                      </h6>
                      <ul>
                        <li>
                          <p>
                            Simultaneous submissions of the same manuscript to
                            different journals will not be tolerated.
                          </p>
                        </li>
                        <li>
                          <p>
                            Manuscripts with contents outside the scope will not be
                            considered for review..
                          </p>
                        </li>
                        <li>
                          <p>
                            International Journal Papers will be refereed by at
                            least 3 or 4 experts (reviewers) as suggested by the
                            editorial board, of which 01 from India and the rest 02
                            or 03 from overseas.
                          </p>
                        </li>
                        <li>
                          <p>
                            In addition, Editors will have the option of seeking
                            additional reviews when needed.
                          </p>
                        </li>
                        <li>
                          <p>
                            Authors will be informed when Editors decide further
                            review is required. The journal's Editors-in-Chief makes
                            all publication decisions based on the referees' reports
                            (reviewer's report).
                          </p>
                        </li>
                        <li>
                          <p>
                            Authors of papers that are not accepted are notified
                            promptly.
                          </p>
                        </li>
                        <li>
                          <p>
                            All submitted manuscripts are treated as confidential
                            documents. The double-blind review process will review
                            all submitted papers.
                          </p>
                        </li>
                        <li>
                          <p>
                            All manuscripts submitted for publication in IJSREAT (International Journal of Scientific
                            Research in Engineering & Technology) were cross-checked for plagiarism software.
                            Manuscripts found to be plagiarized during the initial stages of review are outrightly
                            rejected and not considered for publication in the journal.
                          </p>
                        </li>
                        <li>
                          <p>
                            Suppose a manuscript is found to be plagiarized after
                            publication. In that case, the Editor-in-Chief will
                            conduct a preliminary investigation, possibly with the
                            help of an appropriate committee constituted for the
                            purpose. If the manuscript is found to be plagiarized
                            beyond the acceptable limits, the journal will contact
                            the author's Institute / College / University and
                            Funding Agency, if any.
                          </p>
                        </li>
                      </ul>
                      <h6>
                        IJSREAT strictly uses the following double-blind peer review
                        process
                      </h6>
                    </div>
                  </div>

                  <div class="peer-review-process">
                    <div>
                      <h5>Peer review process:</h5>
                      <div class="ps-3">
                        <p>
                          Submissions to the International Journal of Scientific
                          Research in Engineering and Technology (IJSREAT) pass
                          through a double-blind peer-review process. The criteria
                          for publication in the International Journal of Scientific
                          Research in Engineering and Technology (IJSREAT) are as
                          follows:
                        </p>
                      </div>
                      <ul>
                        <li>
                          <p>
                            The paper reveals the findings of first-rate academic
                            research.
                          </p>
                        </li>
                        <li>
                          <p>
                            The stated findings have yet to be published elsewhere.
                          </p>
                        </li>
                        <li>
                          <p>
                            The study adheres to all applicable ethical and
                            scientific integrity requirements.
                          </p>
                        </li>
                        <li>
                          <p>
                            Experiments, statistics, and other analyses are carried
                            out to a high technical quality and are thoroughly
                            reported.
                          </p>
                        </li>
                        <li>
                          <p>
                            The data is used to support the conclusions which are
                            presented correctly.
                          </p>
                        </li>
                        <li>
                          <p>
                            The paper is written in Standard English and presented
                            understandably.
                          </p>
                        </li>
                      </ul>
                      <div class="ps-3">
                        <p>
                          Once the manuscripts have passed quality control, they are
                          assigned to a member of the Editorial Board (or an expert
                          who is not a member) to conduct the peer-review process
                          and decide to accept, invite revision of, or reject the
                          article.
                        </p>
                      </div>
                    </div>
                  </div>
                </div>
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
h3,
h5,
h6 {
  font-family: "Rubik", sans-serif;
}

h6 {
  padding: 10px 0 10px 0;
}

h5 {
  padding-bottom: 10px;
  font-size: 18px;
}

h3 {
  padding-bottom: 20px;
  font-size: 24px;
}

p {
  font-size: 16px;
  font-family: "Rubik", sans-serif;
  color: rgb(100, 117, 137);
  text-align: justify;
  text-justify: inter-word;
}

.reviewList {
  margin-left: -20px;
}

.reviewImage img {
  padding: 40px 80px 0 0;
  max-width: 107%;
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