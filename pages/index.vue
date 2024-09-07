<template>
  <NuxtLayout name="ygency" :header="2" :footer="5" :singlePage="true">
    <!-- Hero Section Start -->
    <section class="hero-area-three pt-180 pb-70 rpt-115 rel z-1">
      <div class="container rel z-1">
        <div class="row pt-35">
          <div class="col-lg-8">
            <div class="hero-three-content wow fadeInLeft delay-0-2s">
              <h1>Hayalleriniz için en iyi çözüm.</h1>
              <p>
                Dijital gücün farkına yıllar önce varmış, her kesim ve sektörün
                ihtiyaç duyduğu kıymetli bilgileri ve hizmetleri bünyesinde
                barındırarak, 360 derece hizmet veriyoruz.
              </p>
              <NuxtLink href="services" class="theme-btn style-two"
                >Proje Başlat <i class="far fa-arrow-left"></i
              ></NuxtLink>
            </div>
          </div>
          <div class="col-lg-4">
            <div class="hero-right-image mt-20 wow fadeInUp delay-0-4s">
              <img src="/assets/images/hero/hero-right.png" alt="Hero" />
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Hero Section End -->

    <section class="service-three-area pt-70 pb-50 rpt-40 rel z-1">
      <div class="container">
        <div class="row justify-content-between align-items-center pb-35">
          <div class="col-xl-6 col-lg-8 col-sm-6">
            <div class="section-title wow fadeInLeft delay-0-2s">
              <span class="sub-title mb-15">Hizmetlerimiz</span>
              <h2>Web tasarım çözümleri sunuyoruz.</h2>
            </div>
          </div>
          <div class="col-lg-4 col-sm-6 text-lg-end">
            <div class="service-items-controls mobile-hide">
              <button class="service-items-prev slick-arrow">
                <i class="far fa-chevron-left"></i>
              </button>
              <button class="service-items-next slick-arrow">
                <i class="far fa-chevron-right"></i>
              </button>
            </div>
          </div>
        </div>
        <div class="service-items-active">
          <Swiper
            :modules="[
              SwiperAutoplay,
              SwiperNavigation,
              SwiperPagination,
              SwiperEffectCreative,
            ]"
            :slides-per-view="1"
            :loop="true"
            :autoplay="{
              delay: 5000,
              disableOnInteraction: true,
            }"
            :navigation="{
              nextEl: '.service-items-next',
              prevEl: '.service-items-prev',
            }"
            :pagination="{
              el: '.p-dot',
              clickable: true,
            }"
            :breakpoints="{
              640: {
                slidesPerView: 1,
              },
              767: {
                slidesPerView: 2,
                spaceBetween: 15,
              },
              1200: {
                slidesPerView: 3,
                spaceBetween: 15,
              },
            }"
          >
            <SwiperSlide class="service-three-item wow fadeInUp delay-0-2s">
              <div class="title-icon">
                <h5>
                  <NuxtLink href="service-details"
                    >Web Design From Figma</NuxtLink
                  >
                </h5>
                <img src="/assets/images/services/icon1.png" alt="Icon" />
              </div>
              <div class="content">
                <p>
                  Figma tasarımlarını gerçeğe dönüştürerek, göz alıcı ve
                  kullanıcı dostu web siteleri oluşturuyoruz.
                </p>
                <NuxtLink class="read-more style-two" href="service-details"
                  ><span>Read More</span> <i class="far fa-arrow-right"></i
                ></NuxtLink>
              </div>
            </SwiperSlide>
            <SwiperSlide class="service-three-item wow fadeInDown delay-0-2s">
              <div class="title-icon">
                <h5>
                  <NuxtLink href="service-details">Vue Development</NuxtLink>
                </h5>
                <img
                  src="/assets/images/services/vue.png"
                  alt="Icon"
                  width="50"
                />
              </div>
              <div class="content">
                <p>
                  Vue.js kullanarak performanslı ve kullanıcı dostu web
                  uygulamaları geliştiriyoruz.
                </p>
                <NuxtLink class="read-more style-two" href="service-details"
                  ><span>Read More</span> <i class="far fa-arrow-right"></i
                ></NuxtLink>
              </div>
            </SwiperSlide>
            <SwiperSlide class="service-three-item wow fadeInUp delay-0-2s">
              <div class="title-icon">
                <h5>
                  <NuxtLink href="service-details"
                    >WordPress Development</NuxtLink
                  >
                </h5>
                <img src="/assets/images/services/icon3.png" alt="Icon" />
              </div>
              <div class="content">
                <p>
                  Esnek ve özelleştirilebilir WordPress siteleri tasarlıyor ve
                  geliştiriyoruz.
                </p>
                <NuxtLink class="read-more style-two" href="service-details"
                  ><span>Read More</span> <i class="far fa-arrow-right"></i
                ></NuxtLink>
              </div>
            </SwiperSlide>
            <SwiperSlide class="service-three-item wow fadeInDown delay-0-2s">
              <div class="title-icon">
                <h5>
                  <NuxtLink href="service-details">Digital Marketing</NuxtLink>
                </h5>
                <img src="/assets/images/services/icon4.png" alt="Icon" />
              </div>
              <div class="content">
                <p>
                  Markanızı dijital dünyada büyütmek için stratejik pazarlama
                  çözümleri sunuyoruz.
                </p>
                <NuxtLink class="read-more style-two" href="service-details"
                  ><span>Read More</span> <i class="far fa-arrow-right"></i
                ></NuxtLink>
              </div>
            </SwiperSlide>
            <SwiperSlide class="service-three-item wow fadeInDown delay-0-2s">
              <div class="title-icon">
                <h5>
                  <NuxtLink href="service-details"
                    >PSD, Figma, XD to HTML Convert</NuxtLink
                  >
                </h5>
                <img src="/assets/images/services/icon2.png" alt="Icon" />
              </div>
              <div class="content">
                <p>
                  Tasarım dosyalarınızı (PSD, Figma, XD) modern ve responsive
                  HTML/CSS kodlarına dönüştürüyoruz.
                </p>
                <NuxtLink class="read-more style-two" href="service-details"
                  ><span>Read More</span> <i class="far fa-arrow-right"></i
                ></NuxtLink>
              </div>
            </SwiperSlide>
            <SwiperSlide class="service-three-item wow fadeInDown delay-0-2s">
              <div class="title-icon">
                <h5>
                  <NuxtLink href="service-details">React Development</NuxtLink>
                </h5>
                <img src="/assets/images/services/icon4.png" alt="Icon" />
              </div>
              <div class="content">
                <p>Sed persiciatis unde omnisey natus error voluptatem</p>
                <NuxtLink class="read-more style-two" href="service-details"
                  ><span>Read More</span> <i class="far fa-arrow-right"></i
                ></NuxtLink>
              </div>
            </SwiperSlide>
            <SwiperSlide class="service-three-item wow fadeInDown delay-0-2s">
              <div class="title-icon">
                <h5>
                  <NuxtLink href="service-details"
                    >UI / UX Development</NuxtLink
                  >
                </h5>
                <img src="/assets/images/services/icon4.png" alt="Icon" />
              </div>
              <div class="content">
                <p>
                  Kullanıcı deneyimini ön planda tutarak etkileyici ve işlevsel
                  arayüzler geliştiriyoruz.
                </p>
                <NuxtLink class="read-more style-two" href="service-details"
                  ><span>Read More</span> <i class="far fa-arrow-right"></i
                ></NuxtLink>
              </div>
            </SwiperSlide>
          </Swiper>
        </div>
        <div class="service-items-controls">
          <div class="service-items-dots">
            <div class="slick-dots p-dot"></div>
          </div>
        </div>
      </div>
    </section>

    <!-- About Us Area start -->
    <section class="about-area-five py-100 rpy-100 rel z-1">
      <div class="container container-1290">
        <div class="row justify-content-between align-items-center">
          <div class="col-lg-6">
            <div class="about-content-five">
              <div class="section-title mb-40 wow fadeInUp delay-0-2s">
                <span class="sub-title mb-15">Hakkımızda</span>
                <h2>Öncü Dijital Dönüşüm Ajansınız</h2>
              </div>
              <p>
                Teknolojinin gücüyle markanızı zirveye taşıyoruz. Vue.js ve
                WordPress geliştirmeden, dijital pazarlama stratejilerine kadar,
                her adımda yanınızdayız. Tasarımlarınızı modern web çözümlerine
                dönüştürüyor, kullanıcı deneyimini en üst seviyeye çıkartıyoruz.
              </p>
              <div class="authors-text mt-45 pt-50">
                <img src="/assets/images/about/author1.jpg" alt="Author" />
                <img src="/assets/images/about/author2.jpg" alt="Author" />
                <img src="/assets/images/about/author3.jpg" alt="Author" />
                <img src="/assets/images/about/author4.jpg" alt="Author" />
                <img src="/assets/images/about/author5.jpg" alt="Author" />
                <span class="text">
                  Dünyanın dört bir yanındaki
                  <span>1000+ Global</span> müşterimize hizmet vermekten gurur
                  duyuyoruz
                </span>
              </div>
            </div>
          </div>
          <div class="col-xl-5 col-lg-6">
            <div class="about-five-images rmt-50 wow fadeInRight delay-0-2s">
              <div class="image-one">
                <img
                  src="/assets/images/about/about-five1.jpg"
                  alt="About Image"
                />
              </div>
              <div class="about-five-shape">
                <img
                  src="/assets/images/about/about-five-bg.png"
                  alt="About Five Shape"
                />
              </div>
              <div class="image-two mt-30">
                <img
                  src="/assets/images/about/about-five2.jpg"
                  alt="About Image"
                />
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- About Us Area end -->

    <!-- Service Style Three start -->
    <!-- <section class="service-three-area pt-70 rpt-40 rel z-1">
      <div class="container">
        <div class="row justify-content-center">
          <div class="col-lg-7">
            <div
              class="section-title text-center mb-60 wow fadeInUp delay-0-2s"
            >
              <span class="sub-title mb-20">Hizmetlerimiz</span>
              <h2>Web tasarım çözümleri sunuyoruz.</h2>
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col-xl-3 col-lg-4 col-md-6">
            <div class="service-three-item wow fadeInUp delay-0-2s">
              <div class="title-icon">
                <h5>
                  <NuxtLink href="service-details"
                    >Web Design From Figma</NuxtLink
                  >
                </h5>
                <img src="/assets/images/services/icon1.png" alt="Icon" />
              </div>
              <div class="content">
                <p>We denounce with righteous indignation dislike beguile</p>
                <NuxtLink class="read-more style-two" href="service-details"
                  ><span>Read More</span> <i class="far fa-arrow-right"></i
                ></NuxtLink>
              </div>
            </div>
          </div>
          <div class="col-xl-3 col-lg-4 col-md-6">
            <div class="service-three-item wow fadeInDown delay-0-2s">
              <div class="title-icon">
                <h5>
                  <NuxtLink href="service-details"
                    >PSD, Figma, XD to HTML Convert</NuxtLink
                  >
                </h5>
                <img src="/assets/images/services/icon2.png" alt="Icon" />
              </div>
              <div class="content">
                <p>At vero eos et accusamus et dignissim ducimbl ditiis</p>
                <NuxtLink class="read-more style-two" href="service-details"
                  ><span>Read More</span> <i class="far fa-arrow-right"></i
                ></NuxtLink>
              </div>
            </div>
          </div>
          <div class="col-xl-3 col-lg-4 col-md-6">
            <div class="service-three-item wow fadeInUp delay-0-2s">
              <div class="title-icon">
                <h5>
                  <NuxtLink href="service-details"
                    >WordPress Development</NuxtLink
                  >
                </h5>
                <img src="/assets/images/services/icon3.png" alt="Icon" />
              </div>
              <div class="content">
                <p>To take trivial example which ever undertakes laborious</p>
                <NuxtLink class="read-more style-two" href="service-details"
                  ><span>Read More</span> <i class="far fa-arrow-right"></i
                ></NuxtLink>
              </div>
            </div>
          </div>
          <div class="col-xl-3 col-lg-4 col-md-6">
            <div class="service-three-item wow fadeInDown delay-0-2s">
              <div class="title-icon">
                <h5>
                  <NuxtLink href="service-details">React Development</NuxtLink>
                </h5>
                <img src="/assets/images/services/icon4.png" alt="Icon" />
              </div>
              <div class="content">
                <p>Sed persiciatis unde omnisey natus error voluptatem</p>
                <NuxtLink class="read-more style-two" href="service-details"
                  ><span>Read More</span> <i class="far fa-arrow-right"></i
                ></NuxtLink>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section> -->
    <!-- Service Style Three end -->

    <!-- Project Grid Area start -->
    <section class="project-grid-area pt-70 rpt-70 pb-10 rpb-25">
      <div class="container container-1210">
        <div class="d-flex justify-content-between align-items-center pb-25">
          <div class="col-xl-6 col-lg-8">
            <div class="section-title mb-30 wow fadeInLeft delay-0-2s">
              <span class="sub-title mb-15">Referanslarımız</span>
              <h2>Başarı yolculuğunda bize güvenenler.</h2>
            </div>
          </div>
          <div class="col-lg-4 text-lg-end">
            <NuxtLink
              href="projects"
              class="theme-btn mb-25 wow fadeInRight delay-0-2s"
              >Tüm Referanslar <i class="far fa-arrow-right"></i
            ></NuxtLink>
          </div>
        </div>
        <div class="row gap-90">
          <div class="col-lg-6">
            <div class="project-item">
              <div class="image wow fadeInUp delay-0-2s">
                <img
                src="/assets/images/projects/project3.png"
                  alt="Project Grid"
                />
              </div>
              <div class="content wow fadeInUp delay-0-2s">
                <NuxtLink href="projects" class="category">Focsel</NuxtLink>
                <h2>
                  <NuxtLink href="project-details"
                    >Web Tasarım / E-Ticaret / Sosyal Medya Yönetimi</NuxtLink
                  >
                </h2>
              </div>
            </div>
          </div>
          <div class="col-lg-6">
            <div class="project-item">
              <div class="image wow fadeInUp delay-0-2s">
                <img
                src="/assets/images/projects/project5.png"
                alt="Project Grid"
                />
              </div>
              <div class="content wow fadeInUp delay-0-2s">
                <NuxtLink href="projects" class="category">Yıldız İhale</NuxtLink>
                <h2>
                  <NuxtLink href="project-details"
                    >UI & UX / Web Tasarım / Front-End / Back-End</NuxtLink
                  >
                </h2>
              </div>
            </div>
          </div>
          <div class="col-lg-6">
            <div class="project-item">
              <div class="image wow fadeInUp delay-0-2s">
                <img
                  src="/assets/images/projects/mst.png"
                  alt="Project Grid"
                />
              </div>
              <div class="content wow fadeInUp delay-0-2s">
                <NuxtLink href="projects" class="category"
                  >MST Endüstriyel Sistemler</NuxtLink
                >
                <h2>
                  <NuxtLink href="project-details"
                    >Web Tasarım / Kurumsal Kimlik / Dijital Reklam Yönetimi</NuxtLink
                  >
                </h2>
              </div>
            </div>
          </div>
          <div class="col-lg-6">
            <div class="project-item">
              <div class="image wow fadeInUp delay-0-2s">
                <img
                  src="/assets/images/projects/tandoor.png"
                  alt="Project Grid"
                />
              </div>
              <div class="content wow fadeInUp delay-0-2s">
                <NuxtLink href="projects" class="category">Tandoor Lavaş</NuxtLink>
                <h2>
                  <NuxtLink href="project-details"
                    >UI / UX / Sosyal Medya Yönetimi / Video & Görsel Tasarım</NuxtLink
                  >
                </h2>
              </div>
            </div>
          </div>
          <div class="col-lg-6">
            <div class="project-item">
              <div class="image wow fadeInUp delay-0-2s">
                <img
                  src="/assets/images/projects/asra-kimya.png"
                  alt="Project Grid"
                />
              </div>
              <div class="content wow fadeInUp delay-0-2s">
                <NuxtLink href="projects" class="category"
                  >Asra Kimya</NuxtLink
                >
                <h2>
                  <NuxtLink href="project-details"
                    >Web Tasarım / Dijital Reklam Yönetimi</NuxtLink
                  >
                </h2>
              </div>
            </div>
          </div>
          <div class="col-lg-6">
            <div class="project-item">
              <div class="image wow fadeInUp delay-0-2s">
                <img
                  src="/assets/images/projects/noi.png"
                  alt="Project Grid"
                />
              </div>
              <div class="content wow fadeInUp delay-0-2s">
                <NuxtLink href="projects" class="category"
                  >Noi Bahçe</NuxtLink
                >
                <h2>
                  <NuxtLink href="project-details"
                    >UI & UX / Sosyal Medya Yönetimi / Dijital Reklam Yönetimi</NuxtLink
                  >
                </h2>
              </div>
            </div>
          </div>
          <div class="col-12 text-center mt-4 d-lg-none">
            <NuxtLink
              href="projects"
              class="theme-btn mb-20 wow fadeInRight delay-0-2s"
              >Tüm Referanslar <i class="far fa-arrow-right"></i
            ></NuxtLink>
          </div>
        </div>
      </div>
    </section>
    <!-- Project Grid Area end -->

    <!-- Why Choose start -->
    <section class="why-choose-area pt-70 rpt-70 pb-70 rpb-70">
      <div class="container">
        <div class="row align-items-center">
          <div class="col-xl-5">
            <div class="row">
              <div class="col-xl-11">
                <div
                  class="why-choose-left-content mb-30 rmb-55 wow fadeInLeft delay-0-2s"
                >
                  <div class="section-title mb-50">
                    <span class="sub-title mb-15">Neden Bizi Seçmelisiniz</span>
                    <h2>Bizimle Çalışmanın Avantajları</h2>
                  </div>
                  <h5>Uzmanlık ve Deneyim</h5>
                  <p>
                    5+ yıllık deneyimimizle, dijital dünyada markanızı en üst
                    seviyeye taşıyoruz.
                  </p>
                  <br />
                  <h5>Müşteri Odaklı Yaklaşım</h5>
                  <p>
                    Müşteri memnuniyeti bizim önceliğimizdir, bu yüzden her
                    projeye özel bir titizlikle yaklaşırız.
                  </p>
                  <NuxtLink class="theme-btn style-two mt-35" href="about"
                    >Daha Fazla Bilgi <i class="far fa-arrow-right"></i
                  ></NuxtLink>
                </div>
              </div>
            </div>
          </div>
          <div class="col-xl-7">
            <div class="row">
              <div class="col-md-6">
                <div class="service-item wow fadeInRight delay-0-2s">
                  <div class="icon">
                    <i class="fal fa-bezier-curve"></i>
                  </div>
                  <h5>
                    <NuxtLink href="service-details"
                      >Özelleştirilmiş Çözümler</NuxtLink
                    >
                  </h5>
                  <p>
                    Her marka benzersizdir; bu yüzden size özel çözümler
                    sunuyoruz.
                  </p>
                </div>
                <div class="service-item wow fadeInRight delay-0-3s">
                  <div class="icon">
                    <i class="fal fa-cogs"></i>
                  </div>
                  <h5>
                    <NuxtLink href="service-details">Sonuç Odaklılık</NuxtLink>
                  </h5>
                  <p>
                    Başarıyı hedefleyen stratejiler geliştiriyor ve uyguluyoruz.
                  </p>
                </div>
              </div>
              <div class="col-md-6">
                <div class="service-item mt-30 wow fadeInRight delay-0-4s">
                  <div class="icon">
                    <i class="fal fa-chart-pie"></i>
                  </div>
                  <h5>
                    <NuxtLink href="service-details"
                      >İleri Teknoloji Kullanımı</NuxtLink
                    >
                  </h5>
                  <p>
                    En yeni teknolojilerle projelerinizi geleceğe taşıyoruz.
                  </p>
                </div>
                <div class="service-item wow fadeInRight delay-0-5s">
                  <div class="icon">
                    <i class="fal fa-shield-cross"></i>
                  </div>
                  <h5>
                    <NuxtLink href="service-details"
                      >Güvenilirlik ve Şeffaflık</NuxtLink
                    >
                  </h5>
                  <p>
                    Şeffaf ve güvenilir bir iş ortağı olarak, her adımda sizinle
                    birlikteyiz.
                  </p>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Why Choose end -->

    <section class="faq-area pt-50 pb-70 rpb-75 rel z-1">
      <div class="container">
        <div class="row align-items-center gap-100">
         
          <div class="col-lg-12">
            <div class="faq-content-part wow fadeInRight delay-0-2s">
              <div class="section-title mb-60">
                <span class="sub-title mb-15">Sıkça Sorulan Sorular</span>
                <h2>Sıkça Sorulan Sorular</h2>
              </div>
              <div class="accordion" id="faq-accordion">
                <div class="accordion-item">
                  <h5 class="accordion-header">
                    <button
                      class="accordion-button"
                      data-bs-toggle="collapse"
                      data-bs-target="#collapseOne"
                    >
                    Kurumsal web tasarımı yaptırmak ne kadar sürer?
                    </button>
                  </h5>
                  <div
                    id="collapseOne"
                    class="accordion-collapse collapse"
                    data-bs-parent="#faq-accordion"
                  >
                    <div class="accordion-body">
                      <p>
                        Web tasarımı projesinin süresi, projenin karmaşıklığına ve müşteri ihtiyaçlarına göre değişir. 
                        Ancak genel olarak, basit bir kurumsal web sitesi 4-6 hafta arasında tamamlanabilir. 
                        Tasarım, içerik sağlama ve onay süreçlerinin zamanında ilerlemesi, bu süreyi etkileyebilir.
                      </p>
                    </div>
                  </div>
                </div>
                <div class="accordion-item">
                  <h5 class="accordion-header">
                    <button
                      class="accordion-button"
                      data-bs-toggle="collapse"
                      data-bs-target="#collapseTwo"
                    >
                    Özel yazılım geliştirme süreciniz nasıl işliyor?
                    </button>
                  </h5>
                  <div
                    id="collapseTwo"
                    class="accordion-collapse collapse"
                    data-bs-parent="#faq-accordion"
                  >
                    <div class="accordion-body">
                      <p>
                        Özel yazılım geliştirme süreci, müşterinin iş ihtiyaçlarının analiz edilmesiyle başlar. 
                        Daha sonra, yazılım mimarisi, kullanıcı arayüzü tasarımı, geliştirme, test ve devreye alma aşamaları izlenir. 
                        Yazılımın kapsamına göre süreç 3-6 ay sürebilir. 
                        Ayrıca, müşteriye özel çözümler sunulurken esneklik ve ölçeklenebilirlik ön planda tutulur.
                      </p>
                    </div>
                  </div>
                </div>
                <div class="accordion-item">
                  <h5 class="accordion-header">
                    <button
                      class="accordion-button"
                      data-bs-toggle="collapse"
                      data-bs-target="#collapseFive"
                    >
                    İçerik Yönetim Sistemi (CMS) kurulumunda hangi özellikler sunuluyor?
                    </button>
                  </h5>
                  <div
                    id="collapseFive"
                    class="accordion-collapse collapse"
                    data-bs-parent="#faq-accordion"
                  >
                    <div class="accordion-body">
                      <p>
                        CMS kurulumlarımız, kullanımı kolay arayüzler, içerik düzenleme araçları, medya yönetimi, SEO optimizasyon özellikleri ve çoklu dil desteği gibi temel fonksiyonları içerir. 
                        İhtiyaca göre özelleştirilmiş modüller eklenebilir, böylece işletmeniz içerikleri hızlı ve etkili bir şekilde yönetebilir.
                      </p>
                    </div>
                  </div>
                </div>
                <div class="accordion-item">
                  <h5 class="accordion-header">
                    <button
                      class="accordion-button"
                      data-bs-toggle="collapse"
                      data-bs-target="#collapseThree"
                    >
                    Kurumsal kimlik tasarımı süreci ne kadar sürer ve hangi materyalleri içerir?
                    </button>
                  </h5>
                  <div
                    id="collapseThree"
                    class="accordion-collapse collapse"
                    data-bs-parent="#faq-accordion"
                  >
                    <div class="accordion-body">
                      <p>
                        Kurumsal kimlik tasarımı, markanızın vizyonuna ve değerlerine uygun bir şekilde tasarlanır. 
                        Süreç, genellikle 4-6 hafta sürer ve logo, kartvizit, antetli kağıt, zarf, dijital materyaller gibi öğeleri içerir. 
                        Ayrıca, marka rehberi hazırlanarak tutarlı bir görsel kimlik sunulur.
                      </p>
                    </div>
                  </div>
                </div>
                <div class="accordion-item">
                  <h5 class="accordion-header">
                    <button
                      class="accordion-button"
                      data-bs-toggle="collapse"
                      data-bs-target="#collapseFour"
                    >
                    Sosyal medya yönetimi kapsamında hangi hizmetleri sunuyorsunuz?
                    </button>
                  </h5>
                  <div
                    id="collapseFour"
                    class="accordion-collapse collapse"
                    data-bs-parent="#faq-accordion"
                  >
                    <div class="accordion-body">
                      <p>
                        Sosyal medya yönetimi kapsamında, içerik planlama, görsel ve metin oluşturma, takipçi etkileşimi, kampanya yönetimi ve analiz raporlaması gibi hizmetler sunuyoruz. 
                        Ayrıca, farklı platformlarda marka bilinirliğini artırmak için hedef odaklı stratejiler geliştiriyoruz. 
                        Facebook, Instagram, LinkedIn, Twitter gibi popüler sosyal medya platformlarında aktif yönetim sağlıyoruz.
                      </p>
                    </div>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
      <div class="faq-shapes">
        <img
          class="shape left"
          src="/assets/images/shapes/ellipse-left.png"
          alt="Shape"
        />
        <img
          class="shape right"
          src="/assets/images/shapes/ellipse-right.png"
          alt="Shape"
        />
      </div>
    </section>

    <!-- Testimonial Area start -->
    <!-- <SlidersTestimonial /> -->
    <!-- Testimonial Area end -->

    <!-- Blog Style Four start -->
    <section class="blog-area-four pt-70 rpt-70 pb-70 rpb-70">
      <div class="container container-1290">
        <div class="row justify-content-center">
          <div class="col-xl-8 col-lg-10">
            <div
              class="section-title text-center mb-60 wow fadeInUp delay-0-2s"
            >
              <span class="sub-title mb-20">Blog</span>
              <h2>Blog Yazılarımızı Keşfedin, Güncel Kalın!</h2>
            </div>
          </div>
        </div>
        <div class="row">
          <div class="col-xl-4 col-md-6">
            <div class="blog-item style-three wow fadeInUp delay-0-2s">
              <div class="image">
                <img src="/assets/images/blog/blog-four1.jpg" alt="Blog" />
                <NuxtLink href="blog" class="category">Sosyal Medya</NuxtLink>
              </div>
              <div class="content">
                <ul class="blog-meta">
                  <li>
                    <i class="far fa-calendar-alt"></i>
                    <a href="#">4 Eylül 2024</a>
                  </li>
                </ul>
                <h5>
                  <NuxtLink href="blog-details"
                    >İnstagramın İş Hayatımızdaki Yeri</NuxtLink
                  >
                </h5>
                <div class="author">
                  <img
                    src="/assets/images/blog/blog-author1.jpg"
                    alt="Author"
                  />
                  <span class="name">Bernard R. Kay</span>
                </div>
              </div>
            </div>
          </div>
          <div class="col-xl-4 col-md-6">
            <div class="blog-item style-three wow fadeInUp delay-0-4s">
              <div class="image">
                <img src="/assets/images/blog/blog-four2.jpg" alt="Blog" />
                <NuxtLink href="blog" class="category">Yazılım</NuxtLink>
              </div>
              <div class="content">
                <ul class="blog-meta">
                  <li>
                    <i class="far fa-calendar-alt"></i>
                    <a href="#">4 Temmuz 2024</a>
                  </li>
                </ul>
                <h5>
                  <NuxtLink href="blog-details"
                    >Yazılım Hizmetlerinin Hayatımıza Faydaları Nelerdir?</NuxtLink
                  >
                </h5>
                <div class="author">
                  <img
                    src="/assets/images/blog/blog-author2.jpg"
                    alt="Author"
                  />
                  <span class="name">Bernard R. Kay</span>
                </div>
              </div>
            </div>
          </div>
          <div class="col-xl-4 col-md-6">
            <div class="blog-item style-three wow fadeInUp delay-0-6s">
              <div class="image">
                <img src="/assets/images/blog/blog-four3.jpg" alt="Blog" />
                <NuxtLink href="blog" class="category">Sosyal Medya</NuxtLink>
              </div>
              <div class="content">
                <ul class="blog-meta">
                  <li>
                    <i class="far fa-calendar-alt"></i>
                    <a href="#">1 Ağustos 2024</a>
                  </li>
                </ul>
                <h5>
                  <NuxtLink href="blog-details"
                    >İnstagram Algoritması Hakkında Bilmeniz Gerekenler</NuxtLink
                  >
                </h5>
                <div class="author">
                  <img
                    src="/assets/images/blog/blog-author3.jpg"
                    alt="Author"
                  />
                  <span class="name">Bernard R. Kay</span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>
    <!-- Blog Style Four end -->
  </NuxtLayout>
</template>

<script>
import { ygencyUtilits } from "~/utilits";

export default {
  name: "index",
  mounted() {
    ygencyUtilits.counterUp();
  },
};
</script>
