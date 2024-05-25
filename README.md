# Portfolio
<!doctype html>
<html lang="en">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <title>Personal Portfolio Website</title>
    <link rel="stylesheet" href="style.css">
    <script src="https://kit.fontawesome.com/73eeb7bbf1.js" crossorigin="anonymous"></script>
    <style>
      *{
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
    box-sizing: border-box;
}
html{
    scroll-behavior: smooth;
}
body{
    background: #080808;
    color: #fff;
}
#header{
    width: 100%;
    height: 100vh;
    background-image: url(https://scontent.fmnl25-5.fna.fbcdn.net/v/t1.15752-9/438203898_1127994608247808_7482794543686424435_n.png?_nc_cat=104&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFStWEKKb1SBYQQkAfo61A4NsuSdru64fA2y5J2u7rh8KhQWJWOLo7vkbNpaU9PwsDBrwHYJSmnmb7sHkrr72Je&_nc_ohc=8XxxstgzsncQ7kNvgE_aNPy&_nc_ht=scontent.fmnl25-5.fna&oh=03_Q7cD1QGpWJGHQ2o56biSc54DL4rZt-Kq_-8ore9G7dI2cUsq3Q&oe=66772A2B);
    background-size: cover;
    background-position: right;
}
.container{
        padding: 10px 10%;
}

nav{
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
}

.logo{
    width: 200px;
}

nav ul li{
    display: inline-block;
    list-style: none;
    margin: 10px 20px;
}

nav ul li a{
    color: #fff;
    text-decoration: none;
    font-size: 18px;
    position: relative;
}
nav ul li a::after{
    content: '';
    width: 0;
    height: 3px;
    background: #ff004f;
    position: absolute;
    left: 0;
    bottom: -6px;
    transition: 0.5s;
}
nav ul li a:hover::after{
    width: 100%;
}
.header-text{
    margin-top: 20%;
    font-size: 30px;
}
.header-text h1{
    font-size: 60px;
    margin-top: 20px;
}
.header-text h1 span{
    color: #ff004f;
}
/* ---------about----------- */
#about{
    padding: 80px 0;
    color: #ababab;
}
.row{
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.about-col-1{
    flex-basis: 35%;
}
.about-col-1 img{
    width: 100%;
    border-radius: 15px;
}
.about-col-2{
    flex-basis: 60%;
}

.sub-title{
    font-size: 60px;
    font-weight: 600;
    color: #fff;
}

.tab-titles{
    display: flex;
    margin: 20px 0 40px;
}
.tab-links{
    margin-right: 50px;
    font-size: 18px;
    font-weight: 500;
    cursor: pointer;
    position: relative;
}
.tab-links::after{
    content: '';
    width: 0;
    height: 3px;
    background: #ff004f;
    position: absolute;
    left: 0;
    bottom: -8px;
    transition: 0.5s;
}

.tab-links.active-link::after{
    width: 50%;
}

.tab-contents ul li{
    list-style: none;
    margin: 10px 0;
}
.tab-contents ul li span{
    color: #b54769;
    font-size: 14px;
}
.tab-contents{
    display: none;
}.tab-contents.active-tab{
    display: block;
}

/*--------------services---------------*/
#services{
    padding: 30px 0;
}
.services-list{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 40px;
    margin-top: 50px;
}
.services-list div{
    background: #262626;
    padding: 40px;
    font-size: 13px;
    font-weight: 300;
    border-radius:  10px;
    transition: background 0.5s, transform 0.5s;
}
.services-list div i{
    font-size: 50px;
    margin-bottom: 30px;
}
.services-list div h2{
    font-size: 30px;
    font-weight: 500;
    margin-top: 15px;
}
.services-list div a{
    text-decoration: none;
    color: #fff;
    font-size: 12px;
    margin-top: 20px;
    display: inline-block;
}
.services-list div:hover{
    background: #ff004f;
    transform: translate(-10);
}
/*-----------portfolio-----------*/
#portfolio{
    padding: 50px 0;
}
.work-list{
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 40px;
    margin-top: 50px;
}
.work{
    border-radius: 10px;
    position: relative;
    overflow: hidden;
}
.work img{
    width: 100%;
    border-radius: 10px;
    display: block;
    transition: transform 0.5s;
}
.layer{
    width: 100%;
    height: 0;
    background: linear-gradient(rgba(0,0,0,0.6), #ff004f);
    border-radius: 10px;
    position: absolute;
    left: 0;
    bottom: 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    padding: 0 40px;
    text-align: center;
    font-size: 14px;
    transition: height 0.5s;
}
.layer h3{
    font-weight: 500;
    margin-bottom: 20px;
}
.layer a{
    margin-top: 20px;
    color: #ff004f;
    text-decoration: none;
    font-size: 18px;
    line-height: 60px;
    background: #fff;
    width: 60px;
    height: 60px;
    border-radius: 50%;
    text-align: center;
}
.work:hover img{
    transform: scale(1.1);
}
.work:hover .layer{
    height: 100%;
}
.btn{
    display: block;
    margin: 50px auto;
    width: fit-content;
    border: 1px solid #ff004f;
    padding: 14px 50px;
    border-radius: 6px;
    text-decoration: none;
    color: #fff;
    transition: background 0.5s;
}
.btn:hover{
    background: #ff004f;
}

/*-------------contact-----------*/
.contact-left{
    flex-basis: 35%;
}    
.contact-right{
    flex-basis: 60%;    
}
.contact-left p{
    margin-top: 30px;
}
.contact-left p i{
    color: #ff004f;
    margin-right: 15px;
    font-size: 25px;
}
.social-icons{
    margin-top: 30px;
}
.social-icons a{
    text-decoration: none;
    font-size: 30px;
    margin-right: 15px;
    color: #ababab;
    display: inline-block;
    transition: transform 0.5s;
}
.social-icons a:hover{
    color: #ff004f;
    transform: translateY(-5px);
}
.btn.btn2{
    display: inline-block;
    background: #ff004f;
}
.contact-right form{
    width: 100%;
}
form input, form textarea{
    width: 100%;
    border: 0;
    outline: none;
    background: #262626;
    padding: 15px;
    margin: 15px 0;
    color: #fff;
    font-size: 18px;
    border-radius: 6px;
}
form btn2{
    padding: 14px 60px;
    font-size: 18px;
    margin-top: 20px;
    cursor: pointer;
}
.copyright{
    width: 100%;
    text-align: center;
    padding: 25px 0;
    background: #262626;
    font-weight: 300;
    margin-top: 20px;
}
.copyright i{
    color: #ff004f;
}
/*--------------css for small screens-----------*/
nav .fa-solid{
    display: none;
}

@media only screen and (max-width: 600px){
    #header{
        background-image: url(https://scontent.fmnl25-5.fna.fbcdn.net/v/t1.15752-9/438203898_1127994608247808_7482794543686424435_n.png?_nc_cat=104&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeFStWEKKb1SBYQQkAfo61A4NsuSdru64fA2y5J2u7rh8KhQWJWOLo7vkbNpaU9PwsDBrwHYJSmnmb7sHkrr72Je&_nc_ohc=8XxxstgzsncQ7kNvgE_aNPy&_nc_ht=scontent.fmnl25-5.fna&oh=03_Q7cD1QGpWJGHQ2o56biSc54DL4rZt-Kq_-8ore9G7dI2cUsq3Q&oe=66772A2B);
        background-size: cover;
        background-position: right;
    }
    .header-text{
        margin-top: 100%;
        font-size: 16px;
    }
    .header-text h1{
        font-size: 30px;
    }
    nav .fa-solid{
        display: block;
        font-size: 25px;
    }
    nav ul{
        background: #ff004f;
        position: fixed;
        top: 0;
        right: -200px;
        width: 200px;
        height: 100vh;
        padding-top: 50px;
        z-index: 2;
        transition: right 0.5s;
    }
    nav ul li{
        display: block;
        margin: 25px;
    }
    nav ul .fa-solid{
        position: absolute;
        top: 25px;
        left: 25px;
        cursor: pointer;
    }
    .sub-title{
        font-size: 40px;
    }
    .about-col-1, .about-col-2{
        flex-basis: 100%;
    }
    .about-col-1{
        margin-bottom: 30px;
    }
    .about-col-2{
        font-size: 14px;
    }
    .tab-links{
        font-size: 16px;
        margin-right: 20px;
    }
    .contact-left, .contact-right{
        flex-basis: 100%;
    }
    .copyright{
        font-size: 14px;
    }
}
    </style>
  </head>
  <body>
  <div id="header">
    <div class="container">
      <nav>
        <img src="https://scontent.fmnl25-4.fna.fbcdn.net/v/t1.15752-9/438245665_1089124615655456_6619434263659645117_n.png?_nc_cat=109&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEOZAF8aC8fRLAB37uTji3MnB-dTqkZ2E-cH51OqRnYT88JiZESZOmJ-AJVCgCZ7G_tth6AhJbBAbef6yUBteVD&_nc_ohc=LCnAfUTybQ4Q7kNvgGtbsYY&_nc_ht=scontent.fmnl25-4.fna&oh=03_Q7cD1QEnxmeNcN1U9xeauW_mYfDSBiHfbUK8wJtNtpfuIuua0g&oe=667753DE" class="logo">
        <ul id="sidemenu">
          <li><a href="#header">Home</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#portfolio">Portfolio</a></li>
          <li><a href="#contact">Contact</a></li>
          <i class="fa-solid fa-xmark" onclick="closemenu()"></i>
        </ul>
        <i class="fa-solid fa-bars" onclick="openmenu()"></i>
      </nav>
      <div class="header-text">
        <p>Student</p>
        <h1>Hi, I'm <span>Elezar</span><br>Jay From Cavite</h1>
      </div>
    </div>
  </div>
  <!-----------about----------->
  <div id="about">
    <div class="container">
      <div class="row">
        <div class="about-col-1">
          <img src="https://scontent.fmnl25-1.fna.fbcdn.net/v/t1.15752-9/436818011_1170782510601007_2597545816537084194_n.jpg?_nc_cat=108&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEqNPY8t6dbX2RWVXtvX5mc2F-fjY4rfkrYX5-Njit-Snpgi5MGNSwqZVACxQJizj_TZGPc3kjunT2KbVJZdMXt&_nc_ohc=Y_si5WjWEYAQ7kNvgGOYYiG&_nc_ht=scontent.fmnl25-1.fna&oh=03_Q7cD1QEhpTCA3rd4ck1CYWa4ybcYquIvDz-jMFi7fWSxEkgEqQ&oe=667741CB">
        </div>
        <div class="about-col-2">
          <h1 class="sub-title">About Me</h1>
          <p>Hi, I'm Elezar Jay, a diligent Computer Science student who is crafting my own path towards a bright future. With a passion for technology and a determination to succeed, i'm not just studying for degree, but actively shaping my own destiny in the world of computer science. Through hard work, dedication, and a hunger for knowledge, i'm paving the way for my own success in the exciting realms of technology and innovation.</p>

          <div class="tab-titles">
            <p class="tab-links active-link" onclick="opentab('skills')">Skills</p>
            <p class="tab-links" onclick="opentab('experience')">Experience</p>
            <p class="tab-links" onclick="opentab('education')">Education</p>
          </div>
          <div class="tab-contents active-tab" id="skills">
            <ul>
              <li><span>JavaScript</span><br>Asynchronous Programming<br>Fundamentals</li>
              <li><span>Html</span><br>Accessibility<br>Semantics<br>Forms<br>Multimedia<br>Semantic Markup</li>
              <li><span>Bootstrap</span><br>Responsive Design<br>Component Usage<br>Customization<br>Layouts</li>
            </ul>
          </div>
          <div class="tab-contents" id="experience">
            <ul>
              <li><span>2024 - Current</span><br> I'm currently in the midst of shaping my expertise through practical experience. With a thirst for knowledge and a drive to excel, I'm actively immersing myself in real-world challenges, eagerly seizing every opportunity to grow. As I navigate this journey, I'm not just accumulating experience; I'm refining my skills, broadening my understanding, and crafting a narrative of resilience and proficiency in my chosen field. Join me as I turn aspirations into achievements, one step at a time.</li>
            </ul>
          </div>
          <div class="tab-contents" id="education">
            <ul>
              <li><span>2024 - Current</span><br>Cavite State University - Bacoor Campus</li>
              <li><span>2021-2022</span><br>ABE Intenational Business College</li>
              <li><span>2018-2019</span><br>Bacoor National Highschool - Main</li>
            </ul>
        </div>
      </div>
    </div>
  </div>
</div>
<!---------services--------->
<div id="services">
  <div class="container">
    <h1 class="sub-title">My Services</h1>
    <div class="services-list">
      <div>
        <i class="fa-brands fa-js"></i>
        <h2>JavaScript</h2>
        <p>"Hey there! Need help with JavaScript? I'm here for you. Whether you're stuck on 
          assignments or aiming to level up your coding skills, let's work together. 
          We can schedule virtual sessions where I'll guide you through concepts, assist with 
          projects, and answer any questions you have. Let's tackle JavaScript together!"</p>
          <a href="#">Learn more</a>
      </div>
      <div>
        <i class="fa-solid fa-code"></i>
        <h2>Html</h2>
        <p>"Hey there! Need a hand with HTML? Look no further! Whether you're grappling with web page 
          structure or aiming to refine your HTML skills, I'm here to support you. Let's arrange virtual
           sessions where we can delve into HTML fundamentals, collaborate on projects, and address any 
           questions you have. Together, we'll conquer HTML and build awesome web experiences!"</p>
          <a href="#">Learn more</a>
      </div>
      <div>
        <i class="fa-brands fa-bootstrap"></i>
        <h2>Bootstrap</h2>
        <p>"Hey! Need help with Bootstrap? You're in luck! Whether you're grappling with responsive design or 
          seeking to polish your web development skills, I'm here to assist you. Let's schedule virtual 
          sessions where we can delve into Bootstrap's intricacies, collaborate on projects, and address
           any questions you have. Together, we'll harness the power of Bootstrap to create visually
            stunning and user-friendly websites!"</p>
          <a href="#">Learn more</a>
      </div>
    </div>
  </div>
</div>
<!----------portfolio------------->
<div id="portfolio">
  <div class="container">
    <h1 class="sub-title">My Work</h1>
    <div class="work-list">
      <div class="work">
        <img src="https://scontent.fmnl25-4.fna.fbcdn.net/v/t1.15752-9/438245662_981506313346599_1175393186416064223_n.png?_nc_cat=109&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeGfnvyxnLlJgChdOFI1B2pz5vTEfnOrAd3m9MR-c6sB3d8_FHFoN7wxgjH2q_u92nLZ3ZIZ_E86OAsQMRdMwDTU&_nc_ohc=nHz1z9PNPUYQ7kNvgGhJOR6&_nc_ht=scontent.fmnl25-4.fna&oh=03_Q7cD1QFyLK49A8En0GPajCLzgk2-1Rhjg_GJeYggWE3cUg_FQA&oe=66772AD3">
        <div class="layer">
          <h3>Bootsrap Introduction</h3>
          <p>Responsive columns adjust their layout or behavior based on the screen size or 
            device type to ensure optimal viewing and usability across different devices and 
            screen resolutions.</p>
            <a href="https://zarjay.github.io/ACTIVITY-1-ELEZAR-JAY-/"><i class="fa-solid fa-up-right-from-square"></i></a>
        </div>
      </div>
      <div class="work">
        <img src="https://scontent.fmnl25-1.fna.fbcdn.net/v/t1.15752-9/438237580_302998496228742_681417573879842588_n.png?_nc_cat=103&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEKyjyz1_xam62_d41YYGv6lRYoA4RFHuOVFigDhEUe44A9dKo29wx2qUGMqGB6TMDbkDtQCnSklAsLU72hPomQ&_nc_ohc=q6vxWD6vz-sQ7kNvgGIAqFG&_nc_ht=scontent.fmnl25-1.fna&oh=03_Q7cD1QEptUht2UdPFNx9UoMwwDqUN2Xq97klCjeJKk9tj7IIRQ&oe=667743B7">
        <div class="layer">
          <h3>Responsive Column</h3>
          <p>Responsive columns adjust their layout or behavior based on the screen size or 
            device type to ensure optimal viewing and usability across different devices and 
            screen resolutions.</p>
            <a href="https://zarjay.github.io/ACTIVITY-2-ELEZAR-JAY/"><i class="fa-solid fa-up-right-from-square"></i></a>
        </div>
      </div>
      <div class="work">
        <img src="https://scontent.fmnl25-1.fna.fbcdn.net/v/t1.15752-9/438231387_944162427170287_1817891014560261737_n.png?_nc_cat=108&ccb=1-7&_nc_sid=5f2048&_nc_eui2=AeEg7_hA-O9iEhUjFa0W7zHnv5zrFSZpsTy_nOsVJmmxPJLkmyqouKXVP4dBC_2VrQsILv8RzE2_75vk5DXveHa8&_nc_ohc=sTY3fSZj9pwQ7kNvgHBMYjt&_nc_ht=scontent.fmnl25-1.fna&oh=03_Q7cD1QG2QFq_EQVlu_QRQpMJpdfv3UFcEC1zypCOcCJASJwUug&oe=66773FC4">
        <div class="layer">
          <h3>Responsive column with image</h3>
          <p>Responsive columns adjust their layout or behavior based on the screen size or 
            device type to ensure optimal viewing and usability across different devices and 
            screen resolutions.</p>
            <a href="https://zarjay.github.io/activity-3-elezar-jay-rodelas/"><i class="fa-solid fa-up-right-from-square"></i></a>
        </div>
      </div>
    </div>
    <a href="#" class="btn">See More</a>
  </div>
</div>
<!-----------contact----------->
<div id="contact">
  <div class="container">
    <div class="row">
      <div class="contact-left">
        <h1 class="sub-title">Contact Me</h1>
        <p><i class="fa-solid fa-paper-plane"></i> zarjay29@gmail.com</p>
        <p><i class="fa-solid fa-square-phone-flip"></i> 09773411219</p>
        <div class="social-icons">
          <a href="https://www.facebook.com/zarjay.rodelas"><i class="fa-brands fa-facebook"></i></a>
          <a href=""><i class="fa-brands fa-twitter-square"></i></a>
          <a href="https://www.instagram.com/elezarjayrodelas/?hl=en"><i class="fa-brands fa-instagram"></i></a>
          <a href=""><i class="fa-brands fa-linkedin"></i></a>
        </div>
      </div>
      <div class="contact-right">
        <form action="https://api.web3forms.com/submit" method="POST">

          <form action="https://api.web3forms.com/submit" method="POST">
          <input type="hidden" name="apikey" value="af1350e7-1124-4f2e-8668-245d949c44aa">
          <input type="text" name="Name" placeholder="Your Name" required>
          <input type="email" name="Email" placeholder="Your Email" required>
          <textarea name="Message" rows="6" placeholder="Your Message"></textarea>
          <button type="submit" class="btn btn2">Submit</button>
        </form>
      </div>
    </div>
  </div>
  <div class="copyright">
    <p>Copyright © Elezar. Made with <i class="fa-solid fa-heart"></i> by Myself.</p>
  </div>
</div>

<script>

  var tablinks = document.getElementsByClassName("tab-links");
  var tabcontents = document.getElementsByClassName("tab-contents");
  function opentab(tabname){
    for(tablink of tablinks){
      tablink.classList.remove("active-link");
    }
    for(tabcontent of tabcontents){
      tabcontent.classList.remove("active-tab");
    }
    event.currentTarget.classList.add("active-link");
    document.getElementById(tabname).classList.add("active-tab");
  }

</script>

<script>

  var sidemenu = document.getElementById("sidemenu");

  function openmenu(){
    sidemenu.style.right = "0"
  }
  function closemenu(){
    sidemenu.style.right = "-200px"
  }

</script>
  
</body>
</html>
