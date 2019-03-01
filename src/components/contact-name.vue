<template>
    <div class="contact-info mb-2">
        <span>{{ name }}</span>
    </div>
</template>

<script>
export default {

    data() {
        return {
            name: "LUCAS HUGDAHL"
        }
    }
}
</script>

<style lang="scss">
    .contact-info { 
        span {
            color: white;
            padding: 0.2% 1.5% 0.2% 1.5%;
            background-color: black;
            font-size: 16px;
            letter-spacing: 3px;
        }
    }
</style>