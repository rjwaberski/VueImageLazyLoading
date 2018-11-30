<template>
  <div class="test">
    <section v-for="section in sections" :key="section.imageUrl">
      <image-item class="image-item" v-if="section " :source="section.imageUrl"/>
    </section>
  </div>
</template>

<script>
import ImageItem from "./ImageItem";
export default {
  components: {
    ImageItem
  },
  data() {
    return {
      sections: [
        {
          imageUrl:
            "https://images.pexels.com/photos/443446/pexels-photo-443446.jpeg"
        },
        {
          imageUrl:
            "https://wallpaper.wiki/wp-content/uploads/2017/04/wallpaper.wiki-Landscape-Free-Wallpaper-HD-PIC-WPB004150.jpg"
        },
        {
          imageUrl:
            "http://thewowstyle.com/wp-content/uploads/2015/04/free-wallpaper-landscape.jpg"
        },
        {
          imageUrl:
            "https://wallpaper.wiki/wp-content/uploads/2017/06/Supernova-rainbow-explosion-backgrounds.jpg"
        },
        {
          imageUrl:
            "https://wallpaper.wiki/wp-content/uploads/2017/06/HD-Wallpapers-Free-Backgrounds.jpg"
        },
        {
          imageUrl:
            "https://wallpaper.wiki/wp-content/uploads/2017/06/HD-Free-Wallpapers-Backgrounds.jpg"
        },
        {
          imageUrl:
            "https://wallpaper.wiki/wp-content/uploads/2017/06/Full-hd-wallpapers-desktop-free-download.jpg"
        }
      ]
    };
  }
};
</script>
