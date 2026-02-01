<template>
  <aside class="card">
    <img class="avatar" src="/profile.jpg" />

    <h2>Ron Alexis Violenta Dela Cruz</h2>
    <h3>Bachelor's Degree - Computer Engineering</h3>

    <div class="info">
      <p>📍 Orani, Bataan</p>

      <p>
        📧 
        <a href="mailto:Ronalexisdelacruz2003@gmail.com">
          Ronalexisdelacruz2003@gmail.com
        </a>
      </p>

      <p>💼 Applying for Junior Developer Position</p>
    </div>

    <!-- DOWNLOAD CV -->
    <a href="/MyPortfolio-vue/RADC.pdf" target="_blank">
      <button class="btn">Download CV</button>
    </a>

    <!-- SEND EMAIL -->
    <a href="https://mail.google.com/mail/?view=cm&to=Ronalexisdelacruz2003@gmail.com" target="_blank">
      <button class="btn email">Send Email</button>
    </a>

    <!-- FACEBOOK CONTACT -->
    <a href="https://www.facebook.com/Ronalexis.03" target="_blank">
      <button class="btn facebook">Contact on Facebook</button>
    </a>

    <!-- MY PROJECTS -->
    <a href="https://drive.google.com/drive/folders/1-DGVMCG0YQQLtXkl1NR23pYq7kc8NP9i?usp=drive_link" target="_blank">
      <button class="btn projects">My Projects</button>
    </a>

  </aside>
</template>

<style scoped>
.card {
  background: #0f172a;
  padding: 24px;
  border-radius: 18px;
  text-align: center;
  box-shadow: 0 10px 30px rgba(0,0,0,.4);
}

.avatar {
  width: 120px;
  height: 120px;
  border-radius: 50%;
  object-fit: cover;
  margin-bottom: 12px;
}

.info p {
  font-size: 14px;
  color: #cbd5f5;
}

.btn {
  display: block;
  width: 100%;
  margin-top: 12px;
  padding: 10px 14px;
  background: linear-gradient(135deg, #6366f1, #22d3ee);
  border: none;
  color: white;
  border-radius: 10px;
  cursor: pointer;
  transition: transform 0.1s ease, opacity 0.2s ease;
}

.btn:hover {
  transform: scale(1.02);
  opacity: 0.9;
}

/* Email button */
.email {
  background: linear-gradient(135deg, #22c55e, #4ade80);
}

/* Facebook button */
.facebook {
  background: linear-gradient(135deg, #1877f2, #60a5fa);
}

/* Projects button */
.projects {
  background: linear-gradient(135deg, #f59e0b, #fbbf24);
}

/* Email & Facebook links style */
.info a {
  color: #60a5fa;
  text-decoration: none;
  font-weight: 500;
}

.info a:hover {
  text-decoration: underline;
}
</style>
