<template>
    <div>
        <p>Login page</p>
        <v-flex pa-5>
        <v-card  >
            <v-form ma-3>
            
            <v-text-field label="Email" type="email" :rules="emailRules" required></v-text-field>
            
            <v-text-field label="Password" :rules="passwordRules" type="password" required></v-text-field>
            
            <v-btn type="submit" :rules="submitRules" >Login</v-btn>
        </v-form>

        </v-card>
    </v-flex>
    </div>
    
</template>
<script>
    export default{
        name:'login',
        data(){
            return{

            }

        },
        methods:{

        }
    }
</script>