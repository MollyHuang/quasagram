<template>
  <q-page class="constrain q-pa-md">
    
    <div class="row q-col-gutter-md">
      <div class="col-12 col-sm-8">
        <q-card
          v-for="post in posts"
          :key="post.id"
          class="card-post q-mb-md"
          bordered
          flat
        >

          <q-item>
            <q-item-section avatar>
              <q-avatar>
                <img src="https://instagram.ftpe7-1.fna.fbcdn.net/v/t51.2885-19/11373805_1672166586350116_972886693_a.jpg?_nc_ht=instagram.ftpe7-1.fna.fbcdn.net&_nc_ohc=TuNXbIEO_RkAX8v5P6P&edm=ABfd0MgAAAAA&ccb=7-4&oh=3784e2412487c770a7e760f1c79ecb03&oe=60AA8037&_nc_sid=7bff83">
              </q-avatar>
            </q-item-section>

            <q-item-section>
              <q-item-label class="text-bold">Molly Huang</q-item-label>
              <q-item-label caption>{{ post.location }}</q-item-label>
            </q-item-section>
          </q-item>

          <q-separator />

          <q-img :src="post.imageUrl" />

          <q-card-section>
            <div class="">{{ post.caption }}</div>
            <div class="text-caption text-grey">{{ post.date | niceDate }}</div>
          </q-card-section>

        </q-card>
      </div>

      <div class="col-4 large-screen-only">
        <q-item class="fixed">
          <q-item-section avatar>
            <q-avatar size="48px">
              <img src="https://instagram.ftpe7-1.fna.fbcdn.net/v/t51.2885-19/11373805_1672166586350116_972886693_a.jpg?_nc_ht=instagram.ftpe7-1.fna.fbcdn.net&_nc_ohc=TuNXbIEO_RkAX8v5P6P&edm=ABfd0MgAAAAA&ccb=7-4&oh=3784e2412487c770a7e760f1c79ecb03&oe=60AA8037&_nc_sid=7bff83">
            </q-avatar>
          </q-item-section>

          <q-item-section>
            <q-item-label class="text-bold">mollyhyt</q-item-label>
            <q-item-label caption>Molly Huang</q-item-label>
          </q-item-section>
        </q-item>
      </div>
    </div>

  </q-page>
</template>

<script>
import { date } from 'quasar'

export default {
  name: 'PageHome',
  data() {
    return {
      posts: [
        {
          id: 1,
          caption: 'Golden Gate Bridge',
          date: 1591776655504,
          location: 'San Francisco, United States',
          imageUrl: 'https://cdn.quasar.dev/img/parallax2.jpg'
        },
        {
          id: 2,
          caption: 'Golden Gate Bridge',
          date: 1591776655504,
          location: 'San Francisco, United States',
          imageUrl: 'https://cdn.quasar.dev/img/parallax2.jpg'
        },
        {
          id: 3,
          caption: 'Golden Gate Bridge',
          date: 1591776655504,
          location: 'San Francisco, United States',
          imageUrl: 'https://cdn.quasar.dev/img/parallax2.jpg'
        },
        {
          id: 4,
          caption: 'Golden Gate Bridge',
          date: 1591776655504,
          location: 'San Francisco, United States',
          imageUrl: 'https://cdn.quasar.dev/img/parallax2.jpg'
        }
      ]
    }
  },
  filters: {
    niceDate(value) {
      return date.formatDate(value, 'MMMM D h:mmA')
    }
  }
}
</script>

<style lang="sass">
  .card-post
    .q-img
      min-height: 200px
</style>
