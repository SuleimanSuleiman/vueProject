<template>
    <v-footer dark padless style="position: relative;top: 144px; height: 60px;margin-top: 21px;">
        <div class="foot d-flex" style="width: 100%">
            <v-row class="text-center">
            <v-col cols="2">
                <v-btn icon>
                    <v-icon color="#A7121D">fas fa-dragon</v-icon>
                </v-btn>
            </v-col>
            <v-col cols="8">
                <v-btn icon v-for="i in icons" :key="i">
                    <v-icon>{{i}}</v-icon>
                </v-btn>
            </v-col>
            <v-col cols="2">
                <v-btn icon>
                        <v-icon color="#A7121D">fas fa-heart</v-icon>
                </v-btn>
            </v-col>
            </v-row>
        </div>
    </v-footer>
</template>

<script>
export default{
    name: 'FooterApp',
    data:() =>({
        icons:[
            "mdi-facebook",
            "mdi-twitter",
            "mdi-youtube",
            "mdi-linked"
        ]
    })
}
</script>
