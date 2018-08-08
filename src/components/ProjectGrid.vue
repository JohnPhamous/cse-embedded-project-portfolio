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
            "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/soccer-pong.jpg",
          contributors: [
            {
              name: "Patrick Tumbucon",
              image:
                "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/patrick.jpg",
              url: "https://patricktumbucon.com"
            },
            {
              name: "Patrick Tumbucon",
              image:
                "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/patrick.jpg",
              url: "https://patricktumbucon.com"
            },
            {
              name: "Patrick Tumbucon",
              image:
                "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/patrick.jpg",
              url: "https://patricktumbucon.com"
            },
            {
              name: "Patrick Tumbucon",
              image:
                "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/patrick.jpg",
              url: "https://patricktumbucon.com"
            },
            {
              name: "Patrick Tumbucon",
              image:
                "http://csebcoe.ucr.acsitefactory.com/sites/g/files/rcwecm756/files/patrick.jpg",
              url: "https://patricktumbucon.com"
            }
          ],
          link: "https://patricktumbucon.com/locus/",
          linkTitle: "Demo"
        }
      ]
    };
  }
};
</script>

<style scoped>
</style>
