<template>
    <div id="project-grid">
        <project
            v-for="project in projects"
            :key="project.title"
            :project="project"
        />
    </div>
</template>

<script>
import Project from "./Project";

export default {
  components: {
    Project
  },
  data: function() {
    return {
      projects: [
        {
          title: "Soccer Pong",
          subtitle: "iOS App",
          description:
            "Soccer Pong is an iOS game developed independently by James Luo in his free. The game is a hackey style pong game that supports a global leaderboard and allows for users to play with multiple people locally. Soccer Pong is now available in the App Store for free.",
          image:
            "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/soccer-pong.jpg",
          contributors: [
            {
              name: "James Luo",
              image:
                "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/james.jpg",
              url: "https://jluo117.github.io/"
            }
          ],
          link:
            "https://itunes.apple.com/us/app/soccer-pong-by-acm/id1345533840?ls=1&mt=8",
          linkTitle: "App Store Download"
        },
        {
          title: "Locus",
          subtitle: "Web Application",
          description:
            "Locus is a web application that uses location analytics to help you find the perfect neighborhood. This was created over a weekend during the Esri Intern Hackathon, and I led my team to achieve 2nd place out of 15 teams.",
          image:
            "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/locus.jpg",
          contributors: [
            {
              name: "Patrick Tumbucon",
              image:
                "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/patrick.jpg",
              url: "https://patricktumbucon.com"
            },
            {
              name: "Reed Shoho",
              image:
                "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/reedshoho.jpg",
              url: "#"
            },
            {
              name: "Darlene Dela Rosa",
              image:
                "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/darlenedelarose.jpg",
              url: "https://www.linkedin.com/in/darlene-dela-rosa-027762122/"
            },
            {
              name: "Hector Hernandez",
              image:
                "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/hectorhernandez.jpg",
              url: "https://www.linkedin.com/in/hector-hernandez-617531166/"
            }
          ],
          link: "https://patricktumbucon.com/locus/",
          linkTitle: "Demo"
        },
        {
          title: "Smart RC Car",
          subtitle: "IoT",
          description:
            "1:8th scale RC car that in almost every way replicates a four-wheel drive electric  race car. Custom 32 bit ARM Processor for testing complex driving algorithms, like torque vectoring, traction control, and software wheel differential. Custom 3D Printed Power train, Custom PCBA, and ultrasonic and sonar sensor for collision detection.",
          image:
            "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/Screenshot_2018-08-07%20sammysresume%20Fullscreen%20Page.png",
          contributors: [
            {
              name: "Salvatore Macaluso",
              image:
                "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/sammymaculuso.jpg",
              url: "https://www.sammymacaluso.com/"
            }
          ],
          link:
            "https://www.sammymacaluso.com/fullscreen-page/comp-iqtuyfne/28c0ff75-041b-44a1-ac2c-549d736f0527/6/%3Fi%3D6%26p%3Dihge1%26s%3Dstyle-jhpexs4r",
          linkTitle: "Learn More"
        }
      ]
    };
  }
};
</script>

<style scoped>
</style>
