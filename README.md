<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio</title>
    <link rel="icon" href="favicon.ico">
   <style>* {
    margin: 0;
    padding: 0;
    font-family: 'Poppins', sans-serif;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    background-color: #080808;
    color: #fffffff7;
}

#header {
    width: 100%;
    height: 100%;
    background-image: url("https://png.pngtree.com/thumb_back/fh260/background/20201104/pngtree-technology-background-binary-computer-code-vector-design-image_458702.jpg");
    background-size: cover;
    background-position: center;
}

.container {
    padding: 10px 10%;
    margin-top: 80px;
}

.logo {
    width: 140px;
}

nav {
    background: #4316646b;
    position: fixed;
    width: 100%;
    top: 0;
    right: 0;
    padding: 15px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    flex-wrap: wrap;
}

nav ul li {
    display: inline;
    list-style: none;
    margin: 10px 20px;
}

nav ul li a {
    text-decoration: none;
    color: #fffe;
    font-weight: 600;
    font-size: 18px;
    position: relative;
}

nav ul li a::after {
    content: '';
    width: 0;
    height: 3px;
    background: dodgerblue;
    position: absolute;
    left: 0;
    bottom: -6px;
    transition: 0.5s;
}

nav ul li a:hover::after {
    width: 100%;
}

.header-text {
    margin-top: 20%;
    font-size: 30px;
}

.header-text h1 {
    font-size: 40px;
    margin-top: 20px;
}

.header-text h1 span {
    color: #fd053f;
    font-size: 60px;
}

/* -----about------ */
#about {
    padding: 80px 0;
    color: #dfdfdf;
}

.row {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}

.about-col-1 {
    flex-basis: 35%;
}

.about-col-1 img {
    background-color: #302e2ef7;
    border-radius: 15px;
    width: 100%;
}

.about-col-2 {
    flex-basis: 60%;
}

.sub-title {
    font-size: 60px;
    font-weight: 600;
    color: #fff
}

.tab-titles {
    display: flex;
    margin: 20px 0 40px;
}

.tab-links {
    margin-right: 50px;
    font-size: 18px;
    font-weight: 500;
    position: relative;
    cursor: pointer;
}

.tab-links::after {
    content: '';
    width: 0;
    height: 5px;
    left: 0;
    bottom: -8px;
    transition: 0.5s;
    position: absolute;
    background: dodgerblue;
}

.tab-links:hover::after {
    width: 100%;
}

.tab-links.active-link::after {
    width: 100%;
}

.tab-contents ul li {
    list-style: none;
    margin: 10px 0;
}

.tab-contents ul li span {
    color: #b54769;
    font-size: 14px;
    font-weight: bold;
}

.tab-contents {
    display: none;
}

.tab-contents.active-tab {
    display: block;
}

/* ----------------------------------Services------------------------------------------- */
#services {
    padding: 30px 0;
}

.services-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 40px;
    margin-top: 50px;
}

.services-list div {
    background: #262626;
    font-size: 13px;
    font-weight: 300;
    padding: 40px;
    border-radius: 10px;
    transition: transform 0.5s;
}

.services-list div i {
    font-size: 50px;
    margin-bottom: 30px;
}

.services-list div h2 {
    font-size: 30px;
    font-weight: 500;
    margin-bottom: 15px;
}

.services-list div a {
    text-decoration: none;
    color: white;
    font-size: 12px;
    margin-top: 20px;
    display: inline-block;
}

.services-list div:hover {
    background-color: dodgerblue;
    transform: translateY(-10px);
}

/* -----------------portfolio----------------------------- */

#portfolio {
    padding: 50px 0;
}

.work-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    grid-gap: 40px;
    margin-top: 50px;
}

.work {

    position: relative;
    overflow: hidden;
    border-radius: 10px;
    transition: transform 0.5s;
}

.work img {
    width: 100%;
    border-radius: 10px;
    display: block;
}

.layer {
    width: 100%;
    background: linear-gradient(rgba(0, 0, 0, 0.6), #1e8fff73);
    height: 0;
    border-radius: 10px;
    position: absolute;
    left: 0;
    bottom: 0;
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    text-align: center;
    padding: 0 40px;
    font-size: 14px;
    transition: height 1s;
}

.layer h3 {
    font-weight: 600;
    margin-bottom: 20px;
}

.layer a {
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

.work:hover img {
    transform: scale(1.1);
}

.work:hover .layer {
    height: 100%;
}

.btn {
    display: block;
    margin: 50px auto;
    border: 1px solid dodgerblue;
    width: fit-content;
    padding: 14px 50px;
    border-radius: 6px;
    color: white;
    text-decoration: none;
    transition: background 0.5s;
}

.btn:hover {
    background: dodgerblue;
}

/* ---------------------------------Contact------------------------------------ */
.contact-left {
    flex-basis: 35%;
}

.contact-left p {
    margin-top: 30px;
}

.contact-left p i {
    color: dodgerblue;
    margin-right: 15px;
    font-size: 25px;
}

.social-icons {
    margin-top: 30px;
}

.social-icons a {
    text-decoration: none;
    font-size: 30px;
    margin-right: 15px;
    color: white;
    display: inline-block;
    transition: transform 0.5s;
}

.social-icons a:hover {
    color: dodgerblue;
    transform: translateY(-5px);
}

.contact-right {
    flex-basis: 60%;
}

.contact-right form {
    width: 100%;
}

form input,
form textarea {
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

form .btn2 {
    margin-top: 20px;
    font-size: 18px;
    padding: 14px 60px;
    cursor: pointer;
}

.btn.btn2 {
    display: inline-block;
    background: dodgerblue;
}

.copyright {
    width: 100%;
    text-align: center;
    padding: 25px 0;
    font-weight: 600;
    font-size: 28px;
    margin-top: 20px;
    background: #abababa1;
}

.copyright p img {
    height: 28px;
}

nav .fas {
    display: none;
}

.upload-form {
    margin: 85px auto 0;
    padding: 15px;
    width: 520px;
    background-color: #262626;
    border-radius: 12px;
}

.upload-form form {
    width: 100%;
    display: block;
}

.upload-form form input,
.upload-form form textarea {
    background-color: white;
}

.upload-form form .btn2 {
    display: block;
}

/* ------------------------css for small screen--------------------- */
@media only screen and (max-width:768px) {
    #header {
        background-image: url("https://img.lovepik.com/background/20211101/medium/lovepik-cool-technology-mobile-phone-wallpaper-background-image_400577939.jpg");
    }

    .header-text h1 span {
        color: #fd053f;
        font-size: 23px;
    }

    .header-text {
        margin-top: 100%;
        font-size: 16px;
    }

    .header-text h1 {
        font-size: 30px;
    }

    .logo {
        width: 70px;
    }

    nav .fas {
        display: block;
        font-size: 25px;
    }

    nav ul {
        background: #4316646b;
        position: fixed;
        top: 0;
        right: -200px;
        border-radius: 0 0 0 10px;
        width: 200px;
        height: fit-content;
        padding-top: 50px;
        z-index: 3;
        transition: right 0.9s;
    }

    nav ul li {
        display: block;
        margin: 25px;
    }

    nav ul .fas {
        position: absolute;
        top: 25px;
        left: 25px;
        cursor: pointer;
    }

    .sub-title {
        font-size: 40px;
    }

    .about-col-1,
    .about-col-2 {
        flex-basis: 100%;

    }

    .about-col-1 {
        margin-bottom: 30px;

    }

    .about-col-2 {
        font-size: 14px;
    }

    .tab-links {
        font-size: 16px;
        margin-right: 20px;
    }

    .contact-left,
    .contact-right {
        flex-basis: 100%;
    }

    .copyright {
        font-size: 13px;
    }

    .copyright p img {
        height: 14px;
    }

    .upload-form {
        width: 300px;
    }
}
#msg{
    color: #61b752;
    margin-top: -10px;
    display: block;
}</style>
<script src="https://kit.fontawesome.com/e1127d2db4.js" crossorigin="anonymous"></script>
</head>
</head>

<body>
    <div id="header">
        <div class="container">
            <nav>
                <a href="index.html"><img class="logo" src="" alt="logo"></a>
                <ul id="sidemenu">
                    <li><a href="#">Home</a></li>
                    <li><a href="#about">About</a></li>
                    <li><a href="#services">Services</a></li>
                    <li><a href="#portfolio">Projects</a></li>
                    <li><a href="#contact">Contact</a></li>
                    <i class="fas fa-times" onclick="closemenu()"></i>
                </ul>
                <i class="fas fa-bars" onclick="openmenu()"></i>
            </nav>
            <div class="header-text">
                <p>Web Developer</p>
                <h1>Hi, I'm<br><span>Sourav Thakur</span> <br>from India</h1>
            </div>
        </div>
    </div>

    
    <div id="about">
        <div class="container">
            <div class="row">
                <div class="about-col-1">
                    <img src="WhatsApp.jpeg" alt="">
                </div>
                <div class="about-col-2">
                    <h1 class="sub-title">About Me</h1>
                    <p>Hello,<br>
                        I am a Web/App Developer.<br> I know Java, Html, CSS, JavaScript,MySql
                        C/C++ and other programming technologies.</p>

                    <div class="tab-titles">
                        <p class="tab-links active-link" onclick="opentab('skills')">Skills</p>
                        <p class="tab-links" onclick="opentab('experience')">Experience</p>
                        <p class="tab-links" onclick="opentab('education')">Education</p>
                    </div>
                    <div class="tab-contents active-tab" id="skills">
                        <ul>
                            <li><span>Full-Stack Developer</span><br>Full-Stack Web Developer</li>
                            <li><span>Web-Development</span><br>Full-Stack Web Developer</li>
                    </div>
                    <div class="tab-contents" id="experience">
                        <ul>
                            <li><span>Jan/2023 -current</span><br>Fresher<br>
                                <strong>Role:</strong>Web Developer</li>
                        </ul>
                    </div>
                    <div class="tab-contents" id="education">
                        <ul>
                            <li><span>2017</span><br>10th from CBSE Board Delhi</li>
                            <li><span>2019</span><br>12th Science from CBSE Board Delhi</li>
                            <li><span>2023</span><br>BCA from IGNOU</li>
                        </ul>
                    </div>
                </div>
            </div>

            
  <div id="services">
    <h1 class="sub-title">My Services</h1>
<div class="services-list">
       <div>
<i class="fa-solid fa-code">
                            
</i>
<h2>Websites</h2>
<p>
Static or Dynamic Website I will create on custom demands.
</p>
                        <a href="#">Learn more</a>
</div>
         <div>
         <i class="fa-solid fa-bug"></i>
        <h2>Others</h2>
      <p>
        I provide you other services like bug fixing  etc.
    </p>
<a href="#">Learn more</a>
</div>
</div>
            </div>

           
            <div id="portfolio">
                <h1 class="sub-title">My Work</h1>
                <div class="work-list">
                    <div class="work">
                        <img src="IMG-20230213-WA0007.jpg" alt="">
                        <div class="layer">
<h3>Portfolio Website</h3>
<p>This is current website on you are watching my projects</p>
<a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
</div>
</div>
<div class="work">
    <img src="Screenshot.png" alt="">
    <div class="layer">
        <h3>Car Rental System</h3>
        <p>This is a simple nike website </p>
        <a href="#"><i class="fa-solid fa-arrow-up-right-from-square"></i></a>
    </div>
</div> 
</div>
<a href="#" class="btn">See More</a>
</div>

<div id="contact">
  <div class="container">
    <div class="row">
     <div class="contact-left">
      <h1 class="sub-title">Contact Me</h1>
    <p><i class="fas fa-paper-plane"></i>tsourav061@gmail.com</p>
  <p><i class="fas fa-phone-square-alt"></i>8368024611</p>
   <div class="social-icons">
       <a href="#"><i class="fa-brands fa-twitter"></i></a>
   <a href="#"><i
        class="fa-brands fa-linkedin"></i></a>
     <a href="#"><i
          class="fa-brands fa-instagram"></i></a>
  </div>
 <a href="C:\Users\gaurav\Desktop\web\sourav thakur.pdf" download class="btn btn2">Download CV</a>
  </div>
<div class="contact-right">
   <form name="submit-to-google-sheet">
  <input type="text" name="name" placeholder="Your Name" required>
<input type="email" name="email" placeholder="Your Email" required>
 <textarea name="message" rows="6" placeholder="Your Message"></textarea>
     <span id="msg"></span>
      <button type="submit" class="btn btn2">Submit</button>
             </form>
          </div>
</div>
</div>
</div>
</div>
</div>
    <div class="copyright">
        <p>Copyright <i class="fa-regular fa-copyright"></i> <img src="favicon.ico" alt="img"> Made with Sourav
            Thakur</p>
    </div>


    <script>
        var tablinks = document.getElementsByClassName("tab-links");
        var tabcontents = document.getElementsByClassName("tab-contents");
        function opentab(tabname) {
            for (tablink of tablinks)
            {
                tablink.classList.remove("active-link");
            }
            for (tabcontent of tabcontents)
            {
                tabcontent.classList.remove("active-tab");
            }
            event.currentTarget.classList.add("active-link");
            document.getElementById(tabname).classList.add("active-tab");
        }
    </script>
    <script>
        var sidemenu = document.getElementById("sidemenu");
        function openmenu() {
            sidemenu.style.right = "0";
        }
        function closemenu() {
            sidemenu.style.right = "-200px"
        }
    </script>
    <script>
        const scriptURL = 'https://script.google.com/macros/s/AKfycbwM_rdKGJR3NyLAUssmJMWH8lSRMj37ibxpikSQD42cwB9JxCcahOBBTSOKhdtdSWGj/exec'
        const form = document.forms['submit-to-google-sheet']
        const msg = document.getElementById("msg");
        form.addEventListener('submit', e => {
            e.preventDefault()
            fetch(scriptURL, { method: 'POST', body: new FormData(form) })
                .then(response => {
                    msg.innerHTML="Message sent Succesfully";
                    setTimeout(function(){
                        msg.innerHTML="";
                    },5000);
                    form.reset()
                })
                .catch(error => console.error('Error!', error.message))
        })
    </script>
</body>

</html>
