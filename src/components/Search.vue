<script>
import axios from 'axios';
import { store } from "../store.js";

export default {
    name: 'Search',
    data() {
        return {
            store,
            archetypes: []
        };
    }
    ,
    methods: {
        getArchetypesFromApi() {
            axios.get('https://db.ygoprodeck.com/api/v7/archetypes.php')
            .then((response) => {
                this.archetypes = response.data
            });
        },
        archetypeSelect() {

        }
    }
    ,
    mounted() {
        this.getArchetypesFromApi();
    }
}
</script>

<template>
    <div class="search">
        <div class="container">
            <select v-model="store.selectedArchetype" @change="$emit('selectedSearch')">
                <option>Choose an archetype</option>
                <option v-for="archetype in archetypes" :value="archetype.archetype_name">
                    {{ archetype.archetype_name }}
                </option>
            </select>
        </div>
    </div>
</template>

<style scoped lang="scss">

    .search {
        background-color: black;
        padding-left: 5px;

        select {
            padding: 5px;
            border: 3px solid #d48f38;
        }
    }

</style>