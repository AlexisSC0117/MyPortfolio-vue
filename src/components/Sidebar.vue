<template>
  <aside class="card">
    <img class="avatar" src="./profile.jpg" />

    <h2>Ron Alexis Violenta Dela Cruz</h2>
    <h3>Bachelor's Degree - Computer Engineering</h3>

    <div class="info">
      <p>📍 Orani, Bataan</p>
      <p>📧 Ronalexisdelacruz2003@gmail.com</p>
      <p>💼 Applying for Junior Developer Position</p>
    </div>

    <a href="./RADC.pdf" download target="_blank">
      <button class="btn">Download CV</button>
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

.role {
  color: #94a3b8;
  margin-bottom: 12px;
}

.info p {
  font-size: 14px;
  color: #cbd5f5;
}

.btn {
  margin-top: 16px;
  padding: 10px 14px;
  background: linear-gradient(135deg, #6366f1, #22d3ee);
  border: none;
  color: white;
  border-radius: 10px;
  cursor: pointer;
}
</style>
