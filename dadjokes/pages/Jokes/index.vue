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
    created() {

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


