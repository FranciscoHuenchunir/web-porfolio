<script setup lang="ts">
  const languajes: string =[
  "Java", "Go", "SQL"
  ]
  const Frameworks: string = [
  "Spring Boot"
  ]
  const skillList: string = [
    "Linux", "Bash / Zsh", "Docker", "Bun"
  ]
</script>

<template>

    <section class="section">
      <h3>Habilidades Técnicas</h3>
      <div class="skills-grid">
        <div class="skill-category">
          <h4>Lenguajes</h4>
          <ul class="skill-list">
            <li v-for="item in languajes">{{item}}</li>
          </ul>
        </div>
        <div class="skill-category">
          <h4>Frameworks</h4>
          <ul class="skill-list">
            <li v-for="item in Frameworks">{{item}}</li>
          </ul>
        </div>
        <div class="skill-category">
          <h4>Herramientas y entorno</h4>
          <ul class="skill-list">
            <li v-for="item in skillList">{{item}}</li>
          </ul>
        </div>
      </div>
    </section>

</template>

