<script setup lang="ts">
import WelcomeItem from "./WelcomeItem.vue";
import DocumentationIcon from "./icons/IconDocumentation.vue";
import ToolingIcon from "./icons/IconTooling.vue";
import EcosystemIcon from "./icons/IconEcosystem.vue";
import CommunityIcon from "./icons/IconCommunity.vue";
import SupportIcon from "./icons/IconSupport.vue";
</script>

<script lang="ts">
export default {
  data: function () {
    return {
      userData: [
        {
          nama: "",
          email: "",
        },
      ],
    };
  },
  methods: {
    setData(nama, email) {
      this.nama = nama;
      this.email = email;
    },
  },
};
</script>

<template>
  <div class="text-center hero-section">
    <h1 class="display-5 fw-bold white-text">Organics Beauty Tips</h1>
    <div class="col-lg-6 mx-auto">
      <p class="lead mb-4 white-text">Find your daily beauty tips here</p>
      <div class="d-grid gap-2 d-sm-flex justify-content-sm-center">
        <a href="#about"><button type="button" class="btn btn-primary btn-lg px-4 gap-3">About Us</button></a>
        <a href="#product"
          ><button type="button" class="btn btn-outline-secondary btn-lg px-4">Produk</button></a
        >
      </div>
    </div>
  </div>

  <!--About-->
  <section id="about" class="shapedividers_com-3314 pb-5 pt-5" style="background-color: #c3c3d5">
    <div class="container text-center" style="padding: 85px 0">
      <div class="row">
        <div class="col"></div>
        <div class="col-10">
          <h2>About Us</h2>
          <div>
            <p class="fs-5">
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
              labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
              laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in
              voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat
              non proident, sunt in culpa qui officia deserunt mollit anim id est laborum
            </p>
            <br />
            <br />
            <a href="#jenis-kulit">
              <button type="button" class="btn btn-primary">Read More</button>
            </a>
          </div>
        </div>
        <div class="col"></div>
      </div>
    </div>
  </section>

  <!--Jenis Kulit-->
  <section id="jenis-kulit" class="shapedividers_com-7203 pb-5">
    <div class="container-xxl">
      <div class="row text-center mb-3 mt-5">
        <div class="col">
          <h2>Kenali Jenis Kulitmu</h2>
          <p class="fs-4">Manakah yang termasuk jenis kulit wajahmu?</p>
        </div>
      </div>
      <div class="row justify-content-center align-items-center mt-4 mb-5">
        <div class="col-sm-6 cust-inner-column responsive">
          <h3 class="fw-bold responsive-center">Kulit Wajah Kering</h3>
          <p>
            Kulit wajah kering umumnya terjadi akibat rendahnya tingkat kelembapan pada lapisan kulit terluar.
            Hal ini mengakibatkan kulit kering mudah pecah-pecah dan mengalami keretakan pada permukaan kulit.
            Pemilik kulit wajah kering biasanya memiliki pori-pori kulit yang hampir tak terlihat, permukaan
            luar kulit terlihat kasar dan kusam, serta kulit kurang elastis. Jenis kulit ini juga lebih mudah
            memerah, gatal, bersisik, dan meradang.
          </p>
        </div>
        <div class="col-md-6 cust-inner-column">
          <div class="cust-img-container">
            <img src="./images/1.jpg" alt="Kulit Kering" class="img-fluid" />
          </div>
        </div>
      </div>
      <div>
        <div class="row justify-content-center align-items-center mt-4 mb-5">
          <div class="col-md-6 cust-inner-column">
            <div class="cust-img-container">
              <img src="./images/2.jpg" alt="Kulit Berminyak" class="img-fluid" />
            </div>
          </div>
          <div class="col-md-6 cust-inner-column responsive">
            <h3 class="fw-bold responsive-center">Kulit Wajah Berminyak</h3>
            <p>
              Jenis kulit wajah berminyak cenderung licin dan mengkilap karena produksi minyak atau sebum yang
              berlebih. Sebum dihasilkan secara alami oleh kelenjar minyak atau kelenjar sebaceous di bawah
              permukaan kulit. Meski sebum berfungsi untuk melindungi dan melembapkan kulit, namun kelebihan
              sebum akan menyebabkan kulit wajah menjadi berminyak, pori-pori tersumbat, dan membuat kulit
              rentan mengalami jerawat. Jenis kulit wajah berminyak cenderung memiliki pori-pori besar,
              terlihat berkilau namun kusam, dan biasanya disertai komedo, jerawat, serta noda hitam.
            </p>
          </div>
        </div>
      </div>
    </div>

    <div>
      <div class="row justify-content-center align-items-center mt-4 mb-5">
        <div class="col-md-6 cust-inner-column responsive">
          <h3 class="fw-bold responsive-center">Kulit Wajah Kombinasi</h3>
          <p>
            Jenis kulit wajah kombinasi adalah perpaduan antara kulit berminyak dan kulit kering. Seseorang
            dengan jenis kulit wajah ini memiliki kulit berminyak di zona T, yaitu area dagu, hidung, dan
            dahi, serta kulit kering di area pipi. Jenis kulit wajah ini dapat dipengaruhi oleh faktor genetik
            dan peningkatan hormon selama masa pubertas.
          </p>
        </div>
        <div class="col-md-6 cust-inner-column">
          <div class="cust-img-container">
            <img src="./images/3.jpg" alt="Kulit Kering" class="img-fluid" />
          </div>
        </div>
      </div>
      <div></div>
    </div>
    <!-- <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1440 320">
        <path
          fill="#f2f2f2"
          fill-opacity="1"
          d="M0,128L20,106.7C40,85,80,43,120,69.3C160,96,200,192,240,202.7C280,213,320,139,360,117.3C400,96,440,128,480,117.3C520,107,560,53,600,74.7C640,96,680,192,720,213.3C760,235,800,181,840,160C880,139,920,149,960,165.3C1000,181,1040,203,1080,186.7C1120,171,1160,117,1200,101.3C1240,85,1280,107,1320,112C1360,117,1400,107,1420,101.3L1440,96L1440,320L1420,320C1400,320,1360,320,1320,320C1280,320,1240,320,1200,320C1160,320,1120,320,1080,320C1040,320,1000,320,960,320C920,320,880,320,840,320C800,320,760,320,720,320C680,320,640,320,600,320C560,320,520,320,480,320C440,320,400,320,360,320C320,320,280,320,240,320C200,320,160,320,120,320C80,320,40,320,20,320L0,320Z"
        ></path>
      </svg> -->
  </section>

  <!--alternative rekomendasi product-->
  <section id="product" class="pt-5 pb-5" style="background-color: #a77a95">
    <div class="row">
      <div class="col-sm-3 align-middle responsive-center">
        <h3 class="white-text align-middle">Rekomendasi produk</h3>
        <p class="white-text">
          Lorem Ipsum is simply dummy text of the printing and typesetting industry. Lorem Ipsum has been the
          industry's standard dummy text ever since the 1500s, when an unknown printer took a galley of type
          and scrambled it to make a type specimen book.
        </p>
        <a href="https://www.tokopedia.com/avoskinofficial" target="_blank" class="btn btn-primary px-4 py-2"
          >Shop Now <span class="material-symbols-outlined"> arrow_forward </span>
        </a>
      </div>
      <div class="col-sm-9">
        <div class="row">
          <div class="col-sm responsive">
            <!--card 1-->
            <div class="card">
              <img src="./images/a.jpg" class="card-img-top" alt="..." />
              <div class="card-body py-4 px-4">
                <h5 class="card-title">Facial Wash</h5>
                <p class="card-text flex-fill">
                  Membersihkan kulit wajah sekaligus mencerahkan dan melembapkan kulit. Dengan kandungan utama
                  kojic acid, ekstrak kelapa, lavender, dan minyak zaitun.
                </p>
              </div>
            </div>
          </div>

          <div class="col-sm responsive">
            <!--card 2-->
            <div class="card">
              <img src="./images/b.jpg" class="card-img-top" alt="..." />
              <div class="card-body py-4 px-4">
                <h5 class="card-title">Acne Serum</h5>
                <p class="card-text flex-fill">
                  Serum dengan kandungan Lactic Acid, Niacinamide, dan Kiwi Extract yang bermanfaat sebagai
                  anti aging agent melalui eksfoliasi lapisan kulit terluar.
                </p>
              </div>
            </div>
          </div>

          <div class="col-sm responsive">
            <!--card 3-->
            <div class="card">
              <img src="./images/d.jpg" class="card-img-top" alt="..." />
              <div class="card-body py-4 px-4">
                <h5 class="card-title">MiSolo YSB Vitamin C Set</h5>
                <p class="card-text flex-fill">
                  Rangkaian Your Skin Bae Series dengan kandungan utama vitamin C yang bekerja untuk
                  menghambat produksi serta akumulasi melanin pada kulit, sehingga efektif mencerahkan kulit
                  wajah.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!--Artikel-->
  <section id="artikel" class="mb-5">
    <div>
      <div class="row text-center mb-3 mt-5">
        <div class="col">
          <h2>Artikel</h2>
          <p class="fs-4">Baca artikel terbaru kami</p>
        </div>
      </div>
      <div class="row px-4">
        <div class="col-sm responsive">
          <div class="card">
            <img src="./images/pexels-ron-lach-10222456.jpg" class="card-img-top" alt="..." />
            <div class="card-body px-3 py-4">
              <h4>Artikel 1</h4>
              <p class="card-text">
                Some quick example text to build on the card title and make up the bulk of the card's content.
              </p>
              <a href="#" class="btn btn-primary">Read more</a>
            </div>
          </div>
        </div>
        <div class="col-sm">
          <div class="card responsive">
            <img src="./images/pexels-ivan-samkov-4491158.jpg" class="card-img-top" alt="..." />
            <div class="card-body px-3 py-4">
              <h4>Artikel 2</h4>
              <p class="card-text">
                Some quick example text to build on the card title and make up the bulk of the card's content.
              </p>
              <a href="#" class="btn btn-primary">Read more</a>
            </div>
          </div>
        </div>
        <div class="col-sm">
          <div class="card responsive">
            <img src="./images/pexels-karolina-grabowska-4202329.jpg" class="card-img-top" alt="..." />
            <div class="card-body px-3 py-4">
              <h4>Artikel 3</h4>
              <p class="card-text">
                Some quick example text to build on the card title and make up the bulk of the card's content.
              </p>
              <a href="#" class="btn btn-primary">Read more</a>
            </div>
          </div>
        </div>
        <div class="col-sm">
          <div class="card responsive">
            <img src="./images/pexels-ron-lach-10222456.jpg" class="card-img-top" alt="..." />
            <div class="card-body px-3 py-4">
              <h4>Artikel 4</h4>
              <p class="card-text">
                Some quick example text to build on the card title and make up the bulk of the card's content.
              </p>
              <a href="#" class="btn btn-primary">Read more</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!--contact-->
  <section id="subscribe">
    <div class="container mt-5">
      <div class="row text-center pb-5 pt-5">
        <div class="col">
          <h2>Subscribe for Our Newsletter</h2>
        </div>
      </div>
      <div class="row justify-content-center mb-3">
        <div class="col-2"></div>
        <div class="mb-3 col-sm-8" v-for="(user, index) in userData">
          <div class="form-floating mb-3">
            <input
              type="text"
              name="nama"
              class="form-control"
              id="floatingInput"
              placeholder="Nama kamu"
              v-model="user.nama"
            />
            <label for="floatingInput">Nama</label>
          </div>
          <div class="form-floating">
            <input
              type="email"
              name="email"
              class="form-control"
              id="floatingPassword"
              placeholder="name@example.com"
              v-model="user.email"
            />
            <label for="floatingPassword">Email</label>
          </div>
          <br />
          <!-- <button v-on:click="showText(user.nama, user.email)" class="btn btn-secondary">Subscribe Now</button> -->
          <button
            v-on:click="setData(user.nama, user.email)"
            data-bs-toggle="modal"
            data-bs-target="#ModalSubscribed"
            class="btn btn-secondary"
          >
            Subscribe Now
          </button>
        </div>
        <div class="col-sm-2"></div>
      </div>
    </div>
  </section>

  <!-- Modal -->
  <div
    class="modal fade"
    id="ModalSubscribed"
    tabindex="-1"
    aria-labelledby="ModalSubscribed"
    aria-hidden="true"
  >
    <div class="modal-dialog">
      <div class="modal-content">
        <div class="modal-header">
          <h5 class="modal-title" id="exampleModalLabel">Thank you for Subscribing!</h5>
          <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
        </div>
        <div class="modal-body px-5" v-for="(user, index) in userData">
          <p>
            Terima kasih telah berlangganan newletter kami, <strong>{{ user.nama }}</strong
            >. Silahkan periksa email kamu di <u>{{ user.email }}</u> agar tidak ketinggalan artikel terbaru
            dari ORGANICS BEAUTY TIPS.
          </p>
        </div>
        <div class="modal-footer">
          <button type="button" class="btn btn-secondary" data-bs-dismiss="modal">Close</button>
        </div>
      </div>
    </div>
  </div>

  <!-- Footer -->
  <footer class="bg-footer pt-3 pb-3">
    <div class="row align-items-center">
      <div class="col-sm-6 text-mobile">
        <img src="./images/organics_logo_white-transp.png" width="175" />
      </div>
      <div class="col-sm-6 px-4 text-right">
        <p>Created with <i class="fa fa-heart"></i> by Austenita Nasya Rafi</p>
      </div>
      <div class="col"></div>
    </div>
  </footer>
</template>
