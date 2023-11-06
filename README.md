<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
    <!-- For font -->
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link
      href="https://fonts.googleapis.com/css2?family=Pacifico&display=swap"
      rel="stylesheet"
    />
    <!-- External CSS -->
    <link rel="stylesheet" href="style.css" />

    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.2/css/all.min.css"
    />

    <!-- To get navbar collapse icon -->
    <link
      rel="stylesheet"
      href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
    />

    <!-- For social Media icons -->
    <link
      href="https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css"
      rel="stylesheet"
    />
    <!-- For typing Animation -->
    <script src="https://unpkg.com/typed.js@2.0.16/dist/typed.umd.js"></script>


    <!-- Linking Bootstrap for navbar -->
    
    
  </head>
  <body>
    <!-- For Nav Bar -->
    
    <header class="header">
      <a href="#" class="logo">Mukul Anand</a>
      <nav class="navbar" id="myTopnav">
        <a href="./index.html" style="--i: 1">Home</a>
        <a href="./about.html" style="--i: 2">About</a>
        <a href="./skills.html" style="--i: 3">Skills</a>
        <a href="./project.html" style="--i: 4">Projects</a>
        <a href="./contact.html" style="--i: 5">Contact</a>

        <!-- Icon to appear when navbar collapse -->
        <a href="javascript:void(0);" class="icon" onclick="myFunction()">
          <i class="fa fa-bars"></i>
        </a>
      </nav>
    </header>

    <!-- To hide when there is large screen -->
    <style>
      .navbar .icon {
        display: none;
      }

      @media screen and (max-width: 920px) {
        .navbar a {
          display: none;
        }
        .navbar a.icon {
          position: fixed;
          top: 0;
          right: 0;
          margin-right: 12px;
          margin-top: 12px;
          float: left;
          display: block;
          
        }
        .header {
          background-color: #080808;
        }

        .logo {
          position:fixed;
          top: 0;
          left: 0;
          margin-left: 12px;
          margin-top: 12px;
        }
      }

      @media screen and (max-width: 920px) {
        .navbar.responsive {
          position: fixed;
          right: 0;
          top: 0;
          /* opacity: 0.5; */
          
          background-color: #080808;
        }
        .navbar.responsive .icon {
          position: fixed;
          /* right: -30px; */
          top: 0;

        }
        .navbar.responsive a:not(:last-child) {
          /* background-color: black; */
          position: relative;
          /* top: 0; */
          /* right: 0; */
          margin-left: 20px;
          margin-bottom: 10px;
          padding-right: 20px;
          /* margin-right: 20px; */
          float: none;
          display: block;
          /* flex-direction: column; */
          text-align: left;
        }
      }
    </style>

    <!-- Script for navbar collapse -->
    <script>
      function myFunction() {
        var x = document.getElementById("myTopnav");
        if (x.className === "navbar") {
          x.className += " responsive";
        } else {
          x.className = "navbar";
        }
      }
    </script>

    <!-- For Home section -->
    <section class="home" id="home">
      <div class="home-content">
        <h1 class="buttomAnima">Hi!, I'm</h1>
        <h1><span>Mukul Anand</span></h1>
        <h3 class="buttomAnima">And I'm a <span id="text"></span></h3>
        <p>
          Welcome to my website! I am a dedicated and passionate web developer
          <br />
          with a diverse skill set that encompasses a wide range of
          technologies...
        </p>
        <div class="home-sci">
          <a href="https://www.linkedin.com/in/mukul-anand-131-/" style="--i: 7"
            ><i class="bx bxl-linkedin"></i
          ></a>
          <a href="https://github.com/mukulanand131" style="--i: 8"
            ><i class="bx bxl-github"></i
          ></a>
          <a
            href="https://instagram.com/mukul_anand___?igshid=OGQ5ZDc2ODk2ZA=="
            style="--i: 9"
            ><i class="bx bxl-instagram"></i
          ></a>
          <a href="https://wa.me/qr/CLF66BXRUDRSJ1" style="--i: 10"
            ><i class="bx bxl-whatsapp"></i
          ></a>
        </div>
        <!-- Download CV Button -->
        <div class="btn-con">
          <a href="./Resumes/Web dev Resume.pdf" class="main-btn" target="_blank">
              <span class="btn-box">Download CV <i class="fas fa-download"></i></span>
          </a>  
      </div>
      </div>
      <span class="home-imgHover"></span>
      
    </section>

    <!-- For about Section -->
    <section class="about" id="about">
      <div class="about-img">
        <img src="./images/profile-pic.jpg" alt="" />
      </div>
      <div class="about-text">
        <h2>About<span>Me</span></h2>
        <h4>Full Stack Web Developer</h4>
        <p>
          Hello, I'm Mukul Anand, a Computer Science and Engineering student
          with a passion for coding and web development. I've been honing my
          skills as a full-stack web developer for a year now and am eager to
          continue my learning journey. My focus on the front end involves
          creating visually appealing websites using HTML5, CSS3, and responsive
          design principles. I take pride in crafting engaging user interfaces
          that provide exceptional experiences across various devices and
          browsers. On the back end, I have proficiency in server-side
          technologies like Node.js and Express.js, along with experience in
          working with database systems like MongoDB and MySQL. This enables me
          to build robust and functional web applications. If you're in need of
          a dedicated and skilled front-end developer, I'm keen to connect with
          you and explore how I can contribute to your team or project. Let's
          discuss potential opportunities!
        </p>

        <a href="./about.html" class="btn-box">More About Me</a>
      </div>
    </section>

    <!-- For education Section -->
    <section class="education" id="education">
      <div class="container">
        <h1 class="sub-education">My <span>Education</span></h1>
        <div class="education-list">
          <div>
            <i class="bx bxl-firebase" style="color: #00eeff"></i>
            <h2 class="course">AISSE</h2>
            <h2>Shantiniketan Jubilee School,</h2>
            <h3>Motihari</h3>
            <i class="bx bx-calendar toReduceSize" style="color: #00eeff"></i>
            <h4 class="calander">2016-17</h4>
            <h4 class="grade">CGPA: 10</h4>
            <p></p>
          </div>
          <div>
            <i class="bx bx-book-open" style="color: #00eeff"></i>
            <h2 class="course">AISSCE</h2>
            <h2>Shantiniketan Jubilee School,</h2>
            <h3>Motihari</h3>
            <i class="bx bx-calendar toReduceSize" style="color: #00eeff"></i>
            <h4 class="calander">2017-19</h4>
            <h4 class="grade">Grade: 82.6%</h4>
            <p></p>
          </div>
          <div>
            <i class="bx bxs-graduation" style="color: #00eeff"></i>
            <h2 class="course">B.Tech. (CSE)</h2>
            <h2>Mahatma Gandhi Central University, Motihari</h2>
            <i class="bx bx-calendar toReduceSize" style="color: #00eeff"></i>
            <h4 class="calander">2020-24</h4>
            <h4 class="grade">Grade: 84%</h4>
            <p></p>
          </div>
        </div>
      </div>
    </section>

    <h1 class="skill-land-head">My <span>Skills</span></h1>
    <!-- For Skills -->
    <section class="skills-land" id="skills-land">
      <div class="skill-flex-land">
        <div class="container1-land">
          <h1 class="heading1-land">Technical Skills</h1>
          <!-- Technical Skills -->
          <div class="technical-bars-land">
            <div class="bar-land">
              <i class="bx bxl-python" style="color: #c32ec9"></i>
              <div class="info-land">
                <span>Python</span>
              </div>
              <div class="progress-line-land python">
                <span></span>
              </div>
            </div>
            <div class="bar-land">
              <i class="bx bxl-html5" style="color: #c95d2e"></i>
              <div class="info-land">
                <span>HTML</span>
              </div>
              <div class="progress-line-land html">
                <span></span>
              </div>
            </div>
            <div class="bar-land">
              <i class="bx bxl-css3" style="color: #147bbc"></i>
              <div class="info-land">
                <span>CSS</span>
              </div>
              <div class="progress-line-land css">
                <span></span>
              </div>
            </div>
            <div class="bar-land">
              <i class="bx bxl-bootstrap" style="color: #00eeff"></i>
              <div class="info-land">
                <span>Bootstrap</span>
              </div>
              <div class="progress-line-land bootstrap">
                <span></span>
              </div>
            </div>
            <div class="bar-land">
              <i class="bx bxl-javascript" style="color: #b0bc1e"></i>
              <div class="info-land">
                <span>JavaScript</span>
              </div>
              <div class="progress-line-land javascript">
                <span></span>
              </div>
            </div>
            <div class="bar-land">
              <i class="bx bxl-jquery" style="color: #00eeff"></i>
              <div class="info-land">
                <span>jQuery</span>
              </div>
              <div class="progress-line-land jquery">
                <span></span>
              </div>
            </div>
          </div>
        </div>

        <!-- Professional Skills -->
        <div class="container2-land">
          <h1 class="heading2-land">Professional Skills</h1>
          <div class="radial-bars-land">
            <div class="radial-bar-land">
              <svg x="0px" y="0px" viewBox="0 0 200 200">
                <circle
                  class="progress-bar-land"
                  cx="100"
                  cy="100"
                  r="80"
                ></circle>
                <circle
                  class="path-land path-1"
                  cx="100"
                  cy="100"
                  r="80"
                ></circle>
              </svg>
              <div class="percentage-land">90%</div>
              <div class="text-land">Creativity</div>
            </div>
            <div class="radial-bar-land">
              <svg x="0px" y="0px" viewBox="0 0 200 200">
                <circle
                  class="progress-bar-land"
                  cx="100"
                  cy="100"
                  r="80"
                ></circle>
                <circle
                  class="path-land path-2"
                  cx="100"
                  cy="100"
                  r="80"
                ></circle>
              </svg>
              <div class="percentage-land">85%</div>
              <div class="text-land">Communication</div>
            </div>
            <div class="radial-bar-land">
              <svg x="0px" y="0px" viewBox="0 0 200 200">
                <circle
                  class="progress-bar-land"
                  cx="100"
                  cy="100"
                  r="80"
                ></circle>
                <circle
                  class="path-land path-3"
                  cx="100"
                  cy="100"
                  r="80"
                ></circle>
              </svg>
              <div class="percentage-land">85%</div>
              <div class="text-land">Problem Solving</div>
            </div>
            <div class="radial-bar-land">
              <svg x="0px" y="0px" viewBox="0 0 200 200">
                <circle
                  class="progress-bar-land"
                  cx="100"
                  cy="100"
                  r="80"
                ></circle>
                <circle
                  class="path-land path-4"
                  cx="100"
                  cy="100"
                  r="80"
                ></circle>
              </svg>
              <div class="percentage-land">90%</div>
              <div class="text-land">TeamWork</div>
            </div>
          </div>
        </div>

        <div class="container3-land">
          <h1 class="heading1-land">Technical Skills</h1>
          <div class="technical-bars-land">
            <div class="bar-land">
              <i class="bx bxl-react" style="color: #69bcbc"></i>
              <div class="info-land">
                <span>React</span>
              </div>
              <div class="progress-line-land react">
                <span></span>
              </div>
            </div>
            <div class="bar-land">
              <i class="bx bxl-nodejs" style="color: #07a15a"></i>
              <div class="info-land">
                <span>Node.js</span>
              </div>
              <div class="progress-line-land nodejs">
                <span></span>
              </div>
            </div>
            <div class="bar-land">
              <!-- image -->
              <img src="icons/sql-database-sql-azure.svg" alt="" />
              <div class="info-land">
                <span>SQL</span>
              </div>
              <div class="progress-line-land sql">
                <span></span>
              </div>
            </div>
            <div class="bar-land">
              <i class="bx bxl-mongodb" style="color: #0c7a47"></i>
              <div class="info-land">
                <span>MongoDB</span>
              </div>
              <div class="progress-line-land mongodb">
                <span></span>
              </div>
            </div>
            <div class="bar-land">
              <i class="bx bxl-django" style="color: #1a9f46"></i>
              <div class="info-land">
                <span>Django</span>
              </div>
              <div class="progress-line-land django">
                <span></span>
              </div>
            </div>
            <div class="bar-land">
              <i class="bx bx-brain" style="color: #1294cb"></i>
              <div class="info-land">
                <span>Machine Learning</span>
              </div>
              <div class="progress-line-land machineLearning">
                <span></span>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section>
      <div id="portfolio" itemid="project">
        <div class="main-text" id="project">
          <h2>Latest <span>Project</span></h2>
          <div class="portfolio-content">
            <div class="row">
              <img src="./images/Streamlit web page Heart.png" alt="" />
              <div class="layer">
                <h5>Multiple Malady Prediction System Using ML</h5>
                <p>
                  This Project was a simple prototype of multiple disease
                  detection which includes
                  <span>"Heart Disease Prediction"</span> and
                  <span>"Diabetes Disease Prediction"</span>. This was
                  accomplished by using some algorithms of ML and some
                  standardization techniques.
                </p>

                <p class="tools">
                  TOOLS - Machine Learning Algorithms, Spyder.
                </p>

                <a href="#"
                  ><i class="bx bx-link-external" style="color: aliceblue"></i
                ></a>
              </div>
            </div>
            <div class="row">
              <img src="./images/time series.jpg" alt="" />
              <div class="layer">
                <h5>Deep Learning Insights Using Time Series Data</h5>
                <p>
                  This Project on Time Series Data of 25 years taken from NASA.
                  This was accomplished by using some algorithms of ML, DL and
                  some standardization techniques.
                </p>

                <p class="tools">
                  TOOLS - Machine Learning Algorithms, Google Collab.
                </p>

                <a href="#"
                  ><i class="bx bx-link-external" style="color: aliceblue"></i
                ></a>
              </div>
            </div>
            <div class="row">
              <img src="./images/Dice game.jpg" alt="" />
              <div class="layer">
                <h5>Dice Game</h5>
                <p>
                  This Project on Time Series Data of 25 years taken from NASA.
                  This was accomplished by using some algorithms of ML, DL and
                  some standardization techniques.
                </p>

                <p class="tools">
                  TOOLS - Machine Learning Algorithms, Google Collab.
                </p>

                <a href="#"
                  ><i class="bx bx-link-external" style="color: aliceblue"></i
                ></a>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- For Contact section -->
    <section class="contact" id="contact">
      <div class="contact-text">
        <h2>Contact <span>Me</span></h2>
        <h4>Let's work Together</h4>
        <p>
          Let's work together to bring your ideas to life! I'm excited to hear
          from you and explore how we can collaborate to achieve your goals.
          Whether you have a project in mind, a question to ask, or just want to
          connect, feel free to reach out. I'm here to listen, share ideas, and
          find the best solutions to meet your needs. You can contact me via the
          provided email address or through the contact form below. I look
          forward to the opportunity to work together and make your vision a
          reality.
        </p>
        <div class="contact-list">
          <li>
            <i class="bx bxs-send" style="color: #00eeff"></i
            >mukulanand131@gmail.com
          </li>
          <li><i class="bx bx-phone" style="color: #00eeff"></i>8271862583</li>
        </div>
        <div class="contact-icons">
          <a href="https://www.facebook.com/mukul.anand.146069"><i class="bx bxl-facebook-circle"></i></a>
          <a href="https://twitter.com/Mukul_Anand__"><i class="bx bx-x"></i></a>
          <a href="https://instagram.com/mukul_anand___?igshid=OGQ5ZDc2ODk2ZA=="
            ><i class="bx bxl-instagram"></i
          ></a>
          <a href="https://www.linkedin.com/in/mukul-anand-131-/"
            ><i class="bx bxl-linkedin"></i
          ></a>
        </div>
      </div>

      <div class="contact-form">
        <form action="">
          <input type="" placeholder="Enter Your Name" required />
          <input type="email" placeholder="Enter Your Email" required />

          <input type="" placeholder="Enter Your Subject" required />
          <textarea
            name=""
            id=""
            cols="40"
            rows="10"
            placeholder="Enter Your Message"
            required
          ></textarea>
          <input type="button" value="Submit" class="send" />
        </form>
      </div>
    </section>

    <div class="last-text">
      <p>
        Developed with love
        <i class="bx bx-happy-heart-eyes" style="color: #00eeff"></i> by
        <span class="name">Mukul Anand</span>
      </p>
    </div>

    <a href="#home" class="top"><i class="bx bx-arrow-to-top"></i></a>

    <!-- Setup and start animation! -->
    <script>
      var typed = new Typed("#text", {
        strings: ["Full Stack Web Developer", "&amp; Programar"],
        typeSpeed: 100,
        backSpeed: 100,
        backDelay: 1000,
        loop: true,
      });
    </script>
    <script src="main.js"></script>
  </body>
</html>
