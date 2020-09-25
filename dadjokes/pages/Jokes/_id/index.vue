<template>
 
    <div>
        {{ $route.params.id }}
    </div>
</template>

<script>
import axios from 'axios'
export default {
    data() {
        return {
            joke: {}
        }
    },
    async created() {
        const config = {
            headers: {
                Accept : 'application/json'
            }
        }
      try{
        const res = await axios.get('https://icanhazdadjoke.com/search',
         config);
         console.log(res.data);

         this.jokes = res.data.results;

      } catch (err) {
          console.log(err)
      }
    }
}
</script>

<style

</style>