<template>
<article class="special">
  <div>
  <b-card
    title="Summer Special"
    img-top
    tag="article"
    style="max-width: 14rem;"
    class="mb-2"
 >
 <b-card-text>
    </p>Join us as the sun goes down for a refreshing margarita at half price.</p> <p> <b>Today's sunset is at {{results.sunset}} (UTC).</b></p>
    </b-card-text>
      <b-button href="/menu" variant="primary">See More</b-button>
  </b-card>
</div>
    </article>
</template>


<script>
import axios from 'axios'
export default {
  data() {
    return{
      loading: true,
      results: null,
      results: [],
      errored: false,
    };
  },
  mounted () {
    axios.get('https://api.sunrise-sunset.org/json?lat=47.608013&lng=-122.335167&date=today')
   .then(response => {
     console.log(response.data);
     (this.results = response.data.results)
 })
   .catch(error => {
       console.log(error)
       this.errored = true
   })
   .finally(() => this.loading = false)
 }
}
</script>

<style scoped>
.btn {
  padding: .5rem;
  margin: .5rem;
  border-radius: 2px;
  background-color: gray;
  color: white;
  font-style: bold;
}
.special{
  margin: 3rem;
}
</style>
