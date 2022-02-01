<template>
  <div id="app">
    <div class="container">
      <h1>Tabla de Usuarios</h1>
      <table class="table">
        <thead>
          <tr>
            <th scope="col">#</th>
            <th scope="col">Nombre</th>
            <th scope="col">Apellido</th>
            <th scope="col">RUN</th>
            <th scope="col">Nacimiento</th>
            <th scope="col">Edad</th>
          </tr>
        </thead>
        <tbody>
          <tr v-for="(persona, index) in personas" :key="index">
            <th scope="row">{{ index + 1 }}</th>
            <td>{{ persona.nombre }}</td>
            <td>{{ persona.apellido }}</td>
            <td>{{ persona.rut }}</td>
            <td>{{ persona.fechaNacimiento }}</td>
            <td>{{ persona.edad }}</td>
          </tr>
        </tbody>
      </table>
    </div>
  </div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      personas: [
        {
          id: "61f9a6773986f8d83d7e82ad",
          nombre: "Pennington",
          apellido: "Gregory",
          edad: 34,
          fechaNacimiento: "10-06-2021",
          rut: "23.942.203-9",
        },
        {
          id: "61f9a67784664575ea11b681",
          nombre: "Tracey",
          apellido: "Copeland",
          edad: 24,
          fechaNacimiento: "23-09-2014",
          rut: "27.358.939-2",
        },
        {
          id: "61f9a6771f486dee37c65500",
          nombre: "Hallie",
          apellido: "Mckinney",
          edad: 31,
          fechaNacimiento: "27-12-2020",
          rut: "30.822.125-3",
        },
        {
          id: "61f9a67782b9d568f57545c6",
          nombre: "Alexander",
          apellido: "Webb",
          edad: 35,
          fechaNacimiento: "08-08-2015",
          rut: "19.981.104-5",
        },
        {
          id: "61f9a6774c2f3f887919e5b9",
          nombre: "Roach",
          apellido: "Acevedo",
          edad: 25,
          fechaNacimiento: "24-10-2016",
          rut: "16.100.511-8",
        },
      ],
    };
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
