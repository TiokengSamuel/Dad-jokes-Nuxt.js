<template>
    <h1 class="title">Dad Jokes</h1>
    <ul>
        <li>
            <Nuxt-link to='/'>Home</Nuxt-link>
        </li>
        <li>
            <Nuxt-link to='/jokes'>Jokes</Nuxt-link>
        </li>
        <li>
            <Nuxt-link to='/about'>About</Nuxt-link>
        </li>
    </ul>
</template>

<script>
export default {
    name: 'AppHeader'
}
</script>

<style>
    .header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 1rem;
        border-bottom: 1px dotted #ccc;
    }

    .header .title {
        font-size: 3rem;
        color: #526488;
    }

    .header ul {
        display: flex;
    }

    .header a {
        display: inline-block;
        background: #333;
        color: #fff;
        padding: 0.3rem 1rem;
        margin-right: 0.5rem;
    }
</style>