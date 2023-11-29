<template>
  <div id="app">
    <header>
      <h1>CHOCOMOON</h1>
      <p>Bienvenido a Chocomoon, tu destino para deleitar tus sentidos con exquisitos chocolates y delicias artesanales. 
      En Chocomoon, nos enorgullece ofrecer una amplia variedad de productos de alta calidad, desde indulgentes tabletas 
      de chocolate amargo hasta suaves trufas de caramelo salado. Nuestro compromiso con la excelencia y la creatividad nos impulsa a crear experiencias únicas para tu paladar.</p>
    </header>
    <main>
      <ProductosComponent />
    </main>
    <footer class="footer">
      <p>© 2023 CHOCOMOON</p>
      <p>Todos los derechos reservados</p>
      <p>Email: info@chocomoon.com</p>
    </footer>
  </div>
</template>

<script>
import ProductosComponent from "@/components/ProductosComponent.vue";

export default {
  components: {
    ProductosComponent,
  },
};
</script>


<style>
header {
    text-align: center;
    background-color: #292b2c; 
    color: #ffffff; 
    padding: 20px;
  }

  h1 {
    font-size: 2.5em; 
    margin-bottom: 10px; 
  }

  p {
    font-size: 1.2em; 
    line-height: 1.5;
  }

  .footer {
  text-align: center;
  padding: 10px;
  background-color: #333; 
  color: #fff; 
}

.footer p{
  font-size: 1.2em; 
    line-height: 1; 
}
</style>
 