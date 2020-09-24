<template>
    <div>
        Jokes
    </div>
</template>

<script>
    
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

        const res = await axios.get();
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


