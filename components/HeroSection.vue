<template>
  <section id="home" class="section home">
    <div class="container">
      <div class="row">
        <div class="col-md-8">
          <div class="row">
            <div class="col-md-12">
              <div class="left">
                <h1 class="hero_h1">Hi, I am Isaac Anane Amankwaah</h1>
                <p class="hero__subtitle">Full Stack Developer</p>
                <p class="hero__text">
                  Recognized for demonstrating strong analytical skills
                  and proven software development skills. Resourceful and
                  well-organized with excellent leadership and
                  team-building record.
                </p>
                <div class="hero_btn my-5 d-flex align-items-center align-center justify-content-between">
                  <button class="btn btn_primary">
                    Contact Me <i class="uil uil-play"></i>
                  </button>
                  <div class="navigations">
                    <ul class="nav_list">
                      <li class="nav__item">
                        <a href="https://www.linkedin.com/in/isaac-anane-amankwaah-02a924130/" target="_blank"><i
                            class="uil uil-linkedin"></i>LinkedIn</a>
                      </li>
                      <li class="nav__item">
                        <a href="https://www.facebook.com/realbrasmith/" target="_blank"><i
                            class="uil uil-facebook"></i>Facebook</a>
                      </li>
                      <li class="nav__item">
                        <a href="https://github.com/brasmith9" target="_blank"><i class="uil uil-github"></i>GitHub</a>
                      </li>
                    </ul>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="col-md-4">
          <div class="cube__wrapper">
            <svg viewBox="0 0 200 187" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
              <mask id="mask0" mask-type="alpha">
                <path
d="M190.312 36.4879C206.582 62.1187 201.309 102.826 182.328 134.186C163.346 165.547 
                        130.807 187.559 100.226 186.353C69.6454 185.297 41.0228 161.023 21.7403 129.362C2.45775 
                        97.8511 -7.48481 59.1033 6.67581 34.5279C20.9871 10.1032 59.7028 -0.149132 97.9666 
                        0.00163737C136.23 0.303176 174.193 10.857 190.312 36.4879Z" />
              </mask>
              <g mask="url(#mask0)">
                <path
d="M190.312 36.4879C206.582 62.1187 201.309 102.826 182.328 134.186C163.346 
                        165.547 130.807 187.559 100.226 186.353C69.6454 185.297 41.0228 161.023 21.7403 
                        129.362C2.45775 97.8511 -7.48481 59.1033 6.67581 34.5279C20.9871 10.1032 59.7028 
                        -0.149132 97.9666 0.00163737C136.23 0.303176 174.193 10.857 190.312 36.4879Z" />
                <image href="" />
              </g>
            </svg>
          </div>
        </div>
        <div class="scroll_btn">
          <button id="scroll_btn" class="btn" @click="handleScroll">
            <i class="uil uil-mouse-alt-2 scroll_icon_1 scroll_icon"></i>
            Scroll down
            <i class="uil uil-arrow-to-bottom scroll_icon"></i>
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'HeroSection',
  setup() {
    const handleScroll = () => {
      window.scrollTo(0, document.body.scrollHeight);
    }
    return {
      handleScroll
    }
  }
}
</script>