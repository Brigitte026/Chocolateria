<template>
  <div class="productos">
    <h2>NUESTROS PRODUCTOS</h2>
    <div class="galeria">
      <div v-for="producto in productos" :key="producto.id" class="producto">
        <img :src="producto.imagen" :alt="producto.nombre" class="producto-imagen">
        <div class="producto-info">
          <h3>{{ producto.nombre }}</h3>
          <p>{{ producto.descripcion }}</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      productos: [
        {
          id: 1,
          nombre: "Tableta de Chocolate Amargo",
          descripcion: "Deliciosa tableta de chocolate amargo con un alto contenido de cacao.",
          imagen: "/img/imagen1.jpg",
        },
        {
          id: 2,
          nombre: "Bombones de Frambuesa",
          descripcion: "Bombones rellenos de ganache de chocolate y frambuesa.",
          imagen: "/img/imagen2.jpg",
        },
        {
          id: 3,
          nombre: "Trufas de Caramelo Salado",
          descripcion: "Trufas suaves de chocolate rellenas de caramelo salado.",
          imagen: "/img/imagen3.jpg",
        },
        {
          id: 4,
          nombre: "Chocolate Caliente Gourmet",
          descripcion: "Mezcla de chocolate en polvo para preparar un chocolate caliente de alta calidad.",
          imagen: "/img/imagen4.jpg",
        },
        {
          id: 5,
          nombre: "Caja de Regalo Especial",
          descripcion: "Caja elegante con una selección variada de chocolates para regalo.",
          imagen: "/img/imagen5.jpg",
        },
        {
          id: 6,
          nombre: "Tableta de Chocolate con Almendras",
          descripcion: "Tableta de chocolate con trozos de almendras tostadas.",
          imagen: "/img/imagen6.jpg",
        },
        {
          id: 7,
          nombre: "Trufas de Chocolate Blanco",
          descripcion: "Trufas suaves de chocolate blanco con un toque de vainilla.",
          imagen: "/img/imagen7.jpg",
        },
        {
          id: 8,
          nombre: "Chocolate con Naranja y Jengibre",
          descripcion: "Tableta de chocolate con sabores vibrantes de naranja y jengibre.",
          imagen: "/img/imagen8.jpg",
        },
        {
          id: 9,
          nombre: "Chocolates de Maracuyá",
          descripcion: "Chocolates rellenos con ganache de maracuyá para un toque tropical.",
          imagen: "/img/imagen9.jpg",
        },
        {
          id: 10,
          nombre: "Tableta de Chocolate con Canela",
          descripcion: "Tableta de chocolate con notas cálidas de canela.",
          imagen: "/img/imagen10.jpg",
        },
        {
          id: 11,
          nombre: "Barra de Chocolate con Avellanas",
          descripcion: "Barra de chocolate con trozos de avellanas tostadas.",
          imagen: "/img/imagen11.jpg",
        },
        {
          id: 12,
          nombre: "Chocolate Blanco con Fresas",
          descripcion: "Tableta de chocolate blanco con trozos de fresas deshidratadas.",
          imagen: "/img/imagen12.jpg",
        },
      ],
    };
  },
};
</script>

<style scoped>
.productos {
  background: #007991;
  background: -webkit-linear-gradient(to right, #78ffd6, #007991);
  background: linear-gradient(to right, #78ffd6, #007991);
  text-align: center;
  padding: 20px;
}

.galeria {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  gap: 1rem;
}

.producto {
  box-sizing: border-box;
  overflow: hidden;
  border: 3px solid #ddd;
  display: flex;
  flex-direction: column;
  background: #E4F5F3; 
  border-radius: 8px; 
  padding: 20px; 
  transition: transform 0.3s, box-shadow 0.3s;
}

.producto:hover {
  transform: scale(1.05);
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

.producto-imagen {
  width: 100%;
  height: auto;
}

.producto-info {
  padding: 10px;
  flex-grow: 1;
}


</style>
