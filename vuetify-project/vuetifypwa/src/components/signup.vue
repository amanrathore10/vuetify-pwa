<template>
    <div>
        <v-form>
            <v-text-field label="Name" :rules="nameRules" required></v-text-field>
            <v-text-field label="Email" type="email" :rules="emailRules" required></v-text-field>
            <v-text-field label="Contact Number" type="contactno" required></v-text-field>
            <v-text-field label="Password" :rules="passwordRules" type="password" required></v-text-field>
            <v-text-field label="Confirm Password" :rules="passwordRules" type="confirmpassword" required></v-text-field>
            <v-btn type="submit" :rules="submitRules" >Login</v-btn>
        </v-form>
    </div>
    
</template>

<script>

   export default{
       name:'signup',
       data(){
           return{

           }
       },
       methods:{

       }
   } 

</script>
<style scoped>
    
</style>