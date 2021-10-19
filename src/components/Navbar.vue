<template>
  <div>
    <div id="nav">
      <router-link id="logo-url" to="/">
        <img id="logo" :src="logo" :alt="alt">
      </router-link>
      <router-link to="/">Fazer Pedido</router-link>
      <router-link to="/pedidos">Pedidos</router-link>
    </div>
  </div>
</template>

<script>
export default {
  name: "Navbar",
  props: ["logo", "alt"]
}
</script>

<style scoped>
  #nav {
    background-color: #222;                              /* cor de fundo*/
    border-bottom: 4px solid #111;                       /* borda em baixo*/
    padding: 15px 50px;                                    /* laterais */
    display: flex;                                         /*  */
    justify-content: flex-end;                             /* para direira*/
    align-items: center;                                  /* à direita e na vertical*/
  }
  #nav #logo-url {
    margin: auto; /* */
    margin-left: 0;
  }
  #logo {
    width: 40px;                                          /*altura*/
    height: 40px;                                         /*largura*/
  }
  #nav a {
    color: #fcba03;                                     /*cor do texto*/
    text-decoration: none; 
    margin: 12px;                                         /*afastaemnto entre eles*/
    transition: .5s;                                      /*transição, quando o controle do mouse passa sobre ele*/
  }
  #nav a:hover {
    color: #FFF;
  }
</style>