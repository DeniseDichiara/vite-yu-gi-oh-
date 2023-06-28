<template>
    <div class="container">
        <div class="row p-5 justify-content-evenly cornice">
            <CharacterCard v-for="character in charactersList" 
                :characterImage="character.image"
                :characterName="character.name" 
                :characterArchetype="character.archetype" />
        </div>
    </div>
</template>

<script>
import CharacterCard from './CharacterCard.vue';
import axios from 'axios';

export default {
    name: 'CharacterList',
    data() {
        return {
            charactersList: [],
        }
    },
    components: {
        CharacterCard
    },

    created() {
        axios.get('https://db.ygoprodeck.com/api/v7/cardinfo.php?num=20&offset=0')
            .then((response) => {
                console.log(response.data.data);
                this.charactersList = response.data.data;
            })
            .catch(function (error) {
                console.log(error);
            })
    }
}
</script>


<style lang="scss">
.cornice {
    background-color: white;
}
</style>