<template>
  <div class="container-fluid">
    <div id="app">
      <header class="header">
        <img src="/assets/image/ultah.jpeg" alt="Header Background" class="header-image" />
        <div class="header-overlay"></div>
      </header>
      <div class="row">
        <div class="col-lg-12 p-3"></div>
      </div>
      </div>
      </div>
  <p style="background-color: honeydew;" class="text-black text-left rounded-1 p-2 m-3">
      <NuxtLink to="/galeri" class="text-decoration-none">Galeri</NuxtLink>
    </p>
  <div class="row">
      <div class="col-lg-12">
        <h4 style="background-color: black;" class="text-white text-center rounded-1 p-2 m-4">
          Galeri <b>SMKN 4 TASIKMALAYA</b>
        </h4>
      </div>
    </div>

    <div class="extracurricular-container">
    <div class="extracurricular-grid">
      <div class="activity-card">
        <img src="/assets/image/pramuka.jpeg" alt="Pramuka" class="activity-image" />
        <h2 class="activity-title"><b> Pramuka </b></h2>
      </div>
      <div class="activity-card">
        <img src="/assets/image/pramuka.jpeg" alt="Pramuka" class="activity-image" />
        <h2 class="activity-title"><b> Pramuka </b></h2>
      </div>
      <div class="activity-card">
        <img src="/assets/image/pramuka.jpeg" alt="Pramuka" class="activity-image" />
        <h2 class="activity-title"><b> Pramuka </b></h2>
      </div>
      <div class="activity-card">
        <img src="/assets/image/pramuka.jpeg" alt="Pramuka" class="activity-image" />
        <h2 class="activity-title"><b> Pramuka </b></h2>
      </div>
      </div>
    </div>
  
</template>

<style scoped>
.extracurricular-container {
  padding: 20px;
  font-family: Arial, sans-serif;
  text-align: center;
  background-color: #f9f9f9;
}

h1 {
  color: #333;
  margin-bottom: 20px;
}

.extracurricular-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 20px;
}

.activity-card {
  background: #fff;
  border-radius: 10px;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  overflow: hidden;
  transition: transform 0.3s;
}

.activity-card:hover {
  transform: translateY(-10px);
}

.activity-image {
  width: 100%;
  height: 200px;
  object-fit: cover;
}

.activity-title {
  padding: 10px;
  font-size: 18px;
  color: #555;
}
</style>