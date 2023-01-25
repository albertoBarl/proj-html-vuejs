<template lang="">
  <div class="container-fluid">
    <div class="pCenter">
      <h2>Testimonials</h2>
      <h3>Why do people love me?</h3>
    </div>
    <div>
      <div class="slider d-flex">
        <div class="item-slider" v-for="(item, index) in slider">
          <div class="item">
            <img :src="`./img/${slider[index].ref}`" />
          </div>
        </div>
        <!--Pulsanti di navigazione prec e succ del carosello immagini-->
        <div class="circles-container">
          <div class="circle"></div>
          <div class="circle"></div>
          <div class="circle"></div>
          <div class="circle"></div>
          <div class="circle"></div>
        </div>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      slider: [
        {
          ref: "try",
          inside:
            "I am free to learn at my own pace, follow my own schedule and choose the subject I want to learn from the syllabus. Great study portal for people like me.",
          avatar: "AVATAR",
          owner: "Owner",
          job: "Boh",
        },
        {
          ref: "try",
          inside:
            "I need to get a certification for English proficiency and MaxCoach is my best choice. Their tutors are smart and professional when dealing with students.				",
          avatar: "AVATAR",
          owner: "Owner",
          job: "Boh",
        },
        {
          ref: "try",
          inside:
            "I am happy with their arrangement of lessons and subjects. They reflect a scientific  investigation into effective methods to be adopted for learners of all levels.				",
          avatar: "AVATAR",
          owner: "Owner",
          job: "Boh",
        },
        {
          ref: "try",
          inside:
            "I'm a very strict person so I require everything to be organized and neat. Then, I'll be able to make things right and shine. MaxCoach guys just got me.				",
          avatar: "AVATAR",
          owner: "Owner",
          job: "Boh",
        },
      ],
    };
  },
};
</script>
<style lang="scss" scoped>
@use "../../styles/generals.scss" as *;
@use "../../styles/partials/mixins" as *;
@use "../../styles/partials/variables" as *;

.pCenter {
  display: flex;
  flex-direction: column;
  align-items: center;
  h3 {
    width: 75%;
    text-align: center;
    font-weight: 500;
  }
  h2 {
    font-family: cursive;
    font-style: italic;
    font-size: 40px;
    color: $cielo;
  }
}

.slider {
  width: 50vw;
  height: 50vh;
  position: relative;
}

.item {
  display: none;
}

.item-slider,
.item,
img {
  height: 100%;
}

.item img {
  width: 100%;
  object-fit: cover;
}

.item.active {
  display: block;
}

.circles-container {
  display: flex;
  justify-content: center;
}

.circle {
  display: inline-block;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background-color: rgba(174, 174, 174, 0.509);
  margin: 10px;
  cursor: pointer;
}

.circle.active,
.circle:hover {
  background-color: rgba(174, 174, 174, 1);
}

.hidden {
  display: none;
}
</style>
