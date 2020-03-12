<template>
  <div id="programmingSkills">
    <div class="container">
      <div class="row">
        <div class="col-lg-5">
          <div class="illustration">
            <img :src="illustration1" alt="illustration">
          </div>
        </div>
        <div class="col-lg-7">
          <h1 class="section-title">My Programming Skills</h1>
          <SkillPercent skillName="HTML" :percent="90" colorBar="red" />
          <SkillPercent skillName="CSS" :percent="98" colorBar="lightgreen" />
          <SkillPercent skillName="Javascript" :percent="90" colorBar="blue" />
          <SkillPercent skillName="PHP" :percent="80" colorBar="yellow" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>

// Components
import SkillPercent from './SkillPercent.vue'

// Assets
import illustration1 from '../../assets/illustration1.svg'

export default {

  name: 'Portfolio',

  components: {
    SkillPercent
  },

  data () {
    return {
      illustration1
    }
  }
}
</script>

<style lang="css" scoped>

#programmingSkills {
  margin-bottom: 50px;
}

.illustration {
  max-width: 400px;
}

.illustration img {
  width: 100%;
}

.section-title {
  font-size: 32px;
  font-weight: 200;
  margin-bottom: 30px;
}

</style>