<template>
    <div>
      <section class="speciality-area">
        <div class="container">
          <div class="row justify-content-between">
            <div
            class="col-lg-6 speciality-text wow animate__animated animate__slideInRight"
          >
            <div class="section-heading w-100 mb-28 mt-0">
              <h1 class="whyChoose">Why choose the IJSREAT journal?</h1>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>
                  Strict Plagiarism Policy
                </p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>
                  Good Impact Factor
                </p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>Peer Reviewed Journal</p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>
                  Open Access Journal
                </p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>Reputed Editorial Board</p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>
                  Rapid/Fast Track Publication
                </p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>
                  Fully Archived Journal
                </p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>
                  High Visibility & Indexing
                </p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>
                  High Impact Factor Journal
                </p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>
                  Response Will Be Given Within 12 Hours.
                </p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>
                  The Paper Will Be Reviewed Within Two Days.
                </p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>
                  The author Will Get Their Acceptance/Rejection Notification Within 3 Days Of Submitting the Paper.
                </p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>
                  All The Accepted Papers Will Be Open and Accessible With a Full PDF Download.
                </p>
              </div>
            </div>
            <div class="speciality">
              <div class="sp-text">
                <img alt="image" src="@/assets/Images/tick.png" class="tick" width="24" height="25"/>
                <p>
                  All Authors Will Get a Soft Copy Of the Certificate, Letter Of Acceptance, Reviewer Evaluation Grading
                </p>
              </div>
            </div>
            
            <!-- <a
              href="javascript:void(0)"
              class="wow animate__animated animate__flipInX animate__delay-1s large-blue-button mt-40 speciality-button"
              >Contact Us</a
            > -->
          </div>
          <div
            class="col-xl-5 col-lg-6 wow animate__animated animate__slideInLeft"
          >
          <div class="sp-box-icon text-center">
            <div class="">
            <div class="about-image">
              <img alt="image"
                src="../../../../assets/Images/Why.png"
                class="publish-image"
              />
            </div>
          </div>
          </div>
          </div>
          </div>
        </div>
      </section>
    </div>
  </template>
  
  <script>
//   import ICountUp from "vue-countup-v2";
  
  export default {
    name: "Speciality",
    components: {
    //   ICountUp,
    },
    data() {
      return {
        instance: "",
        options: {
          useGrouping: false,
          startVal: 0,
          duration: 3,
          suffix: "+",
          useEasing: false,
        },
        options2: {
          useGrouping: false,
          startVal: 0,
          duration: 2,
          suffix: "+",
          useEasing: false,
          prefix: 0
        },
      };
    },
  };
  </script>
  
  <style scoped>
  .tick {
    margin-right: 10px;
  }
  .whyChoose {
    color: #D1A614;
  }
  .publish-image{
    width: 80%;
    height: 80%;
  }
  </style>
  
