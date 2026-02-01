<template>
  <main class="content">
    <section>
      <h3>Objective</h3>
      <p>
        Passionate software developer seeking to build modern, scalable, and
        high-performance applications.
      </p>
    </section>

    <section>
      <h3>Career Summary</h3>
      <ul>
        <li>5+ years in Web Development</li>
        <li>Vue, React, Node, Laravel experience</li>
        <li>Strong UI/UX and performance optimization</li>
      </ul>
    </section>

    <section>
      <h3>Experience</h3>
      <div class="job">
        <h4>Frontend Developer — Company</h4>
        <p>2022 – Present</p>
        <p>Built responsive Vue apps and optimized UX.</p>
      </div>
    </section>

    <section>
      <h3>Skills & Tools</h3>
      <div class="skills">
        <span v-for="skill in skills" :key="skill">{{ skill }}</span>
      </div>
    </section>
  </main>
</template>

<script setup>
const skills = [
  "Vue",
  "React",
  "JavaScript",
  "Node.js",
  "Tailwind",
  "Figma",
  "MongoDB",
  "Git"
]
</script>

<style scoped>
.content {
  background: #0f172a;
  padding: 28px;
  border-radius: 18px;
}

section {
  margin-bottom: 24px;
}

h3 {
  margin-bottom: 10px;
  color: #38bdf8;
}

.job {
  padding: 14px;
  background: #020617;
  border-radius: 12px;
  margin-top: 10px;
}

.skills {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(120px, 1fr));
  gap: 10px;
}

.skills span {
  background: #020617;
  padding: 10px;
  border-radius: 10px;
  text-align: center;
}
</style>
