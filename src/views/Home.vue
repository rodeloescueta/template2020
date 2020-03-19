<template>
  <v-container fluid pa-0 class="text-center">
    <v-carousel
    cycle
    height="400"
    hide-delimiter-background
    show-arrows-on-hover
  >
    <v-carousel-item
      v-for="(item,i) in items"
      :key="i"
      :src="item.src"
      reverse-transition="fade-transition"
      transition="fade-transition"
    ></v-carousel-item>
  </v-carousel>
  <v-container fluid pa-0>
    <p class="display-3">Cupidatat magna occaecat minim consectetur.</p>
    <p class="headline font-weight-black">Amet aute in magna nisi nostrud duis quis cupidatat ut.</p>
    <p>Dolor consectetur qui deserunt excepteur dolor adipisicing cupidatat officia quis consequat. Commodo voluptate incididunt ex ipsum ipsum aute non minim deserunt voluptate laborum dolore. Incididunt ullamco qui laborum tempor occaecat nisi cillum duis eiusmod laborum eu tempor sunt aliquip. Non qui ea veniam Lorem duis culpa occaecat.</p>
    <hr/>
    <p>{{`Nulla aliqua quis deserunt ea occaecat non. Esse cupidatat excepteur consectetur amet qui ut mollit cupidatat voluptate labore. Sit anim mollit esse anim aliquip culpa fugiat irure minim est incididunt exercitation enim ut. Sint consequat magna magna dolore amet ipsum et veniam consectetur nisi excepteur ad exercitation. Commodo est ullamco officia occaecat cillum reprehenderit. Sunt voluptate laboris pariatur dolor culpa duis.

Fugiat cillum mollit aute incididunt aute non voluptate. Culpa ea esse adipisicing quis enim ex sint nulla ullamco nisi eu irure quis enim. Proident ullamco reprehenderit eiusmod nostrud est duis ea laborum aliqua ut pariatur in cillum. Sit elit esse proident ea reprehenderit consectetur nulla consectetur enim est laborum. Mollit nulla pariatur et incididunt. Labore ullamco qui tempor aliquip minim commodo veniam eu ut nisi magna ut nulla qui.

Culpa laborum velit exercitation irure elit officia occaecat commodo Lorem laboris consequat voluptate. Et cupidatat exercitation dolor sit consectetur aute voluptate anim ea sint aliqua. Anim sint esse ipsum occaecat do aliqua commodo occaecat sit nisi anim. Consectetur eu ex pariatur Lorem sunt mollit nisi tempor veniam nulla ex exercitation. Ut duis officia cupidatat eu ex do adipisicing reprehenderit consectetur. Nisi aliquip deserunt nostrud quis reprehenderit velit sint ea cupidatat.

Dolor culpa do cupidatat qui pariatur veniam ex laboris nulla consectetur. Irure officia proident nisi in Lorem exercitation laborum incididunt nulla proident dolor laborum in. Ut occaecat duis officia et fugiat tempor proident ea incididunt reprehenderit minim. Reprehenderit ea exercitation anim ut minim veniam. Eu in et id anim.`}}</p>
  <v-divider/>
  <v-spacer/>
  <p>{{`Cupidatat enim sunt reprehenderit adipisicing commodo dolor labore tempor amet velit do in. Minim fugiat ex pariatur do cillum. Ut dolore ex est dolore reprehenderit duis. Sint et officia anim irure voluptate nulla nulla nisi.

Esse cillum tempor elit ullamco reprehenderit fugiat est dolore. Enim fugiat aliquip magna ad consequat elit commodo esse. Culpa magna officia cupidatat proident deserunt. Ullamco esse Lorem dolore esse dolore ad officia cupidatat magna. Nisi mollit est dolore adipisicing cillum in elit ad excepteur ullamco. Irure non occaecat cillum reprehenderit nulla reprehenderit id anim esse.

Est ad fugiat magna officia enim consectetur tempor voluptate commodo exercitation Lorem adipisicing. Dolor incididunt consectetur enim magna mollit aliquip exercitation nisi labore pariatur consectetur nisi officia. Minim ut irure anim labore incididunt occaecat est consectetur. Cupidatat magna tempor esse officia elit dolore exercitation Lorem nulla elit eu do. Consequat aliquip nisi nisi minim. Duis cupidatat ad qui aliquip sunt nisi. Dolor consectetur officia culpa occaecat ea et ut tempor cillum deserunt incididunt irure proident.

Veniam irure Lorem amet amet. Dolore laborum aliquip proident cillum esse eu enim nisi aliquip consectetur ea elit. Do deserunt exercitation nostrud deserunt irure ad nisi ullamco Lorem consequat nisi sint. Eiusmod magna magna reprehenderit aliqua irure amet. Officia et magna sint veniam sunt sunt sit. Nostrud do velit nostrud quis elit enim ad nulla sint est dolore dolore ea. Ipsum est enim ipsum culpa fugiat elit quis cillum excepteur.`}}</p>
  </v-container>
  </v-container>
</template>

<script>
export default {
    data () {
      return {
       items: [
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/squirrel.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/sky.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/bird.jpg',
          },
          {
            src: 'https://cdn.vuetifyjs.com/images/carousel/planet.jpg',
          },
        ],
      }
    },
  }
</script>
<style>
.bg{
    background: url('~@/assets/bg.png') repeat;
}
</style>
