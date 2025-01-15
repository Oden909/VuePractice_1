<template>

  <header>
    <a href="/">
      <img :src="image" alt="Logo"/>
    </a>
    <nav>
      <a href="/">About</a>
      <a href="/">Work</a>
      <a href="/">Contact</a>
    </nav>
  </header>

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

  </main>


  <footer>
    <h2>Lets work together</h2>
    <div class="footer_container">
      <div class="footer_left">
        <p>
          This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com 
          This is a template Figma file, turned into code using Anima. Learn more at AnimaApp.com
        </p>
        <ul>
          <li>
            <a href="">
              <img src="./assets/contactLogos/discord.png" alt="ContactLogo">
            </a>
          </li>
          <li>
            <a href="">
              <img src="./assets/contactLogos/facebook.png" alt="ContactLogo">
            </a>
          </li>
          <li>
            <a href="">
              <img src="./assets/contactLogos/dribbble.png" alt="ContactLogo">
            </a>
          </li>
          <li>
            <a href="">
              <img src="./assets/contactLogos/nstagram.png" alt="ContactLogo">
            </a>
          </li>
          <li>
            <a href="">
              <img src="./assets/contactLogos/behance.png" alt="ContactLogo">
            </a>
          </li>
        </ul>
      </div>
      <div class="footer_right">
        <form>
          <div class="form-group">
            <input type="text" placeholder="Name"/>
          </div>
          <div class="form-group">
            <input type="email" placeholder="Email"/>
          </div>
          <button type="submit" class="submit-button">Submit</button>
        </form>
      </div>
    </div>
  </footer>

</template>

<script>
  import image from "./assets/Logo.png"

  export default {
    data: function () {
      return {
        image: image
      }
    }
  }
</script>

<style scoped>

  header {
    display: flex;
    justify-content: space-between;
    padding: 40px;
    margin-bottom: 40px;
  }

  nav {
    display: flex;
    gap: 20px;
  }

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

  footer {
    padding: 80px 20px;
  }

  .footer_container {
    display: flex;
    justify-content: space-between;
  }

  .footer_left {
    max-width: 570px;
  }

  .footer_left p {
    font-size: 17px;
    font-weight: 400;
    line-height: 27px;
    margin-bottom: 40px;
  }

  .footer_left ul {
    display: flex;
    gap: 10px;
    padding: 0;
  }

  .form-group {
    margin-bottom: 15px;
  }

  input {
    width: 520px;
    padding: 20px;
    font-size: 16px;
    border: none;
    background-color: #f4f4f4;
  }

  input::placeholder {
    color: #2D2D2D;
    font-size: 17px;
    font-weight: 400;
  }

  input:focus {
    outline: none;
    border: 1px solid #3D3D3D;
  }

  .submit-button {
    padding: 30px 60px;
    background-color: #2D2D2D;
    color: #FFFFFF;
    border: none;
    font-size: 20px;
    cursor: pointer;
  }

  .submit-button:hover {
    background-color: #3D3D3D;
  }
</style>
