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

      <div class="row"> 
        <div class="col-lg-12">
          <h4 style="background-color: black;" class="text-white text-center rounded-1 p-2 m-1">
            Kurikulum <b> SMKN 4 TASIKMALAYA</b>
          </h4>
        </div>
        <main class="content">
          <!-- Breadcrumb -->
          <p style="background-color: honeydew;" class="text-black text-left rounded-1 p-2 m-3">
      <NuxtLink to="/kurikulum/" class="text-decoration-none">kurikulum</NuxtLink>
    </p>
        </main>
      </div>
    </div>

    <!-- Kompetensi Keahlian -->
    <div class="app">
      <div class="kompetensi-card">
        <h1 class="text-center">Kompetensi Keahlian</h1>
        <table class="table table-bordered">
          <thead>
            <tr>
              <th>Ikon</th>
              <th>Keahlian</th>
              <th>Fasilitas</th>
            </tr>
          </thead>
          <tbody>
            <tr v-for="item in kompetensi" :key="item.title">
              <td class="text-center">{{ item.icon }}</td>
              <td>{{ item.title }}</td>
              <td>
                <ul>
                  <li v-for="facility in item.facilities" :key="facility">{{ facility }}</li>
                </ul>
              </td>
            </tr>
          </tbody>
        </table>
        <NuxtLink to="/keahlian/"> 
          <button class="selengkapnya">Selengkapnya</button>
        </NuxtLink>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      kompetensi: [
        {
          title: "Teknik Komputer dan Jaringan",
          icon: "💻",
          facilities: [
            "Bengkel TKJ",
            "Network Simulator",
            "Techno Park",
            "Dll"
          ]
        },
        {
          title: "Rekayasa Perangkat Lunak",
          icon: "🖥️",
          facilities: [
            "Laboratorium Komputer",
            "Computer Server",
            "Techno Park",
            "Dll"
          ]
        },
        {
          title: "Teknik dan Bisnis Sepeda Motor",
          icon: "🔧",
          facilities: [
            "Bengkel TBSM",
            "Unit Produksi",
            "Techno Park",
            "Dll"
          ]
        },
        {
          title: "Desain Komunikasi Visual",
          icon: "🖥️",
          facilities: [
            "Laboratorium Komputer",
            "Computer Server",
            "Techno Park",
            "Dll"
          ]
        },
        {
          title: "Teknik Otomasi Industri",
          icon: "🖥️",
          facilities: [
            "Laboratorium Mekatronik",
            "Terminal Input/Output(i/O)",
            "Sumber Daya Listrik",
            "Dll"
          ]
        },
      ]
    };
  }
};
</script>

<style scoped>
.app {
  font-family: Arial, sans-serif;
  padding: 20px;
}

.kompetensi-card {
  background-color: #f9f9f9;
  border: 1px solid #ddd;
  border-radius: 10px;
  padding: 20px;
  box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

.table {
  width: 100%;
  margin-top: 20px;
  border-collapse: collapse;
}

.table th, .table td {
  border: 1px solid #ddd;
  padding: 10px;
  text-align: left;
}

.table th {
  background-color: #007bff;
  color: white;
}

.selengkapnya {
  margin-top: 20px;
  padding: 10px 20px;
  background-color: #007bff;
  color: white;
  border: none;
  border-radius: 5px;
  cursor: pointer;
}

.selengkapnya:hover {
  background-color: #0056b3;
}
</style>
