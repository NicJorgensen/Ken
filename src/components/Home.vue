<template>
  <div class="hello">
    <div class="row">
      <Navbar class="col-sm-12"></Navbar>
      <div class="col-sm-10">
        <h1>Featured Book:</h1>
      </div>

      <div class="col-sm-10 featured">
        <div class="row">
          <div class="col-sm-4 featuredImg">
            <img src="../assets/book4.jpg" alt="Glory of the Emperor" class="featuredBook">
          </div>
          <div class="col-sm-8">
            <h3>Glory of the Emperor</h3>
            <h6>
              <i>Book Four of the Kusunoki Chronicles</i>
            </h6>
            <p>War has come. The Kumashatsu and their allies conquer wherever they fight. The Shogun is dead. The daimyo are
              divided, and falling one by one. Kusunoki Kanto has been captured and is losing his identity as a samurai to
              a ring that transforms him into a wolf. Kusunoki Akashi had been badly wounded and may not recover. But Akashi
              has also found a small glimmer of hope, hope in the form of an emperor chosen by the tama, the very power of
              the land of Shinkoku. But the Emperor faces the enormous challenge of persuading or forcing both samurai and
              shinobi to lay aside a thousand years of enmity and follow him to a final confrontation with the seemingly
              invincible barbarians; a challenge made all the harder by the fact that he is a mere boy. The only chance remaining
              for Shinkoku, the tama, the samurai and the shinobi is to rally behind the Glory of the Emperor.</p>
            <a class="btn amazon" href="https://www.amazon.com/dp/B06XZSVQCX?ref_=pe_2427780_160035660">Buy on Amazon</a>
          </div>
        </div>
      </div>

      <div class="col-sm-10 divider">
        <h1>Kusunoki Chronicles</h1>
      </div>

      <div class="col-sm-10">
        <div class="row books">
          <img src="../assets/book1.jpg" alt="" class="bookCover" @click="kusunoki = 1">
          <img src="../assets/book2.jpg" alt="" class="bookCover" @click="kusunoki = 2">
          <img src="../assets/book3.jpg" alt="" class="bookCover" @click="kusunoki = 3">
          <img src="../assets/book4.jpg" alt="" class="bookCover" @click="kusunoki = 4">
        </div>
      </div>

      <div class="col-sm-10 kusunoki">
        <div class="text-center" v-if="kusunoki == 1">
          <h3>Pride of the Samurai</h3>
          <h6>
            <i>Book One of the Kusunoki Chronicles</i>
          </h6>
          <p>synosis</p>
        </div>
        <div class="text-center" v-if="kusunoki == 2">
          <h3>Treachery of the Daimyo</h3>
          <h6>
            <i>Book Two of the Kusunoki Chronicles</i>
          </h6>
          <p>synosis</p>
        </div>
        <div class="text-center" v-if="kusunoki == 3">
          <h3>Might of the Barbarians</h3>
          <h6>
            <i>Book Three of the Kusunoki Chronicles</i>
          </h6>
          <p>synosis</p>
        </div>
        <div class="text-center" v-if="kusunoki == 4">
          <h3>Glory of the Emperor</h3>
          <h6>
            <i>Book Four of the Kusunoki Chronicles</i>
          </h6>
          <p>War has come. The Kumashatsu and their allies conquer wherever they fight. The Shogun is dead. The daimyo are divided,
            and falling one by one. Kusunoki Kanto has been captured and is losing his identity as a samurai to a ring that
            transforms him into a wolf. Kusunoki Akashi had been badly wounded and may not recover. But Akashi has also found
            a small glimmer of hope, hope in the form of an emperor chosen by the tama, the very power of the land of Shinkoku.
            But the Emperor faces the enormous challenge of persuading or forcing both samurai and shinobi to lay aside a
            thousand years of enmity and follow him to a final confrontation with the seemingly invincible barbarians; a
            challenge made all the harder by the fact that he is a mere boy. The only chance remaining for Shinkoku, the
            tama, the samurai and the shinobi is to rally behind the Glory of the Emperor.</p>
          <a class="btn amazon" href="https://www.amazon.com/dp/B06XZSVQCX?ref_=pe_2427780_160035660">Buy on Amazon</a>
        </div>
      </div>

    </div>
  </div>
</template>

<script>
  import Navbar from "../components/Navbar";
  export default {
    name: 'Home',
    data() {
      return {
        kusunoki: 1
      }
    },
    components: {
      Navbar
    }
  }
</script>

<style scoped>
  h1 {
    color: white;
  }

  .row {
    display: flex;
    justify-content: center
  }

  .featured {
    background-color: rgba(114, 139, 161, 0.75);
    min-height: 40vh;
    border-radius: 20px;
    text-align: center;
    margin: 10px;
  }

  .featuredImg {
    display: flex;
    align-items: center;
    justify-content: center;
  }

  .featuredBook {
    height: 35vh;
    margin: 10px;
  }

  p {
    line-height: 100%;
  }

  .amazon {
    background-color: silver;
    margin: 5px;
    color: #2c3e50;
    font-weight: 700
  }

  .divider {
    background-color: rgba(119, 170, 1, 0.75);
    min-height: 10vh;
    border-radius: 20px;
    margin: 10px;
    display: flex;
    justify-content: flex-start;
    align-items: center
  }

  .books {
    display: flex;
    justify-content: space-around
  }

  .bookCover {
    height: 35vh;
    cursor: pointer;
    margin: 5px;
  }

  .kusunoki {
    background-color: rgba(114, 139, 161, 0.75);
    min-height: 40vh;
    border-radius: 20px;
    margin: 10px;
  }
</style>