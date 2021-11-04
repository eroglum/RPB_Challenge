<template>
  <v-card
    class="mx-auto"
  >
    

    <v-container>
        <div class="headline">Länder, Regionen, Orte
            <v-btn color="#16828F" :right="true" :absolute="true" text>Alle</v-btn>
        </div>
        <div class="subtitle-1">Lorem ipsum Länder, Regionen, Orte</div>
      <v-row dense>
        <v-slide-group multiple class="pa-4" :show-arrows="false">
          <v-slide-item v-for="(item, i) in items"
          :key="i">
        
          <v-card id="karte" class="rounded-xl mx-2" border-color="lime" outlined>
            
                <v-img :src="item.image"></v-img>
                <a :href=item.link><v-card-text class="text--primary">
      <v-row>
        <v-col class="d-flex justify-space-between subtitle-2">{{item.text}}</v-col>
        <v-col class="text-right h6"><span class="caption">ab</span> € {{item.price}}</v-col>
      </v-row>
    </v-card-text>
    </a>
          </v-card>
          
        </v-slide-item>
        </v-slide-group>
      </v-row>
    </v-container>
  </v-card>
</template>

<script>
  export default {
    data: () => ({
      items: [
{
"text": "Ägypten",
"price": 1237,
"image": "https://images.flux.reisen/hotel/1262/1/s",
"link": "https://google.com"
},
{
"text": "Griechenland",
"price": 334,
"image": "https://images.flux.reisen/hotel/1262/1/s",
"link": "https://google.com"
},
{
"text": "Türkei",
"price": 237,
"image": "https://images.flux.reisen/hotel/1262/1/s",
"link": "https://google.com"
},
{
"text": "Italien",
"price": 237,
"image": "https://images.flux.reisen/hotel/1262/1/s",
"link": "https://google.com"
},
{
"text": "Spanien",
"price": 379,
"image": "https://images.flux.reisen/hotel/1262/1/s",
"link": "https://google.com"
},
{
"text": "Kroatien",
"price": 88,
"image": "https://images.flux.reisen/hotel/1262/1/s",
"link": "https://google.com"
},
{
"text": "Österreich",
"price": 0,
"image": "https://images.flux.reisen/hotel/1262/1/s",
"link": "https://google.com"
}
],
    }),
  }
</script>

<style>

#karte {
    box-shadow: -2px 2px 1px #D9E15F;
    background: linear-gradient(white)
}
a {
  text-decoration: none !important;
}

</style>