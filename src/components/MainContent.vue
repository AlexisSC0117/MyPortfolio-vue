<template>
  <main class="content">
    <section>
      <h3>Objective</h3>
      <p>
        A motivated and detail-oriented individual seeking an opportunity to apply programming, problem-solving, and software development skills to create efficient and high-quality applications while continuously learning and growing in a collaborative environment.
      </p>
    </section>

    <section>
      <h3>Character Summary</h3>
      <p>
        A Dedicated Bachelor’s degree holder with Certificates, possessing basic programming skills and a strong desire to grow in the tech industry. Eager to learn new technologies, support development tasks, and contribute positively to organizational goals.
      </p>

      <h3>Certifications</h3>
      <ul>
        <li>Visual Graphics & Design NCIII</li>
        <li>Computer Systems Servicing NCII</li>
        <li>Instrumentation & Control Servicing NCII</li>
        <li>Instrumentation & Control Servicing NCIII</li>
        <li>Electronic Products Assembly and Servicing NCII</li>
        <li>Consumer Electronics Servicing NCIII</li>
      </ul>
    </section>

    <section>
      <h3>Experience</h3>
      <div class="job">
        <h4>Faculty Member — Microcity College of Business and Technology Inc.</h4>
        <p>2025–Present</p>
        <p>Instructor for Computer Engineering Subjects</p>
      </div>
    </section>

    <section>
      <h3>Skills & Tools</h3>

      <div v-for="group in skillGroups" :key="group.title" class="skill-group">
        <h4>{{ group.title }}</h4>

        <div class="skills">
          <span v-for="skill in group.skills" :key="skill">
            {{ skill }}
          </span>
        </div>
      </div>
    </section>
  </main>
</template>

<script setup>
const skillGroups = [
  {
    title: "Website Development",
    skills: [
      "HTML & CSS",
      "C Language",
      "SQL",
      "Vue.js"
    ]
  },
  {
    title: "Graphic Media & 3D Design",
    skills: [
      "Adobe Illustrator",
      "Adobe Photoshop",
      "AutoCAD",
      "SketchUp"
    ]
  },
  {
    title: "AI Integration",
    skills: [
      "ChatGPT",
      "Grok"
    ]
  }
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

.skill-group {
  margin-top: 14px;
}

.skill-group h4 {
  margin-bottom: 8px;
  color: #7dd3fc;
  font-size: 15px;
}

.job {
  padding: 14px;
  background: #020617;
  border-radius: 12px;
  margin-top: 10px;
}

.skills {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(140px, 1fr));
  gap: 10px;
}

.skills span {
  background: #020617;
  padding: 10px;
  border-radius: 10px;
  text-align: center;
  font-size: 14px;
}
</style>
