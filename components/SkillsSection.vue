<template>
  <section id="skills" class="skills section">
    <h1 class="section__title">Skills</h1>
    <p class="section__subtitle">My Technologies</p>
    <div class="row inner_skills">
      <div class="col-md-6">
        <div class="skill">
          <div
            class="skill__head collapsed border-bottom"
            data-bs-toggle="collapse"
            href="#frontend"
            role="button"
            aria-expanded="false"
            aria-controls="frontend"
          >
            <h5 class="d-flex align-items-center">
              <i class="uil uil-brackets-curly"></i>
              Frontend Developer
            </h5>
            <i class="uil uil-angle-down"></i>
          </div>
          <div id="frontend" class="collapse multi-collapse show">
            <div class="card card-body">
              <div class="skill__progress">
                <div class="skill__title">
                  <p>HTML</p>
                  <p>99%</p>
                </div>
                <div class="progress">
                  <div
                    class="progress-bar"
                    role="progressbar"
                    style="width: 50%"
                    aria-valuenow="50"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
              </div>
              <div class="skill__progress">
                <div class="skill__title">
                  <p>CSS</p>
                  <p>40%</p>
                </div>
                <div class="progress">
                  <div
                    class="progress-bar"
                    role="progressbar"
                    style="width: 50%"
                    aria-valuenow="40"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="skill">
          <div
            class="skill__head"
            data-bs-toggle="collapse"
            href="#design"
            role="button"
            aria-expanded="false"
            aria-controls="design"
          >
            <h5>
              <i class="uil uil-brackets-curly"></i>
              Designer
            </h5>
            <i class="uil uil-angle-down"></i>
          </div>
          <div id="design" class="collapse multi-collapse">
            <div class="card card-body">
              <div class="skill__progress">
                <div class="skill__title">
                  <p>HTML</p>
                  <p>99%</p>
                </div>
                <div class="progress">
                  <div
                    class="progress-bar"
                    role="progressbar"
                    style="width: 50%"
                    aria-valuenow="50"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
              </div>
              <div class="skill__progress">
                <div class="skill__title">
                  <p>CSS</p>
                  <p>40%</p>
                </div>
                <div class="progress">
                  <div
                    class="progress-bar"
                    role="progressbar"
                    style="width: 50%"
                    aria-valuenow="40"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6">
        <div class="skill">
          <div
            class="skill__head"
            data-bs-toggle="collapse"
            href="#backend"
            role="button"
            aria-expanded="false"
            aria-controls="backend"
          >
            <h5>
              <i class="uil uil-brackets-curly"></i>
              Backend Developer
            </h5>
            <i class="uil uil-angle-down"></i>
          </div>
          <div id="backend" class="collapse multi-collapse">
            <div class="card card-body">
              <div class="skill__progress">
                <div class="skill__title">
                  <p>HTML</p>
                  <p>99%</p>
                </div>
                <div class="progress">
                  <div
                    class="progress-bar"
                    role="progressbar"
                    style="width: 50%"
                    aria-valuenow="50"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
                </div>
              </div>
              <div class="skill__progress">
                <div class="skill__title">
                  <p>CSS</p>
                  <p>40%</p>
                </div>
                <div class="progress">
                  <div
                    class="progress-bar"
                    role="progressbar"
                    style="width: 50%"
                    aria-valuenow="40"
                    aria-valuemin="0"
                    aria-valuemax="100"
                  ></div>
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
    name: 'SkillsSection'
  }
</script>
