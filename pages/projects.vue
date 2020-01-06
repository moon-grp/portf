<template>
  <v-container>
    <v-row class="mt-9">
      <v-col v-for="card in cards" :key="card.title" :cols="card.flex">
        <v-card raised>
          <v-img
            :src="card.src"
            class="white--text align-end"
            height="150px"
          >
          </v-img>
          <v-card-title v-text="card.title"></v-card-title>
          <v-card-actions>
            <v-spacer></v-spacer>

            <v-btn icon>
              <v-icon>mdi-heart</v-icon>
            </v-btn>

            <v-btn icon>
              <v-icon>mdi-bookmark</v-icon>
            </v-btn>

            <v-btn icon>
              <v-icon>mdi-share-variant</v-icon>
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'projects',
  data: () => ({
    cards: [
      { title: 'Pre-fab homes', src: '/expense.png', flex: 3 },
      { title: 'Favorite road trips', src: '/borodash.png', flex: 3 },
      { title: 'Best airlines', src: '/empdash.png', flex: 3 },
      { title: 'Best airlines', src: '/coffee.png', flex: 3 },
      { title: 'Best airlines', src: '/insure.png', flex: 3 },
      { title: 'Best airlines', src: '/reiner.png', flex: 3 },
      { title: 'Best airlines', src: '/reiss.png', flex: 3 }
    ]
  })
}
</script>

<style scoped></style>
