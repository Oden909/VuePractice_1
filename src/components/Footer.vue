<template>
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
              <img src="../assets/contactLogos/discord.png" alt="ContactLogo">
            </a>
          </li>
          <li>
            <a href="">
              <img src="../assets/contactLogos/facebook.png" alt="ContactLogo">
            </a>
          </li>
          <li>
            <a href="">
              <img src="../assets/contactLogos/dribbble.png" alt="ContactLogo">
            </a>
          </li>
          <li>
            <a href="">
              <img src="../assets/contactLogos/nstagram.png" alt="ContactLogo">
            </a>
          </li>
          <li>
            <a href="">
              <img src="../assets/contactLogos/behance.png" alt="ContactLogo">
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
    export default {
        
    }
</script>

<style scoped>
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