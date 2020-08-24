<template>
<vueper-slides fade :touchable="false">
  <vueper-slide
    v-for="(slide, i) in slides"
    :key="i"
    :image="slide.image"
    :title="slide.title"
    :content="slide.content" />
</vueper-slides>
</template>

<script>
import { VueperSlides, VueperSlide } from 'vueperslides'
import 'vueperslides/dist/vueperslides.css'

export default {
  components: { VueperSlides, VueperSlide },
  data: () => ({
      slides: [
        {
            image: 'https://keyassets.timeincuk.net/inspirewp/live/wp-content/uploads/sites/18/2020/01/botnia-targa-25-1-outboard-powered-boat-review-running-shot-credit-richard-langdon.jpg'
        },
        {
            image: 'https://images.pexels.com/photos/163236/luxury-yacht-boat-speed-water-163236.jpeg?auto=compress&cs=tinysrgb&dpr=1&w=500'
        },
    ]
  }),
}
</script>