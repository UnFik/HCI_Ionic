<template>
    <ion-page>
        <ion-header>
            <ion-row class="ion-align-items-center">
                <ion-col size="3">
                    <a href="/kolam">
                        <font-awesome-icon icon="fa-solid fa-angle-left" style="margin-left: 10%; font-size: 30px;"/>
                    </a>
                </ion-col>
                <ion-col>
                    <h1>Registrasi Kolam</h1>
                </ion-col>
            </ion-row>
        </ion-header>

        <ion-content :fullscreen="true">
            <ion-icon src="icon/home-sharp.svg"></ion-icon>
        </ion-content>
    </ion-page>
</template>

<script lang="ts">
import {
    IonContent,
    IonHeader,
    IonPage,
    IonIcon,
} from "@ionic/vue";
import { defineComponent } from "vue";
import { homeSharp } from "ionicons/icons";

export default defineComponent({
    name: "RegisterPage",
    components: {
        IonContent,
        IonHeader,
        IonPage,
        IonIcon,
    },
    setup() {
        return {
            "home-sharp" : homeSharp,
        };
    },
});
</script>

<style scoped>
#container {
    text-align: center;

    position: absolute;
    left: 0;
    right: 0;
    top: 50%;
    transform: translateY(-50%);
}

#container strong {
    font-size: 20px;
    line-height: 26px;
}

#container p {
    font-size: 16px;
    line-height: 22px;

    color: #8c8c8c;

    margin: 0;
}

#container a {
    text-decoration: none;
}

a:visited {
    color: white;
}

ion-button {
    --background: #1B7C1A;
}

ion-card,
ion-card-title,
ion-card-subtitle {
    color: black;
}

ion-card-title {
    font-weight: bold;
    font-size: 18px !important;
}

ion-card {
    border-radius: 16px;
    margin-bottom: 20px !important;
}

ion-button {
    --border-radius: 12px
}

.deactive {
    --background: #952229;
}

.fixedButton {
    /* --border-radius : 50%; */
    position: fixed;
    bottom: 0px;
    right: 0px;
    width: 100px;
    height: auto;
}
</style>
