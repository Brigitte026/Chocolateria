<template>
  <div>
    <h2>Menú</h2>
    <ul>
      <li><a href="#inicio">Inicio</a></li>
      <li><a href="#productos">Productos</a></li>
      <li><a href="#contacto">Contacto</a></li>
    </ul>
  </div>
</template>


<script>
// Lógica del componente aquí
export default {
  name: 'MenuComponent',
  // otras configuraciones
};
</script>

<style scoped>
.menu-container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
  background-color: #f0f0f0; /* Color de fondo de la barra del menú */
}

.menu {
  display: flex;
  list-style-type: none;
  margin: 0;
  padding: 0;
}

.menu li {
  margin-right: 20px;
}

</style>
