<template>
    <div>
        Jokes
    </div>
</template>

<script>
    import axios from 'axios'

    export default {
    data() {
        return {
            jokes: []
        }
    },
    async created() {
        const config = {
            headers: {
                'Accept' : 'application/json'
            }
        }
      try{
        const res = await axios.get('https://icanhazdadjoke.com/search',
         config);
         console.log(res.data);
         this.joke = res.data.resulsts;
      } catch (err) {
          console.log(err)
      }
    },
     head() {
        return {
            title: 'Dad jokes',
            meta:[
                {
                   hid: 'description',
                    name: 'description',
                    content: 'Best place for corny dad jokes'
                 }
                    
                ]
            }
         }    
        };
    </script>

    <style>

    </style>


