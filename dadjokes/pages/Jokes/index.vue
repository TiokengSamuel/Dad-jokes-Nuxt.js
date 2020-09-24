<template>
    <div>
        Jokes
    </div>
</template>

<script>
    data(){
        return {
            jokes: []
        }
    }
    export default {
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


