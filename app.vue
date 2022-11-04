<template>
    <v-card text="Vuetify" variant="tonal">
        <h1>Welcome to the homepage</h1>
        <v-menu transition="slide-x-transition">
            <template v-slot:activator="{ props }">
                <v-btn
                        color="primary"
                        class="ma-2"
                        v-bind="props"
                >
                    Slide X Transition
                </v-btn>
            </template>
            <v-list>
                <v-list-item
                        v-for="n in 5"
                        :key="n"
                        link
                >
                    <v-list-item-title v-text="'Item ' + n"></v-list-item-title>
                </v-list-item>
            </v-list>
        </v-menu>
    </v-card>
</template>
