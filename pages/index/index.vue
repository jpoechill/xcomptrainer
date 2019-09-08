<template>
    <div class="container pt-2">
      <div v-for="n in 4" :key="n" class="row">
        <div class="col-md-4 my-3">
          <div class="tab bg-blue ripple-drk noselect text-center text-uppercase p-2 rounded font-weight-bold">
            Loss
          </div>
          <div class="w-100">
            <div class="d-inline-block text-white float-right">
              + 
            </div>
          </div>
        </div>
        <div class="col-md-4 my-3">
          <div class="tab bg-light text-dark noselect ripple-lgt text-center text-uppercase p-2 rounded font-weight-bold">
            Win
          </div>
          <div class="w-100">
            <div class="d-inline-block text-white float-right">
              + 
            </div>
          </div>
        </div>
        <div class="col-md-4 my-3">
          <div class="tab bg-blue ripple-drk noselect text-center text-uppercase p-2 rounded font-weight-bold">
            Loss
          </div>
          <div class="w-100">
            <div class="d-inline-block text-white float-right">
              + 
            </div>
          </div>
        </div>
      </div>
    </div>
</template>

<script>
export default {

}
</script>

<style>

</style>