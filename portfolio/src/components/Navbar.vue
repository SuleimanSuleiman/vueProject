<template>
    <v-app-bar dark color="#111111" flat class="px-8" >
        <v-btn icon>
            <v-icon color="#A7121D">fas fa-dragon</v-icon>
        </v-btn>
        <v-spacer></v-spacer>
        <v-btn text @click="scroll('Home')">Home</v-btn>
        <v-btn text @click="scroll('Project')">Project</v-btn>
        <v-btn text @click="scroll('About')">About</v-btn>
        <v-btn text @click="scroll('Contect')">Contect</v-btn>
        <router-link class="s white--text" to="/Help" exact >
                <a href class="lin">About</a>
        </router-link>
    </v-app-bar>
</template>

<script>
export default{
    methods:{
        scroll(name){
            let element = document.getElementById(name);
            element.scrollIntoView({behavior: 'smooth'});
        }
    }
}
</script>

<style scoped>
    a{
        text-decoration: none;
        color: white;
    }
</style>