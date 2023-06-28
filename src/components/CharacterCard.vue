<template>
    <article class="card mb-3 col-2 me-3">
        <img src="https://images.ygoprodeck.com/images/cards/34541863.jpg" class="card-img-top" alt="...">
        <div class="card-body">
            <h5 class="card-title">
                {{ name }}
            </h5>
            <p class="card-text">
                Alien
            </p>
        </div>
    </article>
</template>

<script>
export default {
    name: 'CharacterCard',
    data() {
        return {

        }
    },
    props:{
        image : String,
        name : String,
        archetype : String,
    }
}
</script>


<style lang="scss"></style>