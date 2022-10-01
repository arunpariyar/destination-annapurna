<template>
  <!-- THE GALLERY SECTION -->
  <section class="section section--2">
    <div class="section-heading" id="section--2">Impressions</div>
    <div class="gallery">
      <figure class="gallery__photos gallery__photos--1">
        <img
          src="../assets/images/gallery/suspended bridge-Pakding-Nepal.jpg"
          alt="suspended Bridge Phakding"
          class="gallery__photo"
        />
      </figure>
      <figure class="gallery__photos gallery__photos--2">
        <img
          src="../assets/images/gallery/Annapurna-Narchyang-Nepal.jpg"
          alt="Annapurna Narchyang Nepal"
          class="gallery__photo"
        />
      </figure>
      <figure class="gallery__photos gallery__photos--3">
        <img
          src="../assets/images/gallery/Annapurna Peak and pass in the Himalaya mountains.jpg"
          alt="Annapurna Peak and pass in the Himalaya mountains"
          class="gallery__photo"
        />
      </figure>
      <figure class="gallery__photos gallery__photos--4">
        <img
          src="../assets/images/gallery/Annapurna-Machapuchhare.jpg"
          alt="Annapurna Machapuchhare"
          class="gallery__photo"
        />
      </figure>
      <figure class="gallery__photos gallery__photos--5">
        <img
          src="../assets/images/gallery/Near-Annapurna-Pokhara-Nepal.jpg"
          alt="Near-Annapurna-Pokhara-Nepal"
          class="gallery__photo"
        />
      </figure>
      <figure class="gallery__photos gallery__photos--6">
        <img
          src="../assets/images/gallery/poonhill.jpg"
          alt="poonhill in Ghorepani"
          class="gallery__photo"
        />
      </figure>
      <figure class="gallery__photos gallery__photos--7">
        <img
          src="../assets/images/gallery/village-nestled-in-annapurna.jpg"
          alt="Village nestled in Annapurna"
          class="gallery__photo"
        />
      </figure>
      <figure class="gallery__photos gallery__photos--8">
        <img
          src="../assets/images/gallery/waterfall-manang-nepal.jpg"
          alt="Waterfall in Manang"
          class="gallery__photo"
        />
      </figure>
      <figure class="gallery__photos gallery__photos--9">
        <img
          src="../assets/images/gallery/mardi-himal-base-camp.jpg"
          alt="Mardi Himal Base Camp"
          class="gallery__photo"
        />
      </figure>
      <figure class="gallery__photos gallery__photos--10">
        <img
          src="../assets/images/gallery/yellow-fewa-lake.jpg"
          alt="Yellow Fewa Lake"
          class="gallery__photo"
        />
      </figure>
    </div>
  </section>
</template>
<script>
export default {
  name: "Gallery",
};
</script>
<style lang="scss" scoped>
.section-heading {
  font-family: var(--font-heading);
  text-transform: uppercase;
  text-align: center;
  font-size: 3.5rem;
  color: var(--earth);
  letter-spacing: 15px;
  margin: 8rem 0;
}
.gallery {
  grid-column: fullbleed-start / fullbleed-end;
}

.gallery {
  display: grid;
  grid-template-columns: repeat(8, 1fr);
  grid-template-rows: repeat(7, 5vw);
  grid-gap: 1vw;

  &__photos {
    width: 100%;
    overflow: hidden;

    & > img {
      transition: all 0.5s;
      transform: scale(1.03);
    }
    & > img:hover {
      transform: scale(1.15);
    }
    &--1 {
      grid-column: 1 / span 2;
      grid-row: 1 / span 2;
    }
    &--2 {
      grid-column: 1 / span 2;
      grid-row: 3 / -1;
    }
    &--3 {
      grid-column: 3 / span 3;
      grid-row: 1 / span 3;
    }
    &--4 {
      grid-column: 3 / span 1;
      grid-row: 4 / span 2;
    }
    &--5 {
      grid-column: 4 / span 2;
      grid-row: 4 / span 2;
    }
    &--6 {
      background-position: center;
      grid-column: 3 / span 3;
      grid-row: 6 / span 2;
    }
    &--7 {
      grid-column: 6 / span 3;
      grid-row: 5 / -1;
    }
    &--8 {
      grid-column: 7 / span 2;
      grid-row: 1 / span 4;
    }
    &--9 {
      background-position: center;
      grid-column: 6 / span 1;
      grid-row: 1 / span 3;
    }
    &--10 {
      grid-column: 6 / span 1;
      grid-row: 4 / span 1;
    }
  }

  &__photo {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
  }
}
</style>
