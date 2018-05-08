<template>
    <div class="navbar">
        <h2>Kenneth Jorgensen</h2>
        <div class="buttons">
            <button class="btn btn-light">Home</button>
            <button class="btn btn-light">Bio</button>
            <button class="btn btn-light">Contact</button>
        </div>
    </div>
</template>

<script>
    export default {
        name: 'Navbar',
        data() {
            return {

            }
        }
    }
</script>

<style scoped>
    .navbar {
        min-height: 15vh;
        background-color: silver;
        display: flex;
        justify-content: space-between;
        color: #2c3e50
    }

    .btn {
        font-weight: 700;
        color: #2c3e50;
        margin: 1rem
    }

    .buttons {
        display: flex;
        justify-content: space-around;
    }
</style>