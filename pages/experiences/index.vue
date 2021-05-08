<template>
  <section class="hero is-default">
    <div class="hero-body">
      <div class="container">

        <div class="columns is-vcentered is-centered">
            <div class="column is-5 ">
              <span>

              <!-- <div class="container"> -->
                <div class="card is-project-card">
                  <div class="card-image">
                      <figure class="image is-square is-project-image">
                          <a @click="handleClick"><img class="is-project-card" src="~/assets/experiences/kpmg.png"></a>
                      </figure>
                  </div>
                  <div class="card-content">
                      <div class="content">
                          <a @click="handleClick" class="text_project ml-0">KPMG</a>
                          <p class="is-subtitle">Associate Data Scientist & Analytics Modeler</p>
                          <div class=" is-multi-tag" >
                            <div class="funtag" style="margin-bottom: 10px;">
                              <b-tag rounded class="funtag" style="position: absolute; top: 0; margin-left:-75px"><b>python</b></b-tag>
                              <b-tag rounded class="funtag" style="position: absolute; top: 0; margin-left:-9px"><b>data engineering</b></b-tag>
                              <b-tag rounded class="funtag" style="position: absolute; top: 0; margin-left:120px"><b>machine learning</b></b-tag>
                              <b-tag rounded class="funtag" style="position: absolute; top: 0; margin-left:250px"><b>consulting</b></b-tag>
                            </div>
                          </div>
                      </div>
                  </div>
                </div>
                <b-modal v-model="isImageModalActive">
                  <!-- <section class="hero is-full"> -->
                    <div class="card is-project-card">
                      <article  class="hero-body article content">
                        <h3 style="margin-top: -10px">Experience by Area</h3>
                        <strong>Machine Learning</strong>
                        <ul>
                          <li>Designed a Machine Learning fraud detection tool for mortgage lender using random forest model, optimized hyperparameters using Grid Search algorithm; constructed a data aggregation system using VBA code</li>
                          <li>Led data science model pipeline development for Oil & Gas client: created commodities trading prediction pipeline using Airflow, Snowflake, and Azure ML, for US and European markets; devised Azure cloud infrastructure, for continuous development and ML model improvements to support the client’s technical environment and stakeholder needs; configured automated model retraining and deployment pipelines.</li>
                        </ul>
                        <strong>Neural Network</strong>
                        <ul>
                          <li>Created matching algorithm for a computer vision faster-RCNN model output to correlate unindexed object detection predictions to their ground truth equivalents, making error analysis possible. Developed whitespace removal and cutoff amendment post processing algorithms on object detection model results, increased model F1 scores by over 30%.</li>
                          <li>Programmed a recommendation system for stock room products using PySpark neural network implementation of collaborative filtering leading to new onsite sales avenues for life sciences client.</li>
                          <li>Developed a Convolutional Neural Network (CNN) model using Tensorflow to detect and classify animal images to assist biology research project for a University employer.</li>
                        </ul>
                        <strong>Natural Language Processing</strong>
                        <ul>
                          <li>Developed intelligent NLP extraction system for a financial services client which identified loan contracts affected by a deprecated index rate and classified documents based on specific language indicators</li>
                          <li>Programmed statistical NLP models for audit attribute extraction, architected an automated data cleaning process saving dozens of hours of manual work for team, generated attribute normalization system in Java.</li>
                          <li>Conducted sentiment analysis Natural Language Processing to analyze hundreds of thousands of product reviews for global travel technology company, created topic modelling visualizations from LDA to derive insights into spectrum of customer sentiment</li>
                        </ul>
                      </article>
                    </div>
                  <!-- </section> -->
                </b-modal>
              </span>
             </div>
          <div class="column is-5">
            <span>
                <div class="card is-project-card">
                  <div class="card-image">
                      <figure class="image is-square is-project-image">
                          <a @click="handleClick"><img class="is-project-card" src="~/assets/experiences/sdl.png"></a>
                      </figure>
                  </div>
                  <div class="card-content">
                      <div class="content">
                        <a class="text_project" @click="handleClick">Shapiro Design Lab</a>
                        <p class="is-subtitle">Software Developer</p>
                        <div class="field is-grouped multibutton" >
                            <div class=" is-multi-tag" >
                              <div class="funtag" style="margin-bottom: 10px;">
                                <b-tag rounded class="funtag" style="position: absolute; top: 0;margin-left:-75px"><b>tensorflow</b></b-tag>
                                <b-tag rounded class="funtag" style="position: absolute; top: 0;margin-left:13px"><b>vue.js</b></b-tag>
                                <b-tag rounded class="funtag" style="position: absolute; top: 0;margin-left:80px"><b>image classification</b></b-tag>

                                <!-- <b-tag rounded class="funtag" style="position: absolute; top: 0; margin-left:65px;"><b>python</b></b-tag> -->
                              </div>
                            </div>
                          </div>
                      </div>
                  </div>
                </div>
                <b-modal v-model="isImageModalActive">
                  <!-- <section class="hero is-full"> -->
                    <div class="card is-project-card">
                      <article  class="hero-body article content">
                        <h3 style="margin-top: -10px">Software Developer at the Shapiro Design Lab</h3>
                        <strong>Machine Learning</strong>
                        <ul>
                          <li>Worked with the Shapiro Design Lab, the University of Michigan's open library project, to build experiential software and hardware tools to increase the accessibility to Michigan's library system.</li>
                          <li>We assisted Ecologists at Michigan to identify, analyze, and categorize hundreds of thousands of camera trap images from the University of Michigan Biological Research Station using Convolutional Neural Networks (CNN's).</li>
                        </ul>
                      </article>
                    </div>
                  <!-- </section> -->
                </b-modal>
            </span>
              </div>
              <div class="column is-5">
                <span>
                  <div class="card is-project-card">
                    <div class="card-image">
                      <figure class="image is-square is-project-image">
                        <a><img class="is-project-card" src="~/assets/experiences/millipore.png"></a>
                      </figure>
                    </div>
                    <div class="card-content">
                      <div class="content">
                        <a class="text_project">Millipore Sigma</a>
                        <p class="is-subtitle">Data Scientist Intern</p>
                          <div class="field is-grouped multibutton" >
                            <div class=" is-multi-tag" >
                              <div class="funtag" style="margin-bottom: 10px;">
                                <b-tag rounded class="funtag" style="position: absolute; top: 0;margin-left:-75px"><b>reccomender systems</b></b-tag>
                                <b-tag rounded class="funtag" style="position: absolute; top: 0;margin-left:85px"><b>ad optimization</b></b-tag>
                                <b-tag rounded class="funtag" style="position: absolute; top: 0;margin-left:203px"><b>dashboard web dev</b></b-tag>
                              </div>
                            </div>
                          </div>
                        </div>
                      </div>
                    </div>
                    <b-modal v-model="isImageModalActive">
                  <!-- <section class="hero is-full"> -->
                    <div class="card is-project-card">
                      <article  class="hero-body article content">
                        <h3 style="margin-top: -10px">Software Developer at the Shapiro Design Lab</h3>
                        <strong>Machine Learning</strong>
                        <ul>
                          <li>Programmed PySpark neural network model to product recommendations for clients, revamped stock processes for b2b sales</li>
                          <li>Created web app and database system providing insights for lab management processes serving 200 internal sales stakeholders</li>
                          <li>Analyzed adwords traffic; launched campaign of mined competitor keywords generating $2.5 million revenue in 8 weeks</li>
                        </ul>
                      </article>
                    </div>
                  <!-- </section> -->
                </b-modal>
                </span>
                </div>
          </div>

        <div class="columns is-vcentered is-centered">
          <div class="column is-5 ">
            <!-- <div class="container"> -->
              <div class="card is-project-card">
                <div class="card-image">
                    <figure class="image is-square is-project-image">
                        <a><img class="is-project-card" src="~/assets/experiences/ai.png"></a>
                    </figure>
                </div>
                <div class="card-content">
                    <div class="content">
                        <a class="text_project ml-0">Office of Academic Innovation</a>
                        <p class="is-subtitle">Research and Learning Analytics Fellow</p>
                        <div class=" is-multi-tag" >
                          <div class="funtag" style="margin-bottom: 10px;">
                            <b-tag rounded class="funtag" style="position: absolute; top: 0; margin-left:-75px"><b>python mooc course creation</b></b-tag>
                          </div>
                        </div>
                    </div>
                </div>
              </div>
          </div>
          <div class="column is-5">
              <div class="card is-project-card">
                <div class="card-image">
                    <figure class="image is-square is-project-image">
                        <a><img class="is-project-card" src="~/assets/experiences/pse.png"></a>
                    </figure>
                </div>
                <div class="card-content">
                    <div class="content">
                      <a class="text_project">PSE</a>
                      <p class="is-subtitle">Founder, President</p>
                      <div class="field is-grouped multibutton" >
                          <div class=" is-multi-tag" >
                            <div class="funtag" style="margin-bottom: 10px;">
                              <b-tag rounded class="funtag" style="position: absolute; top: 0;"><b>leadership</b></b-tag>
                              <b-tag rounded class="funtag" style="position: absolute; top: 0;margin-left:55px"><b>management</b></b-tag>
                              <!-- <b-tag rounded class="funtag" style="position: absolute; top: 0; margin-left:65px;"><b>python</b></b-tag> -->
                            </div>
                          </div>
                        </div>
                    </div>
                </div>
              </div>
              </div>
              <div class="column is-5">
                <div class="card is-project-card">
                  <div class="card-image">
                    <figure class="image is-square is-project-image">
                      <a><img class="is-project-card" src="~/assets/experiences/ql.png"></a>
                    </figure>
                  </div>
                  <div class="card-content">
                    <div class="content">
                      <a class="text_project">Quicken Loans</a>
                      <p class="is-subtitle">Machine learning Engineer Intern</p>
                        <div class="field is-grouped multibutton" >
                          <div class=" is-multi-tag" >
                            <div class="funtag" style="margin-bottom: 10px;">
                              <b-tag rounded class="funtag" style="position: absolute; top: 0;margin-left:55px"><b>fraud detection</b></b-tag>
                              <b-tag rounded class="funtag" style="position: absolute; top: 0;margin-left:55px"><b>machine learning</b></b-tag>
                              <b-tag rounded class="funtag" style="position: absolute; top: 0;margin-left:55px"><b>machine learning</b></b-tag>

                              <!-- <b-tag rounded class="funtag" style="position: absolute; top: 0; margin-left:65px;"><b>python</b></b-tag> -->
                            </div>
                          </div>
                        </div>
                      </div>
                    </div>
                  </div>
                </div>
          </div>


                  <div class="columns is-vcentered is-centered">
          <div class="column is-5 ">
            <!-- <div class="container"> -->
              <div class="card is-project-card">
                <div class="card-image">
                    <figure class="image is-square is-project-image">
                        <a><img class="is-project-card" src="~/assets/experiences/mhacks.png"></a>
                    </figure>
                </div>
                <div class="card-content">
                    <div class="content">
                        <a class="text_project ml-0">MHacks</a>
                        <p class="is-subtitle">Head of Education:initiative</p>
                        <div class=" is-multi-tag" >
                          <div class="funtag" style="margin-bottom: 10px;">
                            <b-tag rounded class="funtag" style="position: absolute; top: 0; margin-left:-75px"><b>python</b></b-tag>
                            <b-tag rounded class="funtag" style="position: absolute; top: 0; margin-left:-9px"><b>data engineering</b></b-tag>
                            <b-tag rounded class="funtag" style="position: absolute; top: 0; margin-left:120px"><b>machine learning</b></b-tag>
                          </div>
                        </div>
                    </div>
                </div>
              </div>
          </div>
          <div class="column is-5">
              <div class="card is-project-card">
                <div class="card-image">
                    <figure class="image is-square is-project-image">
                        <a><img class="is-project-card" src="~/assets/experiences/oud.png"></a>
                    </figure>
                </div>
                <div class="card-content">
                    <div class="content">
                      <a class="text_project">Office of University Development</a>
                      <p class="is-subtitle">Development Intern</p>
                      <div class="field is-grouped multibutton" >
                          <div class=" is-multi-tag" >
                            <div class="funtag" style="margin-bottom: 10px;">
                              <b-tag rounded class="funtag" style="position: absolute; top: 0;"><b>web app</b></b-tag>
                              <b-tag rounded class="funtag" style="position: absolute; top: 0;margin-left:55px"><b>vue.js</b></b-tag>
                              <!-- <b-tag rounded class="funtag" style="position: absolute; top: 0; margin-left:65px;"><b>python</b></b-tag> -->
                            </div>
                          </div>
                        </div>
                    </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
  </section>
</template>
<script>
export default {
  layout: 'default',
  methods: {
    handleClick() {
      if (this.isImageModalActive === false) {
        this.isImageModalActive = true
        // this.$modal.show('example')
      }
    }
  },
  data () {
    return {
      isImageModalActive: false,
    }
  }
}
</script>
<style scoped lang="scss">
  
  
  .is-project-card { 
    width: 90%;

    /* height: auto; */
  }
  .is-project-card:hover { 
    transform:scale(1.03);
    filter:blur(0px);
    opacity:1;
    box-shadow:0 8px 20px 0px rgba(0,0,0,0.125);
    /* height: auto; */
  }
  .card-image { 
    transform:scale(0.97);
  }
  .is-subtitle { 
    // margin-left: -47%;
    font-size: 18px;
    margin-top: -5px;
  }
.text_project {
  transition: background-size .4s ease;
  background: linear-gradient(to bottom, transparent 62%, #d37766 0) center left/00% 30% no-repeat;
  font-family: 'Helvetica Neue', sans-serif; 
  font-size: 35px; 
  font-weight: bold; 
  letter-spacing: -1px; 
  line-height: 0; 
  text-align: left; 
  width: 200px;
  padding-top: -200px;
  height: 47px;
  color: #28292b;
  cursor: pointer;
    letter-spacing: .1rem;
    // margin-left: -43%;
  &:hover {
    background-size: 100% 100%;
    color: rgba(70, 118, 250, 0.7);
  }
  &:active {
    background-size: 80% 100%;
  }
  &-container {
    z-index: 1;
    color: rgba(110, 151, 255, 0.7);
    position: relative;
    background-color: #fff;
    padding: 0px;
    box-shadow: 0 0 90px 10px rgba(255, 255, 255, 0.15);
  }
}

.is-multi-tag {
  z-index:0;
  position: absolute;
  bottom:2.25rem;
  left:5.45rem;
  // border-radius:100%;
  // width:0rem;
  // height:0rem;
  // transform: translate(-50%, -50%);
  // transition: .25s cubic-bezier(0.25, 0, 0, 1);
  .funtag {
      // z-index: 6;
      display: grid;
      place-items: center;
      position: absolute;
      // background-color:rgb(243, 128, 128);
      // transform: translate(-50%, -50%);
      cursor: pointer;
      transition: .25s cubic-bezier(0.25, 0, 0, 1);
      box-shadow:0 0 0rem -.25rem var(--background);
      &:hover {
          background:var(--text);
          color:var(--background);
          box-shadow:0 0 1rem -.25rem var(--background);
      }
      &:first-child:nth-last-child(1),
      &:first-child:nth-last-child(1) ~ * { //If there is 1 child
          &:nth-child(1) {
              right:25%;
          }
      }
      &:first-child:nth-last-child(2),
      &:first-child:nth-last-child(2) ~ * { //If there are 2 children
          &:nth-child(1) {
              // right:37.5%;
              right:25%;
              // bottom:18.75%;

          }
          &:nth-child(2) {
              // right:1%;
              left:-50px;
          }
      }
      &:first-child:nth-last-child(3),
      &:first-child:nth-last-child(3) ~ * { //If there are 3 children
          &:nth-child(1) {
              left:50%;
          }
          &:nth-child(2) {
              left:25%;
          }
          &:nth-child(3) {
              left:15.625%;
          }
      }
      &:first-child:nth-last-child(4), //If there are 4 children, if first child is also 4th item from bottom get self, and
      &:first-child:nth-last-child(4) ~ * { //If there are 4 children, if first child is also 4th item from bottom get siblings
          &:nth-child(1) {
              left:62.5%;
              bottom:18.75%;
          }
          &:nth-child(2) {
              left:37.5%;
              bottom:18.75%;
          }
          &:nth-child(3) {
              left:18.75%;
              bottom:37.5%;
          }
          &:nth-child(4) {
              left:18.75%;
              bottom:62.5%;
          }
      }
  }
  }
</style>
