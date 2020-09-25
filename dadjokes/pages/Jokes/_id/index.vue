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
    created() {
        
    }
}
</script>

<style

</style>