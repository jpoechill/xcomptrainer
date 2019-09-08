<template>
  <div>
    <div class="container">
      <div class="row pb-3">
        <div class="col-md-6">
          xCompTrainer <br>
          jPoechill
        </div>
        <div class="col-md-6 text-right">glory (0): 0</div>
      </div>
      <div class="row">
        <div class="col-md-12">
          <hr class="bg-white">
        </div>
      </div>
      <div class="row">
        <div class="col-md-12 text-white text-center">
          <nuxt-link to="/">Tables</nuxt-link> | 
          <nuxt-link to="/graphs">Graphs</nuxt-link> | 
          <nuxt-link to="/sounds">Sounds</nuxt-link>
        </div>
      </div>
    </div>

    <nuxt-child />

    <div class="container">
      <div class="row">
        <div class="col-md-12">
          Discretion: <br>
          Lorem ipsum, dolor sit amet consectetur adipisicing elit. Expedita tenetur commodi ipsum, non impedit iste molestias veniam quaerat ab accusamus voluptate sit quos illo dolorum?
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style>
a {
  color: #ffffff;
}

/* W/L Tabs */
.tab {
  box-shadow: 1px 1px 1px 1px hsla(0, 0%, 6%, .3);
  transition: all .3s ease-out;
}

.tab:hover {
  box-shadow: 3px 3px 5px 3px rgba(16, 16, 16, .3);
  /* transition: .2s ease-in-out; */
  cursor: pointer;
}

/* Ripple effect */
.ripple-lgt, .ripple-drk {
  background-position: center;
  /* transition: background 0.8s; */
}

.ripple-lgt:hover {
  background: #eee radial-gradient(circle, transparent 1%, #f1f1f1 1%) center/15000%;
}

.ripple-lgt:active {
  background-size: 100%;
  transition: background 0s;
}

.ripple-drk:hover {
  background: #064583 radial-gradient(circle, transparent 1%, #063f77 1%) center/15000%;
}

.ripple-drk:active {
  background-size: 100%;
  transition: background 0s;
}

.bg-blue {
  background-color: #063f77;
}

/* Disable Text Selection */
.noselect {
  -webkit-touch-callout: none; /* iOS Safari */
    -webkit-user-select: none; /* Safari */
     -khtml-user-select: none; /* Konqueror HTML */
       -moz-user-select: none; /* Firefox */
        -ms-user-select: none; /* Internet Explorer/Edge */
            user-select: none; /* Non-prefixed version, currently
                                  supported by Chrome and Opera */
}
</style>
