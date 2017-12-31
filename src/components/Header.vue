<template>
  <div class="hello">
      <div>Hi <span>👋</span></div>
      <h1>I’m {{name}}</h1>
      <div>{{msg}}</div>
      <ul id="social">
        <li v-bind:key="s.icon" v-for="s in social">
          <a :href="s.url"><i :class="'fa fa-'+s.icon" aria-hidden="true"></i></a>
        </li>
      </ul>
  </div>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      name: "Nicolas Ferro",
      msg: "A developer from Buenos Aires, Argentina",
      social: [
        { icon: "github", url: "https://github.com/nikoferro" },
        { icon: "linkedin", url: "https://github.com/nikoferro" }
      ]
    };
  }
};
</script>

<style lang="css" scopped>
#social {
  margin: 0px;
  padding: 0px;
}
#social li {
  list-style: none;
  display: inline-block;
  margin: 1em;
  font-size: 24px;
}
#social li a {
  color: #2c3e50;
  transition: opacity 0.2s;
}
#social li a:hover {
  opacity: 0.5;
}
</style>
