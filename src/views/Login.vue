<template>
    <div class="center">
        <v-row>
            <v-col cols="10" offset="1">
                <v-avatar color="primary" size="95" tile>
                    <v-img src="@/assets/logo.png"></v-img>
                </v-avatar>
                <v-text-field label="UserName" v-model="Placeholder"></v-text-field>
                <v-text-field label="Password" type="Password" v-model="password"></v-text-field>
                <v-btn block @click="authenticate()" class="base-inverted" color="blue">Login</v-btn>
            </v-col>
        </v-row>
    </div>
</template>

<script>
export default {
    data() {
        return {
            UserName: "",
            Password: ""
        }
    },
    methods: {
        authenticate() {
            alert("User Created");
        }
    },

}
</script>

<style lang="scss" scoped>

</style>