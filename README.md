<html>
<head>
<title>Elaine Lee</title>

<link rel="stylesheet" href="css/style.css">

</head>
<body>
<div id="header">
<div class="container">
    <nav>
        <img src="/Images/Black White Modern Handwritten Square Studio Logo.png" class="logo">
        <ul>
            <li><a href="#">About</a></li>
            <li><a href="#">Skills</a></li>
            <li><a href="#">Portfolio</a></li>
            <li><a href="#">Contact</a></li>

            </li>
        </ul>

    </nav>
<!------------ Hero Section----------->
<section class="hero" id="about">
    <img src="/Images/green.png" class="hero-img" width="450" height="450">
    
    <div class="bio">
      <h2 class="bio-title">Hi! Nice to meet you &#128075; </h2>
      <p class="bio-text">
        I’m Elaine, a UX/UI designer passionate about creating digital designs. With a commitment to user-centric design, I blend creativity with problem-solving. Explore my portfolio and let's connect to collaborate on designing the next digital masterpiece!
      </p>
    </div>
  </section>

<!--------------- about--------------->
<section class="more-about">
  <h2>About Me</h2>
  <p>
    I am an innovative visual design professional (UX/UI) passionate about developing digital products. Equipped with a solid educational foundation in design and a recent graduate from George Washington UX/UI design bootcamp. I have hands-on proficiency in design tools such as HTML/CSS and Figma. Strengths in creativity, teamwork, and building projects from ideation to execution allows me to be a valuable addition to any team. Check out some of my projects!</p>
    <a href="#" class="btn">Download CV</a>

  <!---------------Skills--------------->
<section class="mySkills" id="skillssection">
  <h1> My Skills</h1>
  <div class="flexContainer">
      <div class="skill1">
          <h4>Software</h4>
          <p>Visual Code Figma Miro Canva</p>
      </div>
      <div class="skill2">
          <h4>UX/UI</h4>
          <p>HTML CSS Storyboard Affinity Map Wireframe Prototype User Research Design Research</p>
      </div>
      <div class="skill3">
          <h4>Business</h4>
          <p>Project Management Agile Problem Solving Data Analysis Recruitment</p>
      </div>
  </div>
  </section>

 <!-- Projects section -->
 <section class="projects" id="projects">
  <h2 class="projects-title">Recent Projects</h2>
  <div class="projects-container">
    <div class="project-container project-card">
      <img
        src="/Images/dept of edu .png"
        alt="deptofedu"
        loading="lazy"
        class="project-pic"
      />
      <h3 class="project-title">Department of Education Redesign</h3>
      <p class="project-details">
        I undertook the redesign of the Department of Education homepage with a primary goal of improving user accessibility. 
        The project involved streamlining navigation. 
      </p>
      <a href="#" target="_blank" class="project-link">Check it Out</a>
    </div>
    <div class="project-container project-card">
      <img
        src="/Images/Untitled design (55).png"
        alt="travelguardian"
        loading="lazy"
        class="project-pic"
      />
      <h3 class="project-title">Travel Guardian</h3>
      <p class="project-details">
        I designed an app that addresses the safety concerns of travelers by providing valuable insights into secure destinations.
         The app aims to ease anxiety and instill confidence in users, enabling them to explore new places with peace of mind.
      </p>
      <a href="#" target="_blank" class="project-link">Check it Out</a>
    </div>
    <div class="project-container project-card">
      <img
        src="/Images/Untitled design (55).png"
        alt="travel guardian"
        loading="lazy"
        class="project-pic"
      />
      <h3 class="project-title">Transformer Redesign</h3>
      <p class="project-details">
        I redesigned an art museum Transformer's webpage to focuses on enhancing user experience and accessibility to museum information and exhibits. 
      </p>
      <a href="#" target="_blank" class="project-link">Check it Out</a>
    </div>
  </div>
</section>

<!-- Contact section -->
<section class="contact" id="contact">
    <h2>Let's Connect</h2>
    <div class="contact-form-container">
      <div class="contact-form">
        <form action="https://formspree.io/f/xyylnggw" method="POST">
          <div class="form-control">
            <label for="name">Name</label>
            <input
              type="text"
              id="name"
              name="sender-name"
              placeholder="Enter Your Name"
              class="input-field"
              required
            />
          </div>
          <div class="form-control">
            <label for="email">Email</label>
            <input
              type="email"
              id="email"
              name="sender-email"
              placeholder="Enter Your Email"
              class="input-field"
              required
            />
          </div>
          <div class="form-control">
            <label for="message">Message</label>
            <textarea
              id="message"
              cols="60"
              rows="10"
              placeholder="Enter Your Message"
              name="message"
              class="input-field"
              required
            ></textarea>
          </div>
          <input
            type="submit"
            value="Submit"
            id="submit-btn"
            class="submit-btn"
          />
        </form>
      </div>
    </div>
  </section>

</div>






<!-- Code injected by live-server -->
<script>
	// <![CDATA[  <-- For SVG support
	if ('WebSocket' in window) {
		(function () {
			function refreshCSS() {
				var sheets = [].slice.call(document.getElementsByTagName("link"));
				var head = document.getElementsByTagName("head")[0];
				for (var i = 0; i < sheets.length; ++i) {
					var elem = sheets[i];
					var parent = elem.parentElement || head;
					parent.removeChild(elem);
					var rel = elem.rel;
					if (elem.href && typeof rel != "string" || rel.length == 0 || rel.toLowerCase() == "stylesheet") {
						var url = elem.href.replace(/(&|\?)_cacheOverride=\d+/, '');
						elem.href = url + (url.indexOf('?') >= 0 ? '&' : '?') + '_cacheOverride=' + (new Date().valueOf());
					}
					parent.appendChild(elem);
				}
			}
			var protocol = window.location.protocol === 'http:' ? 'ws://' : 'wss://';
			var address = protocol + window.location.host + window.location.pathname + '/ws';
			var socket = new WebSocket(address);
			socket.onmessage = function (msg) {
				if (msg.data == 'reload') window.location.reload();
				else if (msg.data == 'refreshcss') refreshCSS();
			};
			if (sessionStorage && !sessionStorage.getItem('IsThisFirstTime_Log_From_LiveServer')) {
				console.log('Live reload enabled.');
				sessionStorage.setItem('IsThisFirstTime_Log_From_LiveServer', true);
			}
		})();
	}
	else {
		console.error('Upgrade your browser. This Browser is NOT supported WebSocket for Live-Reloading.');
	}
	// ]]>
</script>
</body>








</div>

</html>
