<template>
  <footer class="main-footer footer-five pt-100">
    <div class="container container-1290 pb-40">
      <div class="row justify-content-between">
        <div class="col-lg-4">
          <div class="footer-widget footer-about wow fadeInUp delay-0-2s">
            <div class="footer-logo mb-25">
              <NuxtLink href="/"
              ><img
                src="/assets/images/logos/beyaz-logo.png"
                alt="Logo"
                title="Logo"
                width="180"
            /></NuxtLink>
            </div>
            <p>
              Dijital Çözüm Ortağınız
            </p>
          </div>
        </div>
        <div class="col-xl-3 col-lg-4 col-md-6">
          <div class="footer-widget footer-info wow fadeInUp delay-0-4s">
            <ul class="list-style-two">
              <li>
                <i class="far fa-envelope"></i>
                <a href="mailto:support@gmail.com">info@creart360.com</a>
              </li>
              <li>
                <i class="far fa-phone"></i>
                <a href="callto:05347459930">+90 (534) 745 99 30</a>
              </li>
              <li>
                <i class="far fa-clock"></i>
                <span>Pazartesi - Cuma, 9am - 6pm</span>
              </li>
            </ul>
          </div>
        </div>
        <div class="col-lg-4 col-md-6">
          <div class="social-style-one" style="margin-top:0px!important; gap:10px!important;">
            <a href="#"><i class="fab fa-twitter"></i></a>
            <a href="#"><i class="fab fa-facebook-f"></i></a>
            <a href="#"><i class="fab fa-instagram"></i></a>
            <a href="#"><i class="fab fa-pinterest-p"></i></a>
          </div>
        </div>
      </div>
    </div>
    <div class="copyright-area pt-25 pb-15">
      <div class="container">
        <div class="row">
          <div class="col-lg-6">
            <div class="footer-copyright-text wow fadeInUp delay-0-2s">
              <p>
                 @{{ new Date().getFullYear() }}
                <NuxtLink href="/">Creart360</NuxtLink> Tüm hakları saklıdır.
              </p>
            </div>
          </div>
          <div class="col-lg-6">
            <div
              class="footer-bottom-menu text-lg-end wow fadeInRight delay-0-2s"
            >
              <ul class="navigation onepage clearfix text-capitalize">
                <li><a href="/about">kurumsal</a></li>
                <li><a href="/services">hizmetlerimiz</a></li>
                <li><a href="/projects">referanslar</a></li>
                <li><a href="/blog">blog</a></li>
                <li><a href="/contact">iletişim</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer5",
};
</script>
