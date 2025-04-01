<template>
  <v-footer
    dark
    padless
    style="cursor: pointer;"
  >
    <v-card
      flat
      tile
      class="white--text text-center"
      color="#ffb301"
      width="100%"
    >
      <v-card-text class="black--text d-flex align-center justify-center pa-1">
        <strong>Peça agora e nós entregamos até você!</strong>
        <v-img
          alt="Vuetify Logo"
          class="shrink ml-2"
          contain
          src="@/assets/entrega-rapida.png"
          transition="scale-transition"
          width="35"
        />
      </v-card-text>
    </v-card>
    <v-card
      flat
      tile
      class="lighten-1 white--text text-center"
      color="#313338"
      width="100%"
    >
      <v-row>
        <v-col cols="2">
          <v-card-text class="white--text ">
            <strong style="color:#ffb301;">Quem Somos</strong>
            <p class="mt-4">
              Criamos hambúrgueres artesanais, feitos com ingredientes frescos e de qualidade.
            </p>
          </v-card-text>
        </v-col>
        <v-col cols="3">
          <v-card-text class="white--text">
            <strong style="color:#ffb301;">Siga-nos</strong><br/>
            <v-btn  
              v-for="icon in icons"
              :key="icon"
              class="mx-2 mt-4 white--text"
              icon
              color="accent-4"
            >
              <v-icon size="24px" color="white">
                {{ icon }}
              </v-icon>
            </v-btn>
          </v-card-text>
        </v-col>
        <v-col cols="2">
          <v-card-text class="white--text text-left">
            <strong style="color:#ffb301;">Navegação</strong><br/>
            <v-list class="transparent mt-0">
              <v-list-item-group class="mt-2">
                <v-list-item
                  v-for="(link, index) in links"
                  :key="index"
                  :href="link.url"
                  target="_blank"
                  class="pa-0"
                  style="min-height: 30px;"
                >
                    <v-list-item-title class="white--text" style="font-size: 13px">
                      {{ link.text }}
                    </v-list-item-title>
                </v-list-item>
              </v-list-item-group>
            </v-list>
          </v-card-text>
        </v-col>
        <v-col cols="2">
          <v-card-text class="white--text text-left">
            <strong style="color:#ffb301;">Fique por Dentro</strong>
            <v-text-field
              class="mt-4"
              outlined
              dense
              label="Seu e-mail"
              prepend-inner-icon="mdi-email-plus-outline"
            />
          </v-card-text>
        </v-col>
        <v-col cols="3">
          <v-card-text class="white--text text-left">
            <strong style="color:#ffb301;">Onde Estamos</strong>
            <p class="mt-4">
              Rua dos Sabores, 123 - Centro, Cidade dos Hambúrgueres, GO - 12345-678
            </p>
            <p class="mb-0">
              (62) 0 0000-0000
            </p>
            <p>
              Segunda a Sábado: 11h - 22h
            </p>
          </v-card-text>
        </v-col>
      </v-row>
      <v-divider></v-divider>
      <v-card-text class="white--text">
        {{ new Date().getFullYear() }} — <strong>Todos os direitos reservados.</strong>
      </v-card-text>
    </v-card>
  </v-footer>
</template>

<script>
  export default {
    data: () => ({
      icons: [
        'mdi-facebook',
        'mdi-linkedin',
        'mdi-instagram',
        'mdi-pinterest',
      ],
      links: [
        { text: "Inicio", url: "/", icon: "mdi-home" },
        { text: "Produtos", url: "/sobre", icon: "mdi-information" },
        { text: "Sobre", url: "/contato", icon: "mdi-email" },
      ],
    }),
  }
</script>