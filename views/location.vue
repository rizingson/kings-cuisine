<template>
    <v-container fluid fill-height class="about">
        <v-layout column>
            <v-flex xs6 md6 align-self-center>
                <v-card xs4 color="#242526" dark class="about-card border">
                    <v-img
                        :src="require('../assets/storeFront.jpg')"
                        contain
                    />"
                    <v-card-text class="headline text-xs-center text-uppercase">
                        Location and Hours
                        <hr />
                    </v-card-text>
                    <v-card-text class="subheading mt-2 text-xs-center">
                        360 W Main St. <br />
                        Merced, CA 95340<br />
                        <a class="link" href="tel:209383983">(209) 383-9838</a>
                        <br />
                        <br />
                        <strong>Business Hours:</strong><br />
                        Tuesday-Thursday: 11am to 9pm<br />
                        Friday: 11am to 10pm<br />
                        Saturday: 12pm to 10pm<br />
                        Sunday: 12pm to 9pm
                    </v-card-text>
                    <v-card-actions>
                        <v-btn flat dark color="white" to="/"
                            >Back To Home</v-btn
                        >
                    </v-card-actions>
                </v-card>
            </v-flex>
        </v-layout>
    </v-container>
</template>

<script>


export default {
    name: 'location',
    components: {}
};
</script>

<style></style>
