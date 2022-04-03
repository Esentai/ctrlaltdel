<template>
    <v-navigation-drawer app style="background-color:#272b35" dark>
        <v-card
        height="100vh"
        width="256"
        class="mx-auto"
        style="background-color:#272b35"
        dark
        >

                <v-list-item >
                    <v-list-item-content >
                        <v-list-item-title class="text-h5 text-center" style="margin: 5px 0; font-weight:800">
                           Ctrl Alt Del
                        </v-list-item-title>
                    </v-list-item-content>
                </v-list-item>

                <v-divider></v-divider>
                <v-list-item style="justify-content: center;">
                    <v-list-content>
                        <div class="text-center">
                            <br>
                        <v-badge
                            bordered
                            bottom
                            color="deep-purple accent-4"
                            dot
                            offset-x="10"
                            offset-y="10"
                        >
                            <v-avatar  size="40">
                            <v-img src="../assets/default_user_icon.png"></v-img>
                            </v-avatar>
                        </v-badge>
                            <p style="margin-top:15px">Курманбай Есентай</p>
                        </div>
                    </v-list-content>
                </v-list-item>
                <v-list dense  nav dark>
                    <v-list-item>
                        <v-list-item-icon>
                            <v-icon dark>
                                mdi-cloud-upload
                            </v-icon>
                        </v-list-item-icon>

                        <v-list-item-content>
                            <v-list-item-title>Кибербуллинг</v-list-item-title>
                        </v-list-item-content>
                    </v-list-item>
                                        <v-list-item>
                        <v-list-item-icon>
                            <v-icon dark>
                                mdi-map
                            </v-icon>
                        </v-list-item-icon>

                        <v-list-item-content>
                            <v-list-item-title>Карта города</v-list-item-title>
                        </v-list-item-content>
                    </v-list-item>
                </v-list>
        </v-card>
    </v-navigation-drawer>
</template>

<script>

export default {
        
    }
</script>

<style scoped>
.profile{

  
}
</style>