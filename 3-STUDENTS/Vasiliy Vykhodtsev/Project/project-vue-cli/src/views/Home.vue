<template>
<div>
<header class="header container">

  <div class="header__left">
    <a href="index.html" class="header__logo"><img src="@/assets/img/Group_2.png" alt="">Bran<span>d</span></a>

    <form class="header__search" method="get">
      <div class="browse">Browse <i class="fas fa-caret-down"></i></div>
      <input name="search" type="text" placeholder="Search for Item...">
      <button><i class="fas fa-search"></i></button>
    </form>

  </div>

  <div class="header__right">
    <a 
    href="#" 
    class="header__cart" 
    id="toggle-basket"
    @click="showBasket = !showBasket"
    >
              <img src="@/assets/img/Forma_1.svg" alt="card" class="header__cart-img">
    </a>
    <div class="drop-cart" v-show="showBasket">
                  <Basket ref="bask"/>
                  </div>
          <a href="#" class="button">My Account<i class="fas fa-caret-down"></i></a>
      </div>
</header>
<div class="header__line"></div>
<div class="topnav">
  <a href="#">Home</a>
  <a href="#">Man</a>
  <a href="#">Women</a>
  <a href="#">Kids</a>
  <a href="#">Accoseriese</a>
  <a href="#">Featured</a>
  <a href="#">Hot Deals</a>
</div>

<div class="content">

  <div class="brand__background">
    <div class="container brand">

      <div class="brand__text">THE BRAND<br><span>OF LUXERIOUS <span class="fashion">FASHION</span></span></div>

    </div>
  </div>

  <div class="deal container">
    <div class="men">
      <div class="hot__deal">hOT dEAL<br><span>FOR MEN</span></div>
    </div>
    <div class="accesories">
      <div class="hot__deal">LUXIROUS &amp; trendy<br><span>ACCESORIES</span></div>
    </div>
    <div class="women">
      <div class="hot__deal">30% offer<br><span>women</span></div>
    </div>
    <div class="kids">
      <div class="hot__deal">new arrivals<br><span>FOR kids</span></div>
    </div>

  </div>

  <div class="featured">
    <div class="featured__text">Featured Items<br><span>Shop for items based on what we featured in this week</span></div>

    <Catalog />

    </div>
  </div>

  <div class="browse__all">
    <a href="#" class="">Browse All Product <i class="fas fa-long-arrow-alt-right"></i></a>
  </div>

  <div class="info container">
    <div class="offer">
      <div class="offer__text">30% <span class="offer_inside">OFFER</span><br><span class="for__women">FOR WOMEN</span>
      </div>
    </div>
    <div class="bonus">
      <div class="bonus__main"><img src="@/assets/img/Forma_11.svg" alt="">
        <div class="bonus__info">
          <h2>Free Delivery</h2>
          <p>Worldwide delivery on all. Authorit tively morph next-generation innov tion with extensive models.</p>
        </div>
      </div>
      <div class="bonus__main"><img src="@/assets/img/Forma_12.svg" alt="">
        <div class="bonus__info">
          <h2>Sales &amp; discounts</h2>
          <p>Worldwide delivery on all. Authorit tively morph next-generation innov tion with extensive models.</p>
        </div>
      </div>
      <div class="bonus__main"><img src="@/assets/img/Forma_13.svg" alt="">
        <div class="bonus__info">
          <h2>Quality assurance</h2>
          <p>Worldwide delivery on all. Authorit tively morph next-generation innov tion with extensive models.</p>
        </div>
      </div>
    </div>

  </div>

  <div class="feedback__subscribe__back">
    <div class="feedback__subscribe container">
      <div class="feedback">
        <img src="@/assets/img/Layer_40.png" alt="">
        <div class="feedback__info">
          <p class="feedback__text">“Vestibulum quis porttitor dui! Quisque viverra nunc mi,
            a pulvinar purus condimentum a. Aliquam condimentum mattis neque sed pretium”</p>
          <p class="feedback__name"><span>Bin Burhan</span><br>
            Dhaka, Bd</p>
          <div class="pagination">
            <ul>
              <a href="">
                <li></li>
              </a>
              <a href="">
                <li class="active"></li>
              </a>
              <a href="">
                <li></li>
              </a>
            </ul>
          </div>
        </div>
      </div>


      <div class="subscribe">
        <h2>Subscribe</h2>
        <p>FOR OUR NEWLETTER AND PROMOTION</p>
        <form class="subscribe__form" method="get">
          <input name="search" type="email" placeholder="Enter Your Email">
          <button>Subscribe</button>
        </form>
      </div>

    </div>
  </div>
<footer class="footer container">

  <div class="footer__info">
    <div class="footer__logo">
      <img src="@/assets/img/Group_2.png" alt=""> Bran<span>d</span>
    </div>
    <div class="footer__text">
      <p>Objectively transition extensive data rather than cross functional solutions. Monotonectally syndicate multidisciplinary materials before go forward benefits. Intrinsicly syndicate an expanded array of processes and cross-unit partnerships.</p>
      <span>Efficiently plagiarize 24/365 action items and focused infomediaries.
        Distinctively seize superior initiatives for wireless technologies. Dynamically optimize.</span>
    </div>
  </div>
  <div class="footer__links">
    <div class="footer__link">
      <h2>COMPANY</h2>
      <a href="#">Home</a>
      <a href="#">Shop</a>
      <a href="#">About</a>
      <a href="#">How It Works</a>
      <a href="#">Contact</a>
    </div>
    <div class="footer__link">
      <h2>INFORMATION</h2>
      <a href="#">Terms &amp; Condition</a>
      <a href="#">Privacy Policy</a>
      <a href="#">How to Buy</a>
      <a href="#">How to Sell</a>
      <a href="#">Promotion</a>
    </div>
    <div class="footer__link">
      <h2>SHOP CATEGORY</h2>
      <a href="#">Men</a>
      <a href="#">Women</a>
      <a href="#">Child</a>
      <a href="#">Apparel</a>
      <a href="#">Browse All</a>
    </div>
  </div>
</footer>
<div class="media">
  <div class="media__inside container">
    <p>&copy; 2017 Brand All Rights Reserved.</p>
    <div class="media__links">
      <div class="media__link"><a href="#"><i class="fab fa-facebook-f"></i></a></div>
      <div class="media__link"><a href="#"><i class="fab fa-twitter"></i></a></div>
      <div class="media__link"><a href="#"><i class="fab fa-linkedin-in"></i></a></div>
      <div class="media__link"><a href="#"><i class="fab fa-pinterest-p"></i></a></div>
      <div class="media__link"><a href="#"><i class="fab fa-google-plus-g"></i></a></div>
    </div>
  </div>
</div>
</div>
</template>

<script>
// @ is an alias to /src
import Catalog from '@/components/Catalog.vue'
import Basket from '@/components/Basket.vue'
export default {
  name: 'Home',
  components: { Catalog, Basket },
  data() {
    return {
        showBasket: false
    }
  },
  methods: {
    get(url) {
        return fetch(url)
        .then(data => data.json())
    }
  },

}
</script>
