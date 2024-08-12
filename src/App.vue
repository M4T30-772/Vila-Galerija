<template>
  <div id="app">
    <header>
      <div class="header-container">
        <img src="@/assets/main_logo.png" alt="Logo" class="logo" />
      </div>
    </header>

    <section class="hero">
      <div class="overlay">
        <h1>Dobrodošli u Vila Galerija</h1>
        <p>
          Naši apartmani smješteni su na prestižnoj lokaciji u samom srcu Vukovara, s predivnim pogledom i suvremenim dizajnom. 
          Uživajte u udobnosti i svim pogodnostima urbanog života, uključujući privatni parking koji osigurava jednostavan pristup apartmanu.
        </p>
      </div>
    </section>

    <main>
  <section id="stan1" class="flat-section">
    <h2>Apartman 1 - Aqua</h2>
    
    <div class="description description-left">
      <p>
        Apartman se sastoji od ulaznog hodnika, prostranog dnevnog boravka povezanog s kuhinjom i blagovaonicom, te dvije spavaće sobe koje pružaju udobnost odmora za četiri osobe. Funkcionalna kuhinja opremljena je svim potrebnim sadržajima za ugodan boravak, dok blagovaonica i dnevni boravak, s satelitskim prijemnikom i internetom, nude doživljaj vlastitog doma.

Apartman je u potpunosti klimatiziran, a grijanje je omogućeno centralnim grijanjem, što osigurava maksimalnu udobnost tijekom cijele godine. Kupaonica je opremljena perilicom rublja i novim kupaonskim namještajem. Prva spavaća soba sadrži bračni krevet, noćne ormariće s ukrasnim lampama, te ormar. Druga spavaća soba opremljena je s dva odvojena kreveta, noćnim ormarićima, lampama, ormarom i vješalicama za odjeću.

Apartman ima terasu s vrtnom garniturom, a svakom gostu je na raspolaganju besplatno parkirno mjesto s videonadzorom i vanjski kamin za pripremu jela.
      </p>
    </div>

    <div class="carousel">
      <img :src="flat1Images[currentImageFlat1]" alt="Slika stana 1" />
    </div>

    <div class="description description-right">
      <p>
        The apartment consists of an entrance hall, a spacious living room connected to the kitchen and dining area, and two bedrooms that provide comfortable accommodation for up to four people. The functional kitchen is equipped with all the necessary amenities for a pleasant stay, while the dining area and living room, with satellite TV and internet, offer a homely experience.

The apartment is fully air-conditioned, and heating is provided by central heating, ensuring maximum comfort throughout the year. The bathroom is equipped with a washing machine and new bathroom furniture. The first bedroom features a double bed, nightstands with decorative lamps, and a wardrobe. The second bedroom is furnished with two single beds, nightstands, lamps, a wardrobe, and clothes hangers.

The apartment also has a terrace with garden furniture, and each guest has access to a free parking space with video surveillance and an outdoor grill for meal preparation.
      </p>
    </div>

    <div class="thumbnails">
      <img
        v-for="(img, index) in flat1Images"
        :key="index"
        :src="img"
        @click="setCurrentImageFlat1(index)"
        :class="{ active: index === currentImageFlat1 }"
        alt="Thumbnail"
      />
    </div>
  </section>


      <section id="stan2" class="flat-section">
        <h2>Apartman 2 - Scala</h2>
        <p class="description">
          Apartman se sastoji od ulaznog hodnika, prostranog dnevnog boravka povezanog s kuhinjom i blagovaonicom, te dvije spavaće sobe koje pružaju udoban smještaj za četiri osobe. Funkcionalna kuhinja opremljena je svim potrebnim sadržajima za ugodan boravak, dok blagovaonica i dnevni boravak s satelitskim prijemnikom i internetom nude osjećaj domaće atmosfere.

Apartman je u potpunosti klimatiziran, a grijanje je omogućeno centralnim grijanjem, što osigurava maksimalnu udobnost u svim godišnjim dobima. Kupaonica je opremljena perilicom rublja i novim kupaonskim namještajem. Prva spavaća soba sadrži bračni krevet, noćne ormariće s ukrasnim lampama i ormar. Druga spavaća soba opremljena je s dva odvojena kreveta, noćnim ormarićima, lampama, ormarom i radnim stolom.

Apartman također nudi dva balkona s vrtnom garniturom za sjedenje, idealna za opuštanje na otvorenom. Gostima je na raspolaganju besplatno parkirno mjesto s videonadzorom, kao i vanjski kamin za pripremu jela.
        </p>
        <div class="carousel">
          <img :src="flat2Images[currentImageFlat2]" alt="Slika stana 2" />
        </div>
        <div class="description description-right">
      <p>
        The apartment consists of an entrance hallway, a spacious living room connected to the kitchen and dining area, and two bedrooms that provide comfortable accommodation for four people. The functional kitchen is equipped with all the necessary amenities for a pleasant stay, while the dining area and living room, with satellite TV and internet, offer a cozy, home-like atmosphere.

The apartment is fully air-conditioned, and heating is provided by central heating, ensuring maximum comfort throughout the year. The bathroom is equipped with a washing machine and new bathroom furniture. The first bedroom features a double bed, bedside tables with decorative lamps, and a wardrobe. The second bedroom is furnished with two separate beds, bedside tables, lamps, a wardrobe, and a work desk.

The apartment also offers two balconies with outdoor seating, ideal for relaxing outdoors. Guests have access to a free parking space with video surveillance, as well as an outdoor grill for meal preparation.
      </p>
    </div>

        <div class="thumbnails">
          <img
            v-for="(img, index) in flat2Images"
            :key="index"
            :src="img"
            @click="setCurrentImageFlat2(index)"
            :class="{ active: index === currentImageFlat2 }"
            alt="Thumbnail"
          />
        </div>
      </section>

      <section id="stan3" class="flat-section">
        <h2>Apartman 3 - Vista</h2>
        <p class="description">
          Apartman se sastoji od ulaznog hodnika, dnevnog boravka koji je spojen sa kuhinjom i blagavonicom. U sklopu apartmana nalaze se dvije spavaće sobe
          koji pružaju udobnost odmora za četiri osobe. U apartmanu je omogućen boravak sa doživljajem vlastitog doma koji pruža funkcionalna kuhinja sa svim potrebnim
           sadržajima, ugodna blagavaonica, dnevni boravak sa satelitskim prijemnikom i internetom. Apartman je u potpunosti klimatiziran a grijanje je omogućeno
           sa centralin grijanjem tako da osigurava maksimalnu udobnost u svim godišnjim uvjetima. U sklopu kupaonice osigurana je perilica rublja sa novim 
           kupaonskim namještajem. Prva spavaća soba sastoji se od bračnog kreveta sa noćnim ormarićima, ukrasnim lampama i ormarom. Druga spavaća soba također se sastoji od bračnog kreveta sa noćnim ormarićem, ukrasnom lampom i ormarom. 
           Svakom gostu je na raspolaganju besplatno parking mjesto, sa video nadzorom i vanjski kamin za pripremu jela.
        </p>
        <div class="carousel">
          <img :src="flat3Images[currentImageFlat3]" alt="Slika stana 3" />
        </div>
        <div class="description description-right">
      <p>
        The apartment consists of an entry hall, a living room connected to the kitchen and dining area. It includes two bedrooms that provide comfortable accommodation for four people. 
        The apartment offers a home-like experience with a functional kitchen equipped with all necessary amenities, a cozy dining area, and a living room with satellite TV and internet access. 
        The apartment is fully air-conditioned, and heating is provided by central heating, ensuring maximum comfort in all weather conditions. 
        The bathroom is equipped with a washing machine and new bathroom furnishings. The first bedroom features a double bed with nightstands, decorative lamps, and a wardrobe. 
        The second bedroom has two separate beds, nightstands, lamps, a wardrobe, and a desk. 
        The apartment also has two balconies with garden furniture for seating. Each guest has access to a free parking space with video surveillance and an outdoor fireplace for cooking.
      </p>
    </div>

        <div class="thumbnails">
          <img
            v-for="(img, index) in flat3Images"
            :key="index"
            :src="img"
            @click="setCurrentImageFlat3(index)"
            :class="{ active: index === currentImageFlat3 }"
            alt="Thumbnail"
          />
        </div>
      </section>

      <section id="surroundings" class="flat-section">
        <h2>Okolica i Izgled Zgrade</h2>
        <p class="description">
          Apartman se nalazi između ulica Stjepana Radića i Samostanske ulice, u neposrednoj blizini samog centra grada. U okruženju su crkva Svetog Filipa i Jakova te Vukovarski vodotoranj, jedan od najpoznatijih simbola grada Vukovara. Također, u blizini su gradska tržnica, autobusni kolodvor, muzej grada Vukovara, te Vukovarska Ada. Na samo tri minute vožnje nalazi se muzej Vučedolske kulture, a pet minuta vožnje od apartmana su memorijalno spomen-obilježje Ovčara i gradski bazen.

Boravkom u našem apartmanu osigurat ćete sebi mir i blizinu kulturnih sadržaja. Šetnice uz rijeke Dunav i Vuku, kao i ostale znamenitosti, lako su dostupne pješice, bez potrebe za korištenjem automobila. Apartmani su dizajnirani za duži boravak i pružaju udobnost vlastitog doma. Svi su moderno opremljeni, novoizgrađeni, i nude osigurano parkirno mjesto pod video nadzorom.
        </p>
        <div class="carousel">
          <img :src="surroundingImages[currentImageSurroundings]" alt="Slika okolice" />
        </div>
        <div class="description description-right">
      <p>
        The apartment is located between Stjepan Radić Street and Samostanska Street, in close proximity to the city center. Nearby are the Church of St. Philip and James and the Vukovar Water Tower, one of the most iconic landmarks of the city. The city market, bus station, Vukovar City Museum, and Vukovar Ada are also within easy reach. Just a three-minute drive away is the Vučedol Culture Museum, and a five-minute drive will take you to the Ovčara Memorial and the city swimming pool.

By staying in our apartment, you will enjoy peace and the convenience of nearby cultural attractions. The promenades along the Danube and Vuka rivers, as well as other landmarks, are easily accessible on foot, without the need for a car. The apartments are designed for longer stays and provide the comfort of a home. All are newly built, modernly equipped, and offer secure parking with video surveillance.
      </p>
    </div>
        <div class="thumbnails">
          <img
            v-for="(img, index) in surroundingImages"
            :key="index"
            :src="img"
            @click="setCurrentImageSurroundings(index)"
            :class="{ active: index === currentImageSurroundings }"
            alt="Thumbnail"
          />
        </div>
      </section>
    </main>

    <footer>
  <div class="footer-content">
    <div class="left">
      <img src="@/assets/main_logo.png" alt="Logo" class="logo" />
    </div>
    <div class="center">
      <div class="contact-info">
        <p>Kontaktirajte nas: </p>
        <p>Telefon: +385 98 686 675</p>
        <p>Email: bruno.pakter@gmail.com</p>
        <p>Adresa: Stjepana Radića (Donja Mala) 5, Vukovar</p>
      </div>
    </div>
    <div class="right">
      <span>Aqua</span>
      <span>Scala</span>
      <span>Vista</span>
    </div>
  </div>
</footer>

  </div>
</template>

<script>
export default {
  data() {
    return {
      flat1Images: [
        require('@/assets/vila34.jpg'),
        require('@/assets/vila31.jpg'),
        require('@/assets/vila46.jpg'),
        require('@/assets/vila45.jpg'),
        require('@/assets/vila48.jpg'),
        require('@/assets/vila47.jpg'),
        require('@/assets/vila41.jpg'),
        require('@/assets/vila39.jpg'),
        require('@/assets/vila38.jpg'),
        require('@/assets/vila40.jpg'),
        require('@/assets/vila42.jpg'),
        require('@/assets/vila35.jpg'),
        require('@/assets/vila37.jpg'),
      ],
      flat2Images: [
        require('@/assets/vila57.jpg'),
        require('@/assets/vila58.jpg'),
        require('@/assets/vila69.jpg'),
        require('@/assets/vila67.jpg'),
        require('@/assets/vila65.jpg'),
        require('@/assets/vila75.jpg'),
        require('@/assets/vila70.jpg'),
        require('@/assets/vila55.jpg'),        
        require('@/assets/vila61.jpg'),
        require('@/assets/vila62.jpg'),
        require('@/assets/vila64.jpg'),
        require('@/assets/vila59.jpg'),
        require('@/assets/vila54.jpg'),
        require('@/assets/vila74.jpg'),
      ],
      flat3Images: [
        require('@/assets/vila107.jpg'),
        require('@/assets/vila93.jpg'),
        require('@/assets/vila85.jpg'),
        require('@/assets/vila115.jpg'),
        require('@/assets/vila90.jpg'),
        require('@/assets/vila113.jpg'),
        require('@/assets/vila92.jpg'),
        require('@/assets/vila96.jpg'),
        require('@/assets/vila102.jpg'),
        require('@/assets/vila88.jpg'),
        require('@/assets/vila84.jpg'),
        require('@/assets/vila89.jpg'),
        require('@/assets/vila97.jpg'),
        require('@/assets/vila104.jpg'),
        require('@/assets/vila112.jpg'),
      ],
      surroundingImages: [
        require('@/assets/vila5.jpg'),
        require('@/assets/vila6.jpg'),
        require('@/assets/vila4.jpg'),
        require('@/assets/vila8.jpg'),
        require('@/assets/vila12.jpg'),
        require('@/assets/vila14.jpg'),
        require('@/assets/vila17.jpg'),
        require('@/assets/vila27.jpg'),
        require('@/assets/vila25.jpg'),
        require('@/assets/vila72.jpg'),
        require('@/assets/vila15.jpg'),
        require('@/assets/vila16.jpg'),
        require('@/assets/vila22.jpg'),
        require('@/assets/vila23.jpg'),
        require('@/assets/vila24.jpg'),
      ],
      currentImageFlat1: 0,
      currentImageFlat2: 0,
      currentImageFlat3: 0,
      currentImageSurroundings: 0,
    };
  },
  mounted() {
    setInterval(() => {
      this.nextImageFlat1();
    }, 5000);

    setInterval(() => {
      this.nextImageFlat2();
    }, 5000);
    setInterval(() => {
      this.nextImageFlat3();
    }, 5000);

    setInterval(() => {
      this.nextImageSurroundings();
    }, 5000);
  },
  methods: {
    nextImageFlat1() {
      this.currentImageFlat1 = (this.currentImageFlat1 + 1) % this.flat1Images.length;
    },
    nextImageFlat2() {
      this.currentImageFlat2 = (this.currentImageFlat2 + 1) % this.flat2Images.length;
    },
    nextImageFlat3() {
      this.currentImageFlat3 = (this.currentImageFlat3 + 1) % this.flat3Images.length;
    },
    nextImageSurroundings() {
      this.currentImageSurroundings = (this.currentImageSurroundings + 1) % this.surroundingImages.length;
    },
    setCurrentImageFlat1(index) {
      this.currentImageFlat1 = index;
    },
    setCurrentImageFlat2(index) {
      this.currentImageFlat2 = index;
    },
    setCurrentImageFlat3(index) {
      this.currentImageFlat3 = index;
    },
    setCurrentImageSurroundings(index) {
      this.currentImageSurroundings = index;
    },
  },
};
</script>

<style lang="scss">
#app {
  font-family: 'Open Sans', Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

header {
  background-color: #2c3e50;
  padding: 8px 0; /* Smanjuje padding iznad i ispod */
  text-align: center;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);

  .header-container {
    max-width: 600px; /* Smanjena širina */
    margin: 0 auto;
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100px; /* Smanjuje visinu header-a */
  }

  .logo {
    width: 150px; /* Smanjuje širinu loga */
    height: 100px; /* Smanjuje visinu loga */
  }
}

.hero {
  margin-top: 10px;
  background-image: url('@/assets/4slike.png');
  background-color: white;
  background-size: cover; /* Slika će zauzimati cijelu sekciju bez rezanja */
  background-position: center; /* Slika će biti centrirana unutar sekcije */
  background-repeat: no-repeat; /* Sprečava ponavljanje slike */
  position: relative;
  width: 100%; /* Podešava širinu hero sekcije */
  height: 1000px; /* Možete mijenjati visinu po potrebi */
  max-width: 2000px; /* Maksimalna širina hero sekcije */
  margin-left: auto; /* Centriranje sekcije */
  margin-right: auto; /* Centriranje sekcije */
  display: flex;
  align-items: center;
  justify-content: center;
  color: white;
  text-align: center;
}

.overlay {
  background-color: rgba(0, 0, 0, 0.5);
  padding: 30px; /* Povećaj padding za više prostora unutar overlay-a */
  border-radius: 10px;

  h1 {
    font-size: 3em;
    margin-bottom: 20px;
  }

  p {
    font-size: 1.5em;
    max-width: 600px;
    margin: 0 auto;
  }
}

main {
  padding: 30px;
  flex: 1;
}

.flat-section {
  margin: 50px 0;
  padding: 20px;
  background-color: #f0f0f0;
  border-radius: 10px;
  display: grid;
  grid-template-columns: 1fr 2fr 1fr;
  grid-gap: 20px;
  align-items: center;
  justify-items: center;

  h2 {
    font-size: 2em;
    margin-bottom: 20px;
    color: #2c3e50;
    grid-column: 1 / span 3;
    text-align: center;
  }

  .description {
    font-size: 1.2em;
    color: #555;
    border: 2px solid gold;
    border-radius: 10px;
    padding: 10px; 
    background-color: #ffffff;
    max-width: 500px;
    margin: 10px 60px; 
  }

  .description-left {
    grid-column: 1;
  }

  .description-right {
    grid-column: 3;
  }

  .carousel {
    grid-column: 2;
    display: flex;
    align-items: center;
    justify-content: center;

    img {
      width: 800px;
      height: auto;
      object-fit: cover;
      border: 3px solid gold;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
    }
  }

  .thumbnails {
    grid-column: 1 / span 3;
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    margin-top: 20px;

    img {
      width: 100px;
      height: 100px;
      object-fit: cover;
      border-radius: 10px;
      border: 2px solid #ddd;
      margin: 5px;
      cursor: pointer;
      transition: border 0.3s ease;

      &.active {
        border: 2px solid gold;
      }

      &:hover {
        border: 2px solid gold;
      }
    }
  }
}

footer {
  background-color: #2c3e50;
  color: white;
  padding: 10px 0;
  text-align: center;
  position: fixed;
  bottom: 0;
  width: 100%;
  margin-top: auto;
}

.footer-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 10px;
}

.footer-content .left {
  flex: 1;
  text-align: left;
}

.footer-content .center {
  flex: 2;
  text-align: center;
}

.footer-content .right {
  flex: 1;
  text-align: right;
}

.footer-content .logo {
  height: 90px; /* Povećaj visinu loga */
  width: auto;  /* Automatski prilagodi širinu za očuvanje omjera */
  transform: scale(1.49); /* Skalira logo za 1.5 puta veću veličinu */
  transform-origin: top left; /* Postavi točku skaliranja na lijevo središte */
  padding-left: 50%; /* Ako je potrebno, dodaj malo paddinga s lijeve strane */
}

.footer-content .contact-info p {
  margin: 5px 0;
  font-size: 1em;
}

.footer-content .right {
  flex: 1;
  text-align: center; /* Centriraj cijeli sadržaj unutar .right */
}

.footer-content .right span {
  margin-left: 20px; /* Smanji margine za bolju ravnotežu */
  font-size: 1.7em;
  color: gold; /* Boja teksta zlatna */
  display: inline-block; /* Da margin-left bude učinkovit */
}

#stan1 .carousel img,
#stan2 .carousel img,
#stan3 .carousel img,
#surroundings .carousel img {
  width: 900px; 
  height: 700px;
  object-fit: cover;
}

#stan1 .description,
#stan2 .description,
#stan3 .description,
#surroundings .description {
  max-width: 900px;
}
</style>
