<script>

import { html,js,css,git,github,express,mysql,mongodb,svelte,nodejs,linkedin,logo,expresssql,todoapp,fakerapi } from "./index";

/*
hamburger = document.querySelector(".hamburger");

hamburger.onclick = function () {
  navBar = document.querySelector(".nav-bar");
  navBar.classList.toggle("active");
}; */
</script>




<header>
  <div class="logo">
    <li>
      <a href="/"><i class="fa-solid fa-code fa-2xl"></i></a>
    </li>
  </div>
  <div class="hamburger">
    <div class="line"></div>
    <div class="line"></div>
    <div class="line"></div>
  </div>
  <nav class="nav-bar">
    <ul>
      <li>
        <a href="#skills"
          ><i class="fa-solid fa-screwdriver-wrench"></i>Skills</a
        >
      </li>
      <li>
        <a href="#projects"><i class="fa-solid fa-folder"></i>Projects</a>
      </li>
      <li>
        <a href="#contact"><i class="fa-solid fa-phone"></i>Contact</a>
      </li>
      <li>
        <a
          href="https://drive.google.com/file/d/1r8mG7AgbCDnnOslviGsZhw3B2yGPUGzv/view?usp=sharing"
          target="_blank"
          ><i class="fa-regular fa-file-lines"></i>Resume</a
        >
      </li>
    </ul>
  </nav>
</header>

<div class="main-container">
  <div id="intro">
    <h1>Hi there!</h1>
    <p>
      As a seasoned full-stack developer, I bring a wealth of expertise in Svelte, HTML, CSS, and JavaScript, coupled with proficiency in database management using MySQL and MongoDB. My robust skill set extends to server-side technologies, encompassing Node.js and Express. With a keen eye for front-end design and a mastery of back-end frameworks, I am adept at crafting seamless and dynamic web applications. My commitment to delivering high-quality solutions is underscored by a proven track record in creating engaging user experiences and optimizing database performance. I am enthusiastic about contributing my multifaceted skills to elevate your development team and drive innovative projects forward.
    </p>
  </div>
  <div id="skills">
    <h1 class="div-title">Skills:</h1>
    <img src={svelte} alt="svelte">
    <img src={html} alt="html" />
    <img src={css} alt="css" />
    <img src={js} alt="javascript" />
    <img src={nodejs} alt="nodejs" />
    <img src={mysql} alt="mysql" />
    <img src={mongodb} alt="mongodb" />
  </div>

  <h1 class="div-title">Projects:</h1>

  <div class="projects" id="projects">
    <div class="card">
      <img src={todoapp} alt="" srcset="" />
      <a href="https://todoapp-375619.ue.r.appspot.com/"
        ><h3>Todo App</h3></a
      >
      <p>
        A todo app built using express,mongodb and deployed on Google's App
        Engine
      </p>
    </div>

    <div class="card">
      <img src={expresssql} alt="" srcset="" />
      <a href="https://github.com/Newtonkamau14/Express-Sql"
        ><h3>Express Sql</h3></a
      >
      <p>A CRUD app using express and MySQL.</p>
    </div>

    <div class="card">
      <img src={fakerapi} alt="" srcset="" />
      <a href="https://github.com/Newtonkamau14/Fakerapi"
        ><h3>Faker Api</h3></a
      >
      <p>Using express to make HTTPS requests to an external api.</p>
    </div>
  </div>

  <h1 class="div-title">Contact Me:</h1>

  <div id="contact">
    <a href="https://github.com/Newtonkamau14"
      ><img src={github} alt=""
    /></a>
    <a href="https://www.linkedin.com/"><img src={linkedin} alt="" /></a>
  </div>

  <span><h3 class="other-contact">Phone No: + 254712603849</h3></span>
  <span><h3 class="other-contact">Email: newtonkamau14@gmail.com</h3></span>

  <footer class="footer">
    <p>Newton &#169; <span>{ new Date().getFullYear()}</span></p>
  </footer>
</div>





<style>

/*Navbar*/
header {
  width: 100%;
  height: 80px;
  background: #0b0a10;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 100px;
}

.logo {
  font-size: 20px;
}

.logo li {
  list-style: none;
}

.logo a {
  color: white;
}
.logo a:hover {
  color: rgb(17, 107, 226);
}

.logo a i {
  transition: transform 0.3ms;
}

.logo a i:hover {
  transform: scale(-1, 1);
}

.hamburger {
  display: none;
}

.nav-bar ul {
  display: flex;
  list-style-type: none;
}

.nav-bar ul li a {
  display: block;
  color: white;
  font-size: large;
  padding: 10px 25px;
  text-align: center;
  text-decoration: none;
  margin: 0 5px;
  transition: transform .3ms;
}

.nav-bar ul li a:hover {
  color: rgb(17, 107, 226);
  transform: scale(1.3);
}

.nav-bar ul li a i {
  margin-right: 5px;
}

@media only screen and (max-width: 1320px) {
  header {
    padding: 0 50px;
  }
}

@media only screen and (max-width: 1100px) {
  header {
    padding: 0 30px;
  }
}

@media only screen and (max-width: 900px) {
  .hamburger {
    display: block;
    cursor: pointer;
  }
  .hamburger .line {
    width: 30px;
    height: 3px;
    background: white;
    margin: 6px 0;
  }
  .nav-bar {
    height: 0px;
    position: absolute;
    top: 80px;
    left: 0;
    right: 0;
    width: 100vw;
    background: #0b0a10;
    overflow: hidden;
  }
  .nav-bar ul {
    display: block;
    width: fit-content;
    text-align: center;
    margin: 60px auto 0 auto;
    background: #0b0a10;
    opacity: 0;
  }

  .nav-bar ul li {
    background: #0b0a10;
  }

  .nav-bar ul li a {
    margin-bottom: 40px;
    background: #0b0a10;
  }

 /*  .nav-bar.active {
    height: 450px;
  }
  .nav-bar.active ul {
    opacity: 1;
  } */
}

/*Main content */
.main-container {
  color: white;
  margin-left: auto;
  margin-right: auto;
  width: 70%;
}

#intro {
  margin-top: 200px;
}
#intro h1 {
  text-align: center;
  font-size: 60px;
}

#intro p {
  font-size: x-large;
  text-align: left;
  line-height: 2;
}

#skills {
  margin-top: 300px;
}

#skills img {
  height: 100px;
  width: 100px;
  margin-left: 60px;
}

.div-title {
  font-family: "Courier New", Courier, monospace;
  font-size: 60px;
  text-align: center;
}

.main-container > .div-title {
  margin-top: 300px;
}

.projects {
  display: flex;
  flex-wrap: wrap;
}

.card {
  background-color: #09091b;
  max-width: 400px;
  padding: 10px;
  border: none;
  border-radius: 10px;
  margin: 10px;
}

.card:hover {
  box-shadow: 0 0 10px rgb(17, 107, 226);
}

.card img {
  background-attachment: fixed;
  background-repeat: no-repeat;
  max-width: 100%;
  border-radius: 5px;
}

.card a {
  color: yellowgreen;
  background-color: #09091b;
  text-decoration: none;
}

.card p {
  color: white;
  background-color: #09091b;
}

#contact {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

#contact a {
  margin-top: 40px;
  margin-left: 60px;
}

#contact a img {
  height: 60px;
  width: 60px;
}

.other-contact {
  margin-top: 10px;
  font-family: "Courier New", Courier, monospace;
  font-weight: lighter;
}

.footer {
  margin-top: 150px;
  border-top: 1px solid grey;
}

.footer p {
  margin: 30px 0;
  text-align: center;
}

.footer p:hover {
  color: rgb(17, 107, 226);
}
</style>