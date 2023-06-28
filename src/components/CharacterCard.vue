<template>
    <article class="card mb-3 col-2 me-3">
        <img src="https://images.ygoprodeck.com/images/cards/34541863.jpg" class="card-img-top" alt="...">
        <div class="card-body color">
            <h5 class="card-title">
                {{ name }}
            </h5>
            <p class="card-text">
                {{ archetype }}
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


<style lang="scss">
    .color{
        background-color:  #d48f38;
    }
</style>