<template>
  <q-page class="constrain q-pa-md">
    <q-card class="card-post" flat bordered>

      <q-item>
        <q-item-section avatar>
          <q-avatar>
            <img src="https://instagram.ftpe7-1.fna.fbcdn.net/v/t51.2885-19/11373805_1672166586350116_972886693_a.jpg?_nc_ht=instagram.ftpe7-1.fna.fbcdn.net&_nc_ohc=TuNXbIEO_RkAX8v5P6P&edm=ABfd0MgAAAAA&ccb=7-4&oh=3784e2412487c770a7e760f1c79ecb03&oe=60AA8037&_nc_sid=7bff83">
          </q-avatar>
        </q-item-section>

        <q-item-section>
          <q-item-label class="text-bold">Molly Huang</q-item-label>
          <q-item-label caption>Taipei, Taiwan</q-item-label>
        </q-item-section>
      </q-item>

      <q-separator />

      <q-img src="https://cdn.quasar.dev/img/parallax2.jpg" />

      <q-card-section>
        <div class="">Golden Gate Bridge</div>
        <div class="text-caption text-grey">June 10 9:04AM</div>
      </q-card-section>

    </q-card>
  </q-page>
</template>

<script>
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
  }
}
</script>

<style lang="sass">
  .card-post
    .q-img
      min-height: 200px
</style>
