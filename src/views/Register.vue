<template>
<v-container>
    <v-content>
        <v-container class="fill-height" fluid>
            <v-row align="center" justify="center">
                <v-col cols="12" sm="8" md="8">
                    <v-card class="elevation-12">
                        <v-window v-model="step">
                            <v-window-item :value="1">
                                <v-row class="fill-height">
                                    <v-col cols="12" md="4" class="pink accent-3">
                                        <v-card-text class="white--text mt-12">
                                            <h1 class="text-center display-1">Welcome Back!!</h1>
                                            <h5 class="text-center">To Keep connected with us please login with your personal account</h5>
                                        </v-card-text>
                                        <div class="text-center">
                                            <v-btn rounded outlined white @click="step--">SING IN</v-btn>
                                        </div>
                                    </v-col>
                                    <v-col cols="12" md="8">
                                        <v-card-text class="mt-12">
                                            <v-form>
                                                <v-text-field label="Name" name="Name" prepend-icon="persn" type="text" color="pink accent-3"/>
                                                <v-text-field label="Email" name="Email" prepend-icon="email" type="text" color="pink accent-3"/>
                                                <v-text-field label="Password" name="Password" prepend-icon="lock" type="password" color="pink accent-3"/>
                                            </v-form>  
                                        </v-card-text> 
                                        <div class="text-center mt-n5">
                                            <v-btn rounded color="pink accent-3" white>SING UP</v-btn>
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
</v-container>
</template>
<script>
export default {
    name:'MyRegister',
}
</script>