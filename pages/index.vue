<template>
  <div>
    <div class="flex justify-center">
      <img class="image" src="~/assets/images/dd.png" />
    </div>
    <div>
      <h1 class="text-3xl font-bold">Hello, I'm Huevang</h1>
      <div class="pb-3">
        <p class="w-full border-2 rounded-lg my-3 p-10 "> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; Lorem ipsum dolor
          sit amet consectetur adipisicing elit. Ipsum tempora, voluptates mollitia asperiores numquam velit maiores
          consequuntur non, impedit molestias modi quam, quasi iste iure nisi. Ullam esse sapiente commodi dolores
          soluta ea incidunt aut, animi, optio illo maxime excepturi iure similique ad libero id labore eveniet tenetur.
          Facilis id temporibus, quos corporis aut eius quia illum distinctio culpa eveniet, aperiam dolorum quasi
          quidem rerum molestias dolore atque corrupti cum quod dicta placeat sint ab accusamus voluptas. Voluptatem
          laboriosam eos quod, dicta ducimus placeat labore, mollitia quibusdam et voluptas temporibus molestiae
          numquam? Quam natus, ipsam laudantium velit quod repellat mollitia repellendus fuga ipsa doloremque nostrum
          quasi vero saepe molestias, ad fugit voluptatum est, obcaecati ut provident. Dolores, iste totam! Illum
          dignissimos temporibus dolores velit nam nesciunt eaque quaerat maxime! Enim, ea. Tempore dolorem, nostrum,
          magnam laudantium praesentium quaerat corrupti debitis obcaecati ab libero delectus quam! Illo in
          necessitatibus omnis eaque? Expedita consequatur beatae minus assumenda ab provident hic saepe consectetur rem
          fugit debitis nesciunt dicta labore tempore mollitia omnis possimus architecto nam necessitatibus
          reprehenderit eius qui, pariatur quo reiciendis. Officia sit magni illo quaerat? Harum nostrum, consequuntur
          non doloribus id quibusdam tempore nobis dolorum distinctio dolores, laborum numquam voluptatibus ex esse
          culpa error asperiores, at atque fugiat. Ratione quasi quidem maiores labore enim iste minus, magni fugiat
          sunt debitis eveniet, deleniti possimus commodi omnis error, veritatis nisi nulla blanditiis dicta modi
          explicabo a aliquid accusantium ullam. Dolor id molestiae nesciunt earum quam alias, ipsa ea consectetur vitae
          sapiente unde quae necessitatibus, dicta impedit. Atque modi dolorum sunt, at suscipit necessitatibus
          consectetur, vel, ratione commodi sint eum? Vitae inventore autem amet error hic sapiente, quas similique nisi
          repellendus ipsum exercitationem a dolorum ipsa aut ut magnam pariatur, vel minus quis, expedita recusandae
          ipsam tempora voluptates provident. Eligendi error expedita dignissimos ullam.</p>
      </div>
      <div class="text-3xl font-bold">I'm a Web Developer</div>
    
    </div>
    <div  class="grid grid-cols-4 gap-4">
        <div v-for="(i, index) in data" :key="index" class="w-60 bg-white my-10 rounded-xl text-[#000000] p-5 ">
          <img :src="i.img" class="w-40 h-40 mx-auto" alt="logo"/>
          <h1 class="text-lg font-bold">{{i.title}}</h1>
          <p>Lorem ipsum dolor, sit amet ...</p>
        </div>
      </div>
    <div class="h-10">
      huevnag
    </div>
  </div>
</template>

<script setup lang="ts">
const { $anime } = useNuxtApp()

onMounted(() => {
  $anime({
    targets: '.image',
    translateY: 50,
    easing: 'easeInOutSine',
    direction: 'alternate',
    loop: true,
    duration: 3000
  })

  $anime({
    targets: '.Text',
    translateX: 30,
    easing: 'easeInOutSine',
    direction: 'alternate',
    loop: true,
    duration: 3000
  })
})
const data = [
  {title: 'Front end', img:'https://w7.pngwing.com/pngs/257/475/png-transparent-web-development-html5-video-css3-software-development-frontend-web-development-thumbnail.png'},
  {title: 'Back end', img:'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT_TwWNkctM-SnJzhHU_cvbNbIbF5MRPoWxjQ&s'},
  {title: 'Server', img:'https://cdn2.iconfinder.com/data/icons/firewall-security/500/vab286_4_server_station_isometric_cartoon_center_computer_data-512.png'},
  {title: 'Mobile', img:'https://e7.pngegg.com/pngimages/713/558/png-clipart-computer-icons-pro-git-github-logo-text-logo-thumbnail.png'},
]
</script>


<style scoped></style>
