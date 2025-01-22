<template>
  <Header></Header>
  <main>
    <div class="banner_container">
      <div class="banner_left">
        <h3>Branding | Image making</h3>
        <h1>Visual Designer</h1>
        <p>
          This is a template Figma file, turned into code using Anima. <br>
          Learn more at AnimaApp.com
        </p>
        <a href="/">
          <button>Contact</button>
        </a>
      </div>
      <div class="banner_right">
        <img src="./assets/HeaderImage.png" alt="BannerLogo">
      </div>
    </div>

    <div class="brands_container">
      <ul>
        <li>
          <img src="./assets/brandLogos/googleLogo.png" alt="BrandLogo">
        </li>
        <li>
          <img src="./assets/brandLogos/nikeLogo.png" alt="BrandLogo">
        </li>
        <li>
          <img src="./assets/brandLogos/samsungLogo.png" alt="BrandLogo">
        </li>
        <li>
          <img src="./assets/brandLogos/appleLogo.png" alt="BrandLogo">
        </li>
        <li>
          <img src="./assets/brandLogos/adidasLogo.png" alt="BrandLogo">
        </li>
      </ul>
    </div>

    <section class="skills_section">
      <div class="skills_container">
        <div v-for="(skill, ind) in skills" :key="ind">
          <img :src="skill.imgSrc" alt="skillImg"/>
          <h3>{{ skill.title }}</h3>
          <p>{{ skill.text }}</p>
        </div>
      </div>
    </section>

    <section class="works_section">
      <h2>Latest work</h2>
      <ul class="works_container">
        <li v-for="(work, ind) in works" :key="ind">
          <img :src="work.imgSrc" alt="workImg"/>
          <h3>{{ work.title }}</h3>
          <p>{{ work.text }}</p>
        </li>
      </ul>
    </section>

    <section class="reviews_section">
      <h2>Testimonial</h2>
      <div class="reviews_container">
        <div class="review_card" v-for="(review, ind) in reviews" :key="ind">
          <p class="review_card_text">{{ review.text }}</p>
          <div class="review_user_info">
            <div>
              <img :src="review.imgSrc" alt="userImg"/>
            </div>
            <div>
              <span class="user_rating">★★★★★</span>
              <h4>{{ review.title }}</h4>
              <p class="user_platform_text">Google</p>
            </div>
          </div>

        </div>
      </div>
    </section>
  </main>
  <Footer></Footer>
</template>

<script>
  import image from "./assets/Logo.png"
  import Header from './components/Header.vue'
  import Footer from './components/Footer.vue'

  export default {
    components: {
      Header, Footer
    },
    data: function () {
      return {
        image: image,
        skills: [
          {
            id: 1,
            imgSrc: "./src/assets/skillsLogos/skill1.png",
            title: "Product Design",
            text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com"
          },
          {
            id: 2,
            imgSrc: "./src/assets/skillsLogos/skill2.png",
            title: "Visual Design",
            text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com"
          },
          {
            id: 3,
            imgSrc: "./src/assets/skillsLogos/skill3.png",
            title: "Art Direction",
            text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com"
          }
        ],
        works: [
          {
            id: 1,
            imgSrc: "./src/assets/worksLogos/work1.png",
            title: "Project title",
            text: "UI, Art drection"
          },
          {
            id: 2,
            imgSrc: "./src/assets/worksLogos/work2.png",
            title: "Project title",
            text: "UI, Art drection"
          },
          {
            id: 3,
            imgSrc: "./src/assets/worksLogos/work3.png",
            title: "Project title",
            text: "UI, Art drection"
          },
          {
            id: 4,
            imgSrc: "./src/assets/worksLogos/work4.png",
            title: "Project title",
            text: "UI, Art drection"
          },
          {
            id: 5,
            imgSrc: "./src/assets/worksLogos/work5.png",
            title: "Project title",
            text: "UI, Art drection"
          },
          {
            id: 6,
            imgSrc: "./src/assets/worksLogos/work6.png",
            title: "Project title",
            text: "UI, Art drection"
          },
        ],
        reviews: [
          {
            id: 1,
            imgSrc: "./src/assets/UserLogo.png",
            title: "Gemma Nolen",
            text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com"
          },
          {
            id: 2,
            imgSrc: "./src/assets/UserLogo.png",
            title: "Gemma Nolen",
            text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com"
          },
          {
            id: 3,
            imgSrc: "./src/assets/UserLogo.png",
            title: "Gemma Nolen",
            text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com"
          },
          {
            id: 4,
            imgSrc: "./src/assets/UserLogo.png",
            title: "Gemma Nolen",
            text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com"
          },
          {
            id: 5,
            imgSrc: "./src/assets/UserLogo.png",
            title: "Gemma Nolen",
            text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com"
          },
          {
            id: 6,
            imgSrc: "./src/assets/UserLogo.png",
            title: "Gemma Nolen",
            text: "This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com"
          },
        ]
      }
    }
  }
</script>

<style scoped>

  .banner_container {
    display: flex;
    justify-content: space-between;
    padding: 0 50px;
    margin-bottom: 60px;
  }

  .banner_container p {
    font-size: 17px;
    font-weight: 400;
    line-height: 27px;
    margin: 20px 0 50px 0;
  }  

  .banner_container button {
    padding: 30px 60px;
    background-color: #2D2D2D;
    color: #FFFFFF;
    border: none;
    font-size: 20px;
    cursor: pointer;
  }

  .brands_container {
    padding: 50px;
  }

  .brands_container ul{
    display: flex;
    justify-content: space-between;
  }

  .skills_section {
    padding: 150px 50px;
  }

  .skills_container {
    display: flex;
    justify-content: space-between;
    text-align: center;
  }

  .skills_container div{
    max-width: 395px;
  }
  
  .skills_container p {
    font-size: 17px;
    font-weight: 400;
    line-height: 27px;
    max-width: 310px;
  }

  .skills_container img {
    margin-bottom: 20px;
  }

  .works_section {
    padding: 50px;
  }

  .works_section h2{
    text-align: center;
  }

  .works_container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    padding: 50px 0px;
  }

  .works_container p {
    font-size: 17px;
    font-weight: 400;
    line-height: 27px;
  }

  .reviews_section {
    padding: 50px;
  }

  .reviews_section h2 {
    text-align: center;
  }

  .reviews_container {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 20px;
    padding: 50px 0px;
  }

  .review_card {
    background-color: #F3F3F3;
    padding: 40px;
    max-width: 395px;
  }

  .review_user_info {
    display: flex;
    gap: 10px;
  }

  .review_user_info h4 {
    margin: 10px 0 10px 0;
    font-size: 20px;
    font-weight: 600;
  }

  .user_rating {
    font-size: 25px;
  }

  .user_platform_text {
    margin: 0; 
    font-size: 17px;
    font-weight: 400;
  }

  .review_card_text {
    font-size: 20px;
    font-weight: 600;
    line-height: 30px;
  }

</style>
