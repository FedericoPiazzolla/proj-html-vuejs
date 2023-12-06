<script>
export default {
  data() {
    return {

    }
  }
}
</script>

<template>
  <section class="bg-section">
    <div class="container">
     <div class="box">
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere eius nostrum ex assumenda vel, voluptatum laboriosam rerum voluptas minus quo nulla possimus praesentium quas sunt quae ipsum asperiores rem perspiciatis.
      </div> 
    </div>
    
  </section>
</template>

<style lang="scss" scoped>
.bg-section {
  background-image: url("../assets/img/avada-movers-movewithease-background-new.jpg");
  background-size: cover;
  background-position: center;

  .container {
    width: 70%;
    max-width: 1100px;
    margin: 0 auto;
    min-height: 500px;
    display: flex;
    flex-direction: row-reverse;
    align-items: center;
    .box {
      width: 50%;
      text-align: center;
      background-color: green;
    }
  }
}
</style>