# TXON-task-4
task4.HTML

<!DOCTYPE html> 
<html lang="en" dir="ltr">
  <head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="Style5.css">
    <!-- Fontawesome CDN Link -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
   </head>
<body>
  <!-- navigation menu -->
  <nav>
    <div class="navbar">
      <div class="logo"><i class="fa fa-paypal"></i>Portfolio</div>
      <ul class="menu">
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#skills">Skills</a></li>
        <li><a href="#contact">Contact</a></li>
        <div class="cancel-btn">
          <i class="fas fa-times"></i>
        </div>
      </ul>
    </div>
    <div class="menu-btn">
      <i class="fas fa-bars"></i>
    </div>
  </nav>

  <!-- Home Section Start -->
  <section class="home" id="home">
    <div class="home-content">
      <div class="text">
        <div class="text-one">Hello,</div>
        <div class="text-two">I'm G.Prashanthi</div>
        <div class="text-three">I'm a passionate  fresher with keen interest in web development and currently looking for an organisation  which will provide me an opputunity to excel and improve myself in the path of IT career.</div>
        <div class="text-four">From KURNOOL</div>
      </div>
      <div class="button">
        <button>More Details</button>
      </div>
    </div>
  </section>

  <!-- About Section Start -->
  <section class="about" id="about">
    <div class="content">
      <div class="title"><span>About Me</span></div>
      <div class="text-four">
      I'm currently persuing 3rd BTech in the stream of Computer Science and Engineering in Ravindra College of Engineering For Women at Kurnool.<br>
      </br>
      I quickly learn and evolve things and give my best in the given task.<br></br>
      I'm a confident about doing of exciting things.<br></br>
      I'm a quick learner and I'm very much interested and excited to explore myself in IT field.</div>
    </div>
      
  </section>
          

  <!-- My Skill Section Start -->
  <section class="skills" id="skills">
    <div class="content">
      <div class="title"><span>My Skills</span></div>
      <div class="skills-details">
        <div class="text">
          <div class="topic"></div>
        <div class="boxes">
          <div class="box">
            <div class="topic">JAVA PROGRAMMING</div>
            <h1 align="justify"><font size="5px" color="black" face="arial,verdana,sans-serif">Java is the most comfortable language  which made me confident to code.It is very interesting and easy to understand which futher helped to learn other languages in a simplified manner.</font></h1>
            <br></br>
            <h2><font size="5px" color="darksalmon" face="arial,verdana,sans-serif">CERTIFICATIONS RELATED TO JAVA PROGRAMMING</font></h2>
            <h3><font size="5px" color="black" face="arial,verdana,sans-serif">*Java for Data Science</font></h3>
            <h4><font size="5px" color="black" face="arial,verdana,sans-serif">*Sololearn</font></h4>
            </p><br></br><br></br>
          </div>
          <div class="box">
            <div class="topic">FRONT END WEB DEVELOPMENT</div>
            <h1 align="justify"><font size="5px" color="black" face="arial,verdana,sans-serif">I learnt HTML,CSS,JAVASCRIPT in order to improve  my web development skills</font></h1><br></br><br></br>
            <h2><font size="5px" color="darksalmon" face="arial,verdana,sans-serif">CERTIFICATIONS RELATED TO FRONT END DEVELOPMENT</font></h2>
            <h3><font size="5px" color="black" face="arial,verdana,sans-serif">*Participated in workshop on front end development on the program AIRBAC LABS</font></h3>
            <br></br>
          </div>
          <div class="box">
            <div class="topic">DATA STRUCTURES AND ALGORITHMS</div>
            <h1><font size="5px" color="black" face="arial,verdana,sans-serif">Currently I'm learning data structures and algorithms from the platform of Smart Interviews.It is very interesting and deals with different approaches of solving a problem,finding the optimal solution ,Time Complexitiy,Space Complexity etc.</font></h1><br></br><br></br><br></br><br></br>
          </div>
          <div class="box">
            <div class="topic">MACHINE LEARNING</div>
            <h1 align="justify"><font size="5px" color="black" face="arial,verdana,sans-serif">In Machine Learning I learnt about differnt algorithms used in order to train a machine.</font> </h1><br></br>
            
          </div>

        </div>
      </div>
    </div>
  </section>



  <!-- Contact Me Section Start -->
  <section class="contact" id="contact">
      <div class="title"><span>Contact Me</span></div>
      <div class="text">
        <p>NAME : G.Prashanthi<br></br>
            PHONE : 5347122780<br></br>
            EMAIL : prashu34560@gmail.com<br></br>
            LOCATION : Kurnool,Andhra Pradesh</p>
          
        <div class="button">
          <button>Download CV</button>
        </div>
      </div>
  </section>

   

  <script src="t3.js"></script>
</body>
</html>





JAVA SCRIPT:

// Sticky Navigation Menu Js

let nav = document.querySelector("nav");
let scrollBtn = document.querySelector(".scroll-button a");

let val;

window.onscroll = function() {
  if(document.documentElement.scrollTop > 20){
    nav.classList.add("sticky");
    scrollBtn.style.display = "block";
  }else{
    nav.classList.remove("sticky");
    scrollBtn.style.display = "none";
  }
}

// Side Navigation Menu Js
let body = document.querySelector("body");
let navBar = document.querySelector(".navbar");
let menuBtn = document.querySelector(".menu-btn");
let cancelBtn = document.querySelector(".cancel-btn");

menuBtn.onclick = function() {
  navBar.classList.add("active");
  menuBtn.style.opacity = "0";
  menuBtn.style.pointerEvents = "none";
  body.style.overflowX = "hidden";
  scrollBtn.style.pointerEvents = "none";
}

cancelBtn.onclick = function() {
  navBar.classList.remove("active");
  menuBtn.style.opacity = "1";
  menuBtn.style.pointerEvents = "auto";
  body.style.overflowX = "auto";
  scrollBtn.style.pointerEvents = "auto";
}

// Side Navigation Bar Close While We click On Navigation Links

let navLinks = document.querySelectorAll(".menu li a");
for (var i = 0; i < navLinks.length; i++) {
  navLinks[i].addEventListener("click" , function() {
    navBar.classList.remove("active");
    menuBtn.style.opacity = "1";
    menuBtn.style.pointerEvents = "auto";
  });
}



Style.CSS:

@import url('https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700&family=Ubuntu:wght@400;500;700&display=swap');
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  text-decoration: none;
  scroll-behavior: smooth;
}
:root{
    --primary-color:#e091f2;
    --black-color:#000000;
    --white-color:#fff;

}
body{
  font-family: 'Ubuntu', sans-serif;
}
/* Custom Scroll Bar CSS */


/* navbar styling */
nav{
  position:fixed;
  width:100%;
  padding:20px 0;
  z-index: 999;
  transition: all 0.3s ease;
}
nav.sticky{
  background:var(--primary-color);
  padding:13px 0;
}
nav .navbar{
  width:90%;
  display:flex;
  justify-content: space-between;
  align-items: center;
  margin:auto;
}
.logo{
    color:darkblue;
    font-size:40px;
    font-family:italic;
    float:left;
    padding-top:.6%;
    cursor:pointer;
}

nav .navbar .logo a{
  font-weight: 600;
  font-size: 50px;
  color:var(--primary-color);
}

nav.sticky .navbar .logo a{
  color:var(--white-color);
}

nav .navbar .menu{
  display:flex;
  position:relative;
}
nav .navbar .menu li{
  list-style: none;
  margin:0 40px;
  
}
nav .navbar .menu a{
  font-size: 25px;
  font-style: italic;
  font-weight: 500;
  color:var(--black-color);
  padding:6px 0;
  transition: all 0.4s ease;
}
.navbar .menu a:hover{
  color:var(--primary-color);
}
nav.sticky .menu a{
  color:var(--white-color);
}
nav.sticky .menu a:hover{
  color:var(--black-color);
}


/* side navigation Menu Button CSS */
nav .menu-btn,
.navbar .menu .cancel-btn{
  position:absolute;
  color:var(--white-color);
  right:30px;
  top:20px;
  font-size: 20px;
  cursor: pointer;
  transition: all 0.3s ease;
  display: none;
}
nav .menu-btn{
  color:var(--primary-color);
}
nav.sticky .menu-btn{
  color:var(--white-color);
}
.navbar .menu .menu-btn{
  color:var(--black-color);
}

/* home section styling */
.home{
  height:100vh;
  width:100%;
  background-size: cover;
  background-position: center center;
  background-attachment: fixed;
}
.home .home-content{
  width:90%;
  height:100%;
  margin:auto;
  display:flex;
  flex-direction: column;
  justify-content: center;
}
.home .text-one{
  font-size:25px;
  color:var(--black-color);
}
.home .text-two{
  color:var(--black-color);
  font-size: 60px;
  font-weight: 600;
  margin-left: -3px;
}
.home .text-three{
  font-size: 30px;
  margin:5px 0;
  color:lightslategrey;
  justify-content: end;
}
.home .text-four{
  font-size: 30px;
  margin:5px 0;
  color:var(--black-color);
}
.home .button{
  margin:14px 0;
}
.home .button button{
  outline:none;
  padding:8px 16px;
  border-radius: 6px;
  font-size: 25px;
  font-weight: 400;
  background:var(--primary-color);
  color:var(--white-color);
  cursor:pointer;
  border:2px solid transparent;
  transition: all 0.4s ease;
}
.home .button button:hover{
  border-color:var(--primary-color);
  background-color: var(--white-color);
  color:var(--primary-color);
}

/* About Section Styling */


section .title{
  display:flex;
  justify-content: center;

}
section .title span{
  color:var(--primary-color);
  font-size: 40px;
  font-weight: 600;
  position:relative;
  padding-bottom:100px;
  padding-top:30px;
}
.about{
  background:#faedfb;
}

.about{
  height:100vh;
  width:100%;
  background-size: cover;
  background-position: center center;
  background-attachment: fixed;
}
.about .content{
  width:90%;
  height:100%;
  margin:auto;
  display:flex;
  flex-direction: column;
  justify-content: center;
}
.about .text-four{
  font-size: 27px;
  margin:5px 0;
  color:rgb(39, 16, 30);
  justify-content: end;
}

section .button{
  margin:16px 0;
}
section .button button{
  outline:none;
  padding:8px 16px;
  border-radius: 4px;
  font-size: 25px;
  font-weight: 400;
  background: var(--primary-color);
  color:var(--white-color);
  border:2px solid transparent;
  cursor: pointer;
  transition: all 0.4s ease;
}
section .button button:hover{
  border-color:var(--primary-color);
  background-color: var(--white-color);
  color:var(--primary-color);
}

/* My Skills CSS */
.skills{
  background:#ADDFFF;
}
.skills .content{
  padding:60px 0;
}
.skills .skills-details{
  display:flex;
  justify-content: space-between;
  align-items: center;
}
.skills-details .text{
  width:95%;
}
.skills-details .boxes{
  width:105%;
  display:flex;
  flex-wrap: wrap;
  justify-content:space-between;
}
.skills-details .box{
  width:calc(100% / 2 - 20px);
  margin:20px 0;
}
.skills-details .boxes .topic{
  font-size: 40px;
  color:darkmagenta;
  font-weight: 550;
  position:relative;
}

/* Contact Me CSS */
.contact{
    background: #93FFE8;
  }
.contact .content{
    margin:0 auto;
    padding:30px 0;
  }
.contact .text{
    width:80%;
    text-align: center;
    margin:auto;
    color:rgb(49, 9, 16);
    font-size:30px;
    font-weight:200;
    font-style:serif;
}
