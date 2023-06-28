<template>
    <main>
        <div class="container">
            <div class="row">
                <div class="col-12">
                    <div>
                        <CharacterList />
                    </div>
                </div>
            </div>
        </div>
    </main>
</template>

<script>
import CharacterList from './CharacterList.vue';
export default {
    name: 'AppMain',
    data() {
        return {

        }
    },
    components: {
        CharacterList
    }
}
</script>

<style lang="scss">

</style>

