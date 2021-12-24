<template>
  <div class="entry-container mb-3 pointer p-2" @click="$router.push({name: 'entry', params: {id: 10}})">

      <!-- Titulo -->
      <div class="entry-title d-flex">

          <span class="text-success fs-5 fw-bold">15</span>
          <span class="mx-1 fs-5">Julio</span>
          <span class="mx-1 fs-4 fw-light">2021, jueves</span>

      </div>

      <div class="entry-descrption">
          Do anim eiusmod consectetur pariatur culpa laborum deserunt reprehenderit consectetur adipisicing anim. Sunt do Lorem aliquip labore fugiat sunt sit. Consectetur elit velit esse consectetur adipisicing minim magna anim non proident laboris. Esse eu minim enim in officia. Nostrud quis esse sunt nulla cillum dolore eu magna minim. Proident magna officia aute pariatur cupidatat cillum officia amet sint aliquip ad amet eiusmod. Consequat pariatur elit magna incididunt deserunt incididunt.
      </div>

  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    .entry-container{
        border-bottom: 1px solid #2c3e50;
        transition: 0.2s all ease-in;

        &:hover{
            background: lighten($color: grey, $amount: 45);
            transition: 0.2s all ease-in;
        }
        .entry-descrption{

            font-size: 12px;
        
        }
    }

</style>