<template>
    <form>
        <input type="text" v-model="text" placeholder="Search Jokes...">
    </form>
</template>

<script>
export default {
    name: 'SearchJokes',
    data () {
        return{
        text: ''
    }
 }
}
</script>

<styles>

</style>