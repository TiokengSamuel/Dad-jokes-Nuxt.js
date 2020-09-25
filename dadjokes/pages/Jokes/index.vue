<template>
    <div>
       <Joke v-for="joke in jokes" :key="joke.id"/>
    </div>
</template>

<script>
    import axios from 'axios'
    import Joke from '../../components/Joke'

    export default {
        components: {
            Joke
        },
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


