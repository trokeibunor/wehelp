<template>
  <div class="wrapper w-screen">
    <nav-bar />
    <section class="hero w-screen">
      <h1>Ready to start your journey</h1>
    </section>
    <section class="whContent">
      <div class="whDisplay">
        <div class="intro_text">
          <h1>Other people's story</h1>
          <p>
            We are a group of individuals that share common ground as you do, we
            understand your fears and frustration, join us to start
          </p>
        </div>
        <div class="image_grid">
          <img src="../static/images/top_image.png" alt="" srcset="" />
          <div class="down_row">
            <img src="../static/images/down_first.png" alt="" />
            <div class="right_col">
              <img src="../static/images/right_img.png" alt="" srcset="" />
              <button>Watch more</button>
            </div>
          </div>
        </div>
        <div class="theTalk">
          <h3>
            “It’s not that some people have will power and some don’t. it’s that
            some people are ready to change”
          </h3>
        </div>
        <div class="whSecDisplay">
          <div class="explain_grid">
            <div class="theText">
              <h4>The RoadMap</h4>
              <p>
                We are a group of individuals that share common ground as you
                do, we understand your fears and frustration, join us to start
              </p>
              <button>Join Today</button>
            </div>
            <div class="theExplanation">
              <div class="expBox">
                <img src="../static/images/sign_up.png" alt="" srcset="" />
                <div class="expCon">
                  <h5>Sign Up</h5>
                  <p>It doesn't take anything to Sign up</p>
                </div>
              </div>
              <div class="expBox">
                <img src="../static/images/set_up.png" alt="" srcset="" />
                <div class="expCon">
                  <h5>Set Up meeting Dates</h5>
                  <p>It doesn't take anything to Sign up</p>
                </div>
              </div>
              <div class="expBox">
                <img src="../static/images/learning.png" alt="" srcset="" />
                <div class="expCon">
                  <h5>Keep Learning</h5>
                  <p>It doesn't take anything to Sign up</p>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div class="theTalk">
          <h3>
            “ The fears will come, the not-so worthy syndrome will be there but
            persistence is devour all ”
          </h3>
        </div>
      </div>
      <div class="accolades">
        <div class="acc_cont">
          <div class="acc_box">
            <h5>1000</h5>
            <p>Enrolled Candidates</p>
          </div>
          <div class="acc_box">
            <h5>95%</h5>
            <p>Success rate</p>
          </div>
          <div class="acc_box">
            <h5>850</h5>
            <p>Graduated Candidates</p>
          </div>
        </div>
      </div>
      <div class="meetTeam"></div>
    </section>
  </div>
</template>

<script>
import NavBar from '../components/NavBar.vue'
export default {
  name: 'IndexPage',
  components: {
    NavBar,
  },
}
</script>
<style lang="scss">
.wrapper {
  background-image: url('../static/images/hero_background.png'),
    url('../static/images/background.png');
  height: auto;
}
.hero {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  height: 75vh;
  h1 {
    text-align: center;
    margin: 0 auto;
    width: 60%;
    font-weight: bolder;
    font-size: 80px;
  }
}
.whContent {
  border-radius: 600px 600px 0px 0px;
  background: linear-gradient(
    #fff,
    hsl(173, 81%, 94%),
    hsl(236, 76%, 92%),
    hsl(41, 100%, 94%),
    hsl(173, 94%, 87%),
    hsl(235, 83%, 88%)
  );
  // hsl(43, 91%, 86%)
  // opacity: 0.5;
  color: #000;
  height: auto;
  filter: blur(0px);
  .whDisplay {
    width: 80%;
    margin: 0 auto;
    padding: 4rem 0px 1rem 0px;
    display: flex;
    flex-direction: column;
    .intro_text {
      margin: 0 auto;
      width: 60%;
      text-align: center;
      h1 {
        color: #000;
        font-size: 48px;
      }
      p {
        font-family: 'Montserrat', sans-serif;
      }
    }
    .image_grid {
      width: 80%;
      margin: 4rem auto 2rem auto;
      display: flex;
      flex-direction: column;
      gap: 32px;
      .down_row {
        display: grid;
        grid-gap: 16px;
        grid-template-columns: 1fr 1fr;
        .right_col {
          display: flex;
          flex-direction: column;
          justify-content: space-between;
          button {
            background-color: #3d92a2;
            color: #fff;
            font-family: 'Montserrat', sans-serif;
            width: fit-content;
            height: fit-content;
            padding: 8px 24px;
            border: 1px solid #fff;
            border-radius: 8px;
          }
        }
      }
    }
    .theTalk {
      width: 70%;
      margin: 2rem auto 2px;
      font-size: 42px;
      text-align: center;
      line-height: 100%;
    }
    .whSecDisplay {
      width: 80%;
      padding: 3rem 0px;
      margin: 0 auto;
      .explain_grid {
        display: grid;
        grid-template-columns: 40% 1fr;
        justify-items: flex-end;
        align-items: center;
        .theText {
          h4 {
            font-size: 42px;
            margin: 1rem 0px;
          }
          p {
            margin-bottom: 4rem;
          }
          button {
            background-color: #3d92a2;
            color: #fff;
            font-family: 'Montserrat', sans-serif;
            width: fit-content;
            height: fit-content;
            padding: 8px 24px;
            border: 1px solid #fff;
            border-radius: 8px;
          }
        }
        .theExplanation {
          display: flex;
          flex-direction: column;
          .expBox {
            display: flex;
            flex-direction: row;
            margin: 2rem 0px;
            align-items: center;
            gap: 8px;
            .expCon {
              display: flex;
              flex-direction: column;
              h5 {
                font-weight: bold;
              }
            }
          }
        }
      }
    }
  }
  .accolades {
    background-image: url('../static/images/acc_background.svg');
    background-repeat: no-repeat;
    // background-size: fill;
    width: 100%;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 4rem 0px;
    color: #fff;
    height: 70vh;
    .acc_cont {
      display: flex;
      flex-direction: row;
      width: 100%;
      margin: 0px auto;
      justify-content: space-around;
      align-items: center;
      .acc_box {
        text-align: center;
        h5 {
          font-size: 30px;
        }
      }
    }
  }
  .meetTeam {
    height: 20vh;
  }
}
</style>
