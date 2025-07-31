<script setup lang="ts">
interface Project {
  title: string
  description: string
  technologies: string[]
  status: string
  repositoryLink: string
}
const proyects: Project = [
  {
    title: 'Distro Advisor',
    description:
      'Distro Advisor es una aplicación que te ayuda a descubrir distribuciones de Linux según tus preferencias. Permite explorar y comparar distros basadas en características como arquitectura, entorno de escritorio, sistema base, y más.',
    technologies: ['Vue', 'Spring Boot', 'Go', 'Microservicios'],
    status: 'En proceso',
    repositoryLink: '#',
  },
]
</script>
<template>
  <section class="section">
    <h3>Proyectos</h3>
    <div class="project" v-for="proyect in proyects">
      <h4>{{proyect.title}}</h4>
      <p>{{proyect.description}}</p>

      <div class="tech-list">
        <span class="tech-tag" v-for="tech in proyect.technologies">{{tech}}</span>
      </div>

      <div class="status">{{proyect.status}}</div>

      <p style="margin-top: 15px">
      <a :href="proyect.repositoryLink" class="repo-link">Ver repositorio →</a>
      </p>
    </div>
  </section>
</template>
