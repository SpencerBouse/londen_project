<template>
  <div class="row about-section margin-top animated fadeIn">
    <div class="col-md-4">
      <div class="headers">
        <h2>About</h2>
        <h1>Chris Londen</h1>
      </div>
    </div>

    <div class="col-md-8">
        <div class="abouttext">
          <p>
          Chris Londen is an American-born singer/songwriter who uses Pop, Rock, R&amp;B, Hip-Hop, and Latin
          influences to create unique musical experiences for all to enjoy. His original debut E.P. features vocal
          and instrumental sounds that span genres and challenge industry norms, entitled “3 am.” The intention
          of creating this unique sound, while also being marketable to a wide range of audiences, is the
          cornerstone to his success. Chris Londen is credited not only for his lead and harmony vocals on every
          song of “3 am,” but for the lyrics and creative direction of the project, as a whole.
          He began writing music when he was just 12 years old, as a young visionary, in Virginia Beach, VA. He
          spent his childhood learning music video choreography, taking vocal lessons, writing songs, and
          performing at events in his local area. Here, the music influence in his life exploded, as he was
          introduced to Hip-Hop and R&amp;B music, after growing up strictly on Country music. After he and his
          family moved from Virginia Beach, VA at the age of 16, he took his influences from Virginia-based artists
          Pharrell, Missy Elliott, and Timbaland to the Queen City: Cincinnati, OH. Here, he experienced a major
          culture shock, recognizing that the mid-west way of life was vastly different than that of the east coast.
          This inspired him, progressively more, to begin pursing music styles that differed from that of even
          American-born artists. The melodic impact of many Latin artists, blending with the new wave of the
          current-day British invasion of music in the United States, set the stage for him to challenge himself to
          grow with market trends in music like never-before.
          The first song Chris Londen ever recorded, “Time of Your Life,” is on his debut E.P. His partnership with
          master-class Producer and Sound Engineer, Tony “2Tone” Burkhart of Blacklite Productions, allowed for
          a freedom of unbridled creativity, sonic experimentation, and innovation to bring about how Chris
          Londen speaks through music and connects to listeners, even on an international scale. Chris Londen
          also wrote a track entitled “Streets Have No Names” for the non-profit South African organization, Build
          The Future. After his time serving on the ground in Johannesburg, South Africa, he felt compelled to
          give back the only way he knew how: music. Chris has also performed in London, England; Dublin,
          Ireland; and Cape Town, South Africa for various audiences. He foresees a bright future of success in the
          music industry, hoping to contribute legendary pieces of work that will change the landscape of music
          and blend audiences of multiple types, celebrating diversity, originality, and collaboration.
        </p>
        </div>
      </div>
    </div>


  </div>
</template>

<script>
export default {
  name: 'AboutContent'
}
</script>

<style lang='scss'>
  @import '../../src/assets/sass/now-ui-kit.scss';

  .about-section{
    padding: 1em;
    background-color: white;
    opacity: 0.2;
    color: black;
    .headers {
      text-align: center;
    }
    .abouttext{
      margin-right: 0;
    }
    h1{
      color: purple;
      margin: 0;
      font-weight: 800;
    }
    h2{
      color: black;
      margin: 0;
    }
    p{
      color: black;
    }
    @media (min-width: $screen-sm-min) {
      background-image: linear-gradient(to bottom, rgba(255, 255, 255, 0.9) 0%,rgba(255, 255, 255, 0.6) 100%), url('/static/img/Londen.jpg');
      .headers {
        text-align: right;
      }
      .abouttext{
        margin-right: 20%;
      }
    }
    @media (min-width: $screen-md-min) {

    }
    @media (min-width: $screen-lg-min) {

    }

  }
</style>
