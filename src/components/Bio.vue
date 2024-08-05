/* eslint-disable */
<template>
  <interact
    draggable
    :dragOption="dragOption"
    class="resize-drag"
    :style="style"
    @dragmove="dragmove"
    @resizemove="resizemove"
    :class="{ fullscreen: $store.getters.isFullscreenBio }"
  >
    <div
      class="window"
      id="container"
      :class="{
        fullscreen: $store.getters.isFullscreenBio,
        close: !$store.getters.isShownBio,
      }"
    >
      <div
        class="top-bar"
        id="top-bar"
        v-on:dblclick="$store.commit('toggleFullscreenBio')"
        :class="
          $store.getters.activeWindow == 'Bio'
            ? 'top-bar'
            : 'top-bar-deactivated'
        "
      >
        <div
          style="
            color: white;
            margin-left: 3px;
            display: flex;
            align-items: center;
          "
        >
          <img class="icon-image" src="../assets/win95Icons/bio.png" />Biography
        </div>
        <div class="triple-button">
          <div class="button-hide" v-on:click="minimizeBio">
            <span
              style="
                height: 2px;
                width: 6px;
                background: black;
                margin-top: 8px;
                margin-right: 2px;
              "
            ></span>
          </div>
          <div
            class="button-expand"
            v-on:click="$store.commit('toggleFullscreenBio')"
          >
            <span
              style="
                height: 8px;
                width: 9px;
                border-left: black 1px solid;
                border-right: black 1px solid;
                border-left: black 1px solid;
                border-bottom: black 1px solid;
                border-top: black 2px solid;
              "
            ></span>
          </div>
          <div
            style="margin-right: 3px; padding-left: 1px"
            class="button-close"
            v-on:click="closeBio"
          >
            ×
          </div>
        </div>
      </div>
      <div class="content">
        <div
          class="scroll-container"
          :class="{ expandedScrollContainer: $store.getters.isFullscreenBio }"
        >
          <img class="self" src="../assets/Biography/self.jpg" />
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
              further. In 2024, I successfully completed the JobInTech Bootcamp,
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
      </div>
    </div>
  </interact>
</template>

<style scoped>
.resize-drag {
  box-sizing: border-box;
  background: none;
  user-select: auto;
  -ms-touch-action: auto;
  touch-action: auto;
  min-height: 40px;
  min-width: 350px;
  position: sticky;
  cursor: auto !important;
}

.window {
  min-height: 500px;
  min-width: 350px;
  height: 500px;
  width: 600px;
  background: rgb(195, 195, 195);
  overflow: hidden;
  border-top: solid rgb(250, 250, 250) 2px;
  border-left: solid rgb(250, 250, 250) 2px;
  border-right: solid rgb(90, 90, 90) 1.5px;
  border-bottom: solid rgb(90, 90, 90) 1.5px;
  box-shadow: 1.5px 1.5px black;
  max-height: 100%;
  max-width: 100%;
  align-items: flex-end;
  outline: rgb(222, 222, 222) 1px solid;
}

.self {
  width: 100%;
  height: auto;
  /* border-radius: 5px; */
}

@media only screen and (max-width: 600px) {
  .window {
    min-width: 50vw;
    width: 90vw;
    max-width: 100vw;
  }
  .scroll-container {
    padding-left: 10vw !important;
    padding-right: 10vw !important;
  }
  .expandedScrollContainer {
    padding-left: 10vw !important;
    padding-right: 10vw !important;
  }
}

.button-expand,
.button-close,
.button-hide {
  background: rgb(195, 195, 195);
  border-top: solid rgb(250, 250, 250) 1px;
  border-left: solid rgb(250, 250, 250) 1px;
  border-right: solid rgb(90, 90, 90) 1px;
  border-bottom: solid rgb(90, 90, 90) 1px;
  box-shadow: 1px 1px black;
  height: 16px;
  width: 16px;
  display: flex;
  justify-content: center;
  align-items: center;
  font-size: 20px;
  font-weight: bold;
  margin-left: 2px;
}

.button-close:hover,
.button-expand:hover,
.button-hide:hover {
  cursor: pointer;
}

.button-close:active,
.button-expand:active,
.button-hide:active {
  border-radius: 0px;
  background: rgb(192, 192, 192);
  box-shadow: none;
  border-top: solid rgb(0, 0, 0) 1.5px;
  border-left: solid rgb(0, 0, 0) 1.5px;
  border-bottom: solid rgb(250, 250, 250) 1.5px;
  border-right: solid rgb(250, 250, 250) 1.5px;
}

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

.subtitle {
  font-size: 12px;
  color: gray;
}

.heading {
  padding-bottom: 5px;
}

.inner-content {
  padding-top: 30px;
}

.inner-content:last-child {
  padding-bottom: 80px;
}

.fullscreen {
  width: 100% !important;
  height: var(--fullscreen) !important;
  margin: 0;
  transition: all 0.5s ease;
  padding: 0;
}

.nossaflex-app {
  max-width: 64px;
  max-height: 64px;
  border-radius: 22%;
  overflow: hidden;
  display: inline-block;
  vertical-align: middle;
  background-image: url("../assets/Icons/NossaflexLight.webp");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  border: rgb(0, 0, 0, 0, 0.5) 1px solid;
}

.close {
  display: none;
}

.show {
  display: block;
}

.top-bar {
  display: flex;
  height: 25px;
  width: auto;
  background: rgb(0, 0, 124);
  z-index: 10;
  align-items: center;
  justify-content: space-between;
  flex-direction: row;
  margin: 2px;
}

.top-bar-deactivated {
  background: rgb(123, 125, 123);
}

.triple-button {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.button-red {
  height: 12px;
  width: 12px;
  border-radius: 50%;
  background: #ed6a06;
  display: flex;
  justify-content: center;
  align-items: center;
}

.button-yellow {
  height: 12px;
  width: 12px;
  border-radius: 50%;
  background: #f5bf50;
}

.button-green {
  height: 12px;
  width: 12px;
  border-radius: 50%;
  background: #62c454;
}

.button-red:hover {
  cursor: pointer;
}

.button-yellow:hover {
  cursor: pointer;
}

.button-green:hover {
  cursor: pointer;
}

.textarea-content {
  width: 100%;
  height: 100%;
  background: none;
  border: none;
  overflow: auto;
  outline: none;
  -webkit-box-shadow: none;
  -moz-box-shadow: none;
  box-shadow: none;
  resize: none;
  caret-color: black;
  color: black;
}

.bar {
  background: rgb(0, 0, 124);
  height: 1px;
  width: 100%;
}

.circle {
  background: #f1f0f2;
  width: 150px;
  height: 150px;
  border-radius: 50%;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.05), 0 6px 20px 0 rgba(0, 0, 0, 0.05);
  display: flex;
  justify-content: center;
  align-items: center;
}

.content {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: flex-start;
  height: 100%;
}

.header {
  font-weight: 700;
  font-size: 28px;
  padding-top: 10px;
}

.scroll-container {
  overflow: scroll;
  padding-left: 50px;
  padding-right: 50px;
  padding-top: 20px;
}

.expandedScrollContainer {
  padding-left: 25vw;
  padding-right: 25vw;
}

.paragraph {
  font-weight: 100;
  font-size: 14px;
  padding-bottom: 10px;
}

.paragraph:last-child {
  padding-bottom: 0px;
}

.resizer-r {
  cursor: col-resize;
  height: 100%;
  right: 0;
  top: 0;
  width: 5px;
}

.resizer-b {
  bottom: 0;
  cursor: row-resize;
  height: 5px;
  left: 0;
  width: 100%;
}

.resizer-t {
  top: 0;
  cursor: row-resize;
  height: 5px;
  left: 0;
  width: 100%;
}

.resizer-l {
  cursor: col-resize;
  height: 100%;
  left: 0;
  bottom: 0;
  width: 5px;
}

.resizer {
  position: absolute;
}
</style>

<script>
import interact from "interactjs";
export default {
  props: {
    // shownProp: Boolean
  },
  data: function () {
    return {
      resizeOption: {
        edges: { top: true, left: true, bottom: true, right: true },
      },
      positions: {
        clientX: undefined,
        clientY: undefined,
        movementX: 0,
        movementY: 0,
      },
      dragOption: {
        modifiers: [
          interact.modifiers.restrictRect({
            restriction: "parent",
            endOnly: true,
          }),
        ],
        allowFrom: ".top-bar",
      },

      // values for interact.js transformation
      x: 0,
      y: 0,
    };
  },
  computed: {
    style() {
      return {
        height: `${this.h}px`,
        width: `${this.w}px`,
        transform: `translate(${this.x}px, ${this.y}px)`,
        "--fullscreen": window.innerHeight - 40 + "px",
      };
    },
  },
  methods: {
    // showPhotos(e) {
    //   e.stopPropagation();
    //   this.$store.commit("changeActiveWindow", "Photos");
    //   this.$store.commit("toggleShownPhotos", true);
    //   setTimeout(() => {
    //     this.$store.commit("zIndexIncrement", "photos");
    //   }, 1);
    // },
    showColorization(e) {
      e.stopPropagation();
      this.$store.commit("changeActiveWindow", "Colorization");
      this.$store.commit("toggleShownColorization", true);
      setTimeout(() => {
        this.$store.commit("zIndexIncrement", "colorization");
      }, 1);
    },
    showNossaflex(e) {
      e.stopPropagation();
      this.$store.commit("changeActiveWindow", "NOSSAFLEX");
      this.$store.commit("toggleShownNossaflex", true);
      setTimeout(() => {
        this.$store.commit("zIndexIncrement", "noss");
      }, 1);
    },
    dragmove(event) {
      this.x += event.dx;
      this.y += event.dy;
      this.$store.commit("zIndexIncrement", "bio");
    },
    resizemove(event) {
      this.w = event.rect.width;
      this.h = event.rect.height;

      this.x += event.deltaRect.left;
      this.y += event.deltaRect.top;
    },
    dragMouseDown: function (event) {
      event.preventDefault();
      // get the mouse cursor position at startup:
      this.positions.clientX = event.clientX;
      this.positions.clientY = event.clientY;
      document.onmousemove = this.elementDrag;
      document.onmouseup = this.closeDragElement;
    },
    elementDrag: function (event) {
      event.preventDefault();
      this.positions.movementX = this.positions.clientX - event.clientX;
      this.positions.movementY = this.positions.clientY - event.clientY;
      this.positions.clientX = event.clientX;
      this.positions.clientY = event.clientY;
      // set the element's new position:
      this.$refs.draggableContainer.style.top =
        this.$refs.draggableContainer.offsetTop -
        this.positions.movementY +
        "px";
      this.$refs.draggableContainer.style.left =
        this.$refs.draggableContainer.offsetLeft -
        this.positions.movementX +
        "px";
    },
    closeDragElement() {
      document.onmouseup = null;
      document.onmousemove = null;
    },
    minimizeBio(e) {
      e.stopPropagation();
      this.$store.commit("toggleShownBio", false);
      this.$store.commit("changeActiveWindow", "Finder");
    },
    closeBio(e) {
      e.stopPropagation();
      this.$store.commit("toggleCloseBio", false);
      this.$store.commit("toggleShownBio", false);
    },
  },
  mounted: function () {
    // Query the element
    const ele = document.getElementById("container");

    // The current position of mouse
    let x = 0;
    let y = 0;

    // The dimension of the element
    let w = 0;
    let h = 0;

    const mouseDownHandlerRight = function (e) {
      x = e.clientX;

      const styles = window.getComputedStyle(ele);
      w = parseInt(styles.width, 10);

      document.addEventListener("mousemove", mouseMoveHandlerRight);
      document.addEventListener("mouseup", mouseUpHandlerRight);
    };

    const mouseDownHandlerLeft = function (e) {
      x = e.clientX;

      const styles = window.getComputedStyle(ele);
      w = parseInt(styles.width, 10);

      document.addEventListener("mousemove", mouseMoveHandlerLeft);
      document.addEventListener("mouseup", mouseUpHandlerLeft);
    };

    const mouseDownHandlerUp = function (e) {
      y = e.clientY;

      const styles = window.getComputedStyle(ele);
      h = parseInt(styles.height, 10);

      document.addEventListener("mousemove", mouseMoveHandlerUp);
      document.addEventListener("mouseup", mouseUpHandlerUp);
    };

    const mouseDownHandlerDown = function (e) {
      y = e.clientY;

      const styles = window.getComputedStyle(ele);
      h = parseInt(styles.height, 10);

      document.addEventListener("mousemove", mouseMoveHandlerDown);
      document.addEventListener("mouseup", mouseUpHandlerDown);
    };

    const mouseMoveHandlerUp = function (e) {
      // How far the mouse has been moved
      const dy = e.clientY - y;

      // Adjust the dimension of element
      ele.style.height = `${h - dy}px`;
    };

    const mouseMoveHandlerDown = function (e) {
      // How far the mouse has been moved
      const dy = e.clientY - y;

      // Adjust the dimension of element
      ele.style.height = `${h + dy}px`;
    };

    const mouseMoveHandlerRight = function (e) {
      // How far the mouse has been moved
      const dx = e.clientX - x;

      // Adjust the dimension of element
      ele.style.width = `${w + dx}px`;
    };

    const mouseMoveHandlerLeft = function (e) {
      // How far the mouse has been moved
      const dx = e.clientX - x;

      // Adjust the dimension of element
      ele.style.width = `${w - dx}px`;
    };

    const mouseUpHandlerUp = function () {
      // Remove the handlers of `mousemove` and `mouseup`
      document.removeEventListener("mousemove", mouseMoveHandlerUp);
      document.removeEventListener("mouseup", mouseUpHandlerUp);
    };

    const mouseUpHandlerDown = function () {
      // Remove the handlers of `mousemove` and `mouseup`
      document.removeEventListener("mousemove", mouseMoveHandlerDown);
      document.removeEventListener("mouseup", mouseUpHandlerDown);
    };

    const mouseUpHandlerRight = function () {
      // Remove the handlers of `mousemove` and `mouseup`
      document.removeEventListener("mousemove", mouseMoveHandlerRight);
      document.removeEventListener("mouseup", mouseUpHandlerRight);
    };

    const mouseUpHandlerLeft = function () {
      // Remove the handlers of `mousemove` and `mouseup`
      document.removeEventListener("mousemove", mouseMoveHandlerLeft);
      document.removeEventListener("mouseup", mouseUpHandlerLeft);
    };
    // Query all resizers
    const resizersRight = ele.querySelectorAll(".resizer-r");
    const resizersUp = ele.querySelectorAll(".resizer-t");
    const resizersDown = ele.querySelectorAll(".resizer-b");
    const resizersLeft = ele.querySelectorAll(".resizer-l");

    [].forEach.call(resizersRight, function (resizer) {
      resizer.addEventListener("mousedown", mouseDownHandlerRight);
    });

    [].forEach.call(resizersUp, function (resizer) {
      resizer.addEventListener("mousedown", mouseDownHandlerUp);
    });

    [].forEach.call(resizersDown, function (resizer) {
      resizer.addEventListener("mousedown", mouseDownHandlerDown);
    });

    [].forEach.call(resizersLeft, function (resizer) {
      resizer.addEventListener("mousedown", mouseDownHandlerLeft);
    });
  },
};
</script>
