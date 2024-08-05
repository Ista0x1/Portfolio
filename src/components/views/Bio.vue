<template>
  <div >
          <img class="self" src="../../assets/Biography/self.jpg" />
          <div class="header">Ismail ista</div>
          <div class="subtitle">Full stack Developer</div>
          <div class="subtitle">casablanca 📍</div>
          <div class="badge-grid">
            <img
              class="badge"
              alt="Node.js"
              src="https://img.shields.io/badge/-Node.js-68a063"
            />
            <img
              class="badge"
              alt="Vue.js"
              src="https://img.shields.io/badge/-Vue.js-61b083"
            />
            <img
              class="badge"
              alt="React.js"
              src="https://img.shields.io/badge/-React.js-61dafb"
            />
            <img
              class="badge"
              alt="PHP"
              src="https://img.shields.io/badge/-PHP-787cb5"
            />
            <img
              class="badge"
              alt="Laravel"
              src="https://img.shields.io/badge/-Laravel-ff2d20"
            />
            <img
              class="badge"
              alt="MySQL"
              src="https://img.shields.io/badge/-MySQL-4479a1"
            />
            <img
              class="badge"
              alt="MongoDB"
              src="https://img.shields.io/badge/-MongoDB-4ca158"
            />
            <img
              class="badge"
              alt="Express.js"
              src="https://img.shields.io/badge/-Express.js-404d59"
            />
            <img
              class="badge"
              alt="WordPress"
              src="https://img.shields.io/badge/-WordPress-21759b"
            />
            <img
              class="badge"
              alt="Git"
              src="https://img.shields.io/badge/-Git-critical"
            />
            <img
              class="badge"
              alt="Postman"
              src="https://img.shields.io/badge/-Postman-ff6c37"
            />
            <img
              class="badge"
              alt="C#"
              src="https://img.shields.io/badge/-C%23-239120"
            />
          </div>
          <div class="inner-content">
            <div class="heading"><b>About Me</b></div>
            <div class="paragraph">
              Hello, I'm Ismail Ista, a passionate full-stack developer based in
              Casablanca, Morocco. In 2022, I earned my specialized diploma in
              software development from ISTA, marking the beginning of my
              journey into the world of programming. Driven by a genuine love
              for coding and problem-solving, I decided to enhance my skills
              further. In 2023, I completed the JobInTech Bootcamp,
              specializing in the MERN (MongoDB, Express.js, React.js, Node.js)
              stack. This intensive experience has equipped me with a solid
              foundation in modern web development.
            </div>
            <div class="paragraph">
              I have worked with a mixture of design and frontend/backend
              technologies, be it for Web Development.
            </div>
          </div>
          <div class="inner-content">
            <div class="heading"><b>Experience </b></div>
            <div class="heading"><b>Internship at OFPPT NTIC 1 </b></div>
            <div class="paragraph">
              During my internship at OFPPT NTIC 1, I played the role of a Web
              Developer Intern. I was responsible for creating a web application
              using PHP, HTML, CSS, and JavaScript. The application focused on
              efficiently managing coaches, courses, and schedules, providing a
              streamlined process before the commencement of teaching at ISTA.
            </div>
          </div>

          <div class="inner-content">
            <div class="heading"><b>TrendTek Media</b></div>
            <div class="paragraph">
              At TrendTek Media Digital Agency, I served as a Web Developer. My
              responsibilities included creating websites using WordPress.
              Additionally, I took a lead role in the development of the
              CherinKargo app. This comprehensive application facilitated the
              management of shipping, money transfers, and the handling of
              invoices, contributing to the agency's digital solutions.
            </div>
          </div>

          <div class="inner-content">
            <div class="heading"><b>Azoul Media</b></div>
            <div class="paragraph">
              As a Full Stack Developer at Azoul Media Digital Agency, I took on
              a versatile role that involved both frontend and backend
              development. I successfully created websites using WordPress and
              PHP, showcasing my proficiency in crafting visually appealing and
              functional web solutions.
            </div>
          </div>

          <div class="inner-content">
            <div class="heading"><b>Sportma</b></div>
            <div class="paragraph">
              In continuation, I played a pivotal role in the SportMa project,
              where I served as the lead developer. For SportMa, I designed and
              implemented a robust Laravel API, forming the backbone of the
              mobile application. SportMa is an innovative platform that
              simplifies the booking of sports activities, fosters community
              engagement, and provides interactive chatrooms for users. This
              project allowed me to apply my full-stack skills to deliver a
              seamless and engaging user experience for sports enthusiasts.
            </div>
            <div class="paragraph">
              sportma :
              <a
                style="color: #ff5733"
                target="_blank"
                href="https://play.google.com/store/apps/details?id=ma.sportma.client"
                >[mobile app]</a
              >
              <a style="color: #ff5733" href="https://sportma.app/"
                >[Website]</a
              >
            </div>
          </div>

          <div class="inner-content">
            <div class="heading"><b>DevMasters</b></div>
            <div class="paragraph">
              Dedicated to catalyzing creativity and collaboration within the
              developer community, the Devmasters Marketplace is a dynamic
              digital products platform co-crafted by myself, Walid Telmasani,
              and Ahmed Sajir. This venture emerged from our shared passion for
              empowering developers to showcase, share, and monetize their
              creations.
            </div>
            <div class="paragraph">
              The project's robust foundation rests on the MERN (MongoDB,
              Express.js, React.js, Node.js) stack. This technology ensemble
              ensured a scalable and responsive marketplace, with MongoDB
              handling flexible data storage, Express.js orchestrating a
              powerful backend, React.js delivering a dynamic user interface,
              and Node.js facilitating seamless communication.
            </div>
          </div>

          <!-- <div class="inner-content">
                            <div class="heading"><b>Interests and Hobbies</b></div>
                            <div class="paragraph">Analog photography and colorizing of historical photos have always interested me and some of my photographic works are displayed <span style="cursor: pointer; color: #FF5733;" v-on:click="showPhotos">here</span> while you can find my colorization portfolio <span style="cursor: pointer; color: #FF5733;" v-on:click="showColorization">here</span>.</div>
                        </div> -->

          <div class="inner-content">
            <div class="heading"><b>Résumé</b></div>
            <a
              style="color: #ff5733"
              href="/files/ismailistaresume.pdf"
              class="paragraph"
              >Check out my résumé here.</a
            >
          </div>
  </div>
</template>

<style scoped>
.badge-grid {
  display: table;
  align-items: center;
  margin-top: 20px;
}

.badge {
  width: auto;
  height: 20px;
  border-radius: 0px;
  font-size: 12px;
  padding-right: 10px;
  /* box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.12), 0 6px 20px 0 rgba(0, 0, 0, 0.1); */
}

.self {
  width: 100%;
  height: auto;
  /* border-radius: 5px; */
}

.subtitle {
  font-size: 12px;
  color: gray;
}

.heading {
  padding-bottom: 5px;
}

.header {
  padding-top: 20px;
  padding-bottom: 20px;
}

.inner-content {
  padding-top: 30px;
}

h2,
h4,
h3 {
  padding: 0;
  margin: 0;
}
</style>
