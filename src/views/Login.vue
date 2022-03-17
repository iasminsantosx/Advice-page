<template>
    <v-content>
        <v-container class="fill-height" fluid>
                <v-row align="center" justify="center">
                    <v-col cols="12" sm="8" md="8">
                        <v-card class="elevation-12">
                            <v-window v-model="step">
                                <v-window-item :value="1">
                                    <v-row>
                                        <v-col cols="12" md="8">
                                            <v-card-text class="mt-12">
                                                <h1 class="text-center display-2 pink--text text--accent-3">Sing In</h1>
                                                <v-form>
                                                    <v-text-field label="Email" name="Email" prepend-icon="email" type="text" color="pink accent-3"/>
                                                    <v-text-field label="Password" name="Password" prepend-icon="lock" type="password" color="pink accent-3"/>
                                                </v-form>
                                                <h3 class="text-center mt-3"> Forget your password</h3>
                                            </v-card-text>
                                            <div class="text-center mt-3">
                                                <v-btn @click="logar" rounded color="pink accent-3">SING IN</v-btn>
                                            </div>
                                        </v-col>
                                        <v-col cols="12" md="4" class="pink accent-3">
                                            <v-card-text class="white--text mt-12">
                                                <h1 class="text-center display-1">Hello guys !!</h1>
                                                <h5 class="text-center">Let's go to adventure</h5>
                                            </v-card-text>
                                            <div class="text-center">
                                                <v-btn rounded outilined="" white @click="register">SING UP</v-btn>
                                            </div>
                                        </v-col>
                                    </v-row>
                                </v-window-item>  
                            </v-window>
                        </v-card>
                    </v-col>
                </v-row>
        </v-container>
    </v-content>
</template>

<script>
    export default{
        name:'MyLogin',
        methods:{
        logar() {this.$router.push({ name: "advice" });},
        register(){this.$router.push({ name: "register" });}
        },
    }
</script>