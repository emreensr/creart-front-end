<template>
  <!--Form Back Drop-->
  <div class="form-back-drop" @click="toggleSidebar()"></div>

  <!-- Hidden Sidebar -->
  <section class="hidden-bar project-start">
    <div class="inner-box text-center">
      <div class="cross-icon" @click="toggleSidebar()">
        <span class="fa fa-times"></span>
      </div>
      <div class="title mt-30">
        <h4>Hayalinizi gerçeğe dönüştürelim.</h4>
      </div>

      <!--Appointment Form-->
      <div class="appointment-form">
        <div class="form-group">
          <input type="text" placeholder="İsim" required />
          <input type="text" placeholder="Soyisim" required />
        </div>
        <div class="form-group">
          <input type="tel" placeholder="Telefon" required />
          <input type="email" placeholder="E-Posta" required />
        </div>
        <div class="checkbox-group required">
          <div class="md:col-span-3 sm:col-span-2 pb-4">
            <span class="label">
              Hangi hizmetlerden yararlanmak istiyorsunuz?
            </span>
          </div>
          <div class="checkbox-container">
            <div class="item">
              <div class="form-group">
                <label class="checkbox">
                  <input
                    id="services-1"
                    name="services[]"
                    value="1"
                    type="checkbox"
                  />
                  <span class="checkmark"></span>
                  <span>Kullanıcı Deneyimi Tasarımı (UX)</span>
                </label>
              </div>
            </div>
            <div class="item">
              <div class="form-group">
                <label class="checkbox">
                  <input
                    id="services-2"
                    name="services[]"
                    value="2"
                    type="checkbox"
                  />
                  <span class="checkmark"></span>
                  <span>Kurumsal Web Tasarım</span>
                </label>
              </div>
            </div>
            <div class="item">
              <div class="form-group">
                <label class="checkbox">
                  <input
                    id="services-3"
                    name="services[]"
                    value="3"
                    type="checkbox"
                  />
                  <span class="checkmark"></span>
                  <span>Mobil Uygulama Geliştirme</span>
                </label>
              </div>
            </div>
            <div class="item">
              <div class="form-group">
                <label class="checkbox">
                  <input
                    id="services-4"
                    name="services[]"
                    value="4"
                    type="checkbox"
                  />
                  <span class="checkmark"></span>
                  <span>E-Ticaret (B2B - B2C) Uygulamaları</span>
                </label>
              </div>
            </div>
            <div class="item">
              <div class="form-group">
                <label class="checkbox">
                  <input
                    id="services-5"
                    name="services[]"
                    value="5"
                    type="checkbox"
                  />
                  <span class="checkmark"></span>
                  <span>Özel Yazılım Geliştirme</span>
                </label>
              </div>
            </div>
            <div class="item">
              <div class="form-group">
                <label class="checkbox">
                  <input
                    id="services-6"
                    name="services[]"
                    value="6"
                    type="checkbox"
                  />
                  <span class="checkmark"></span>
                  <span>İçerik Yönetim Sistemi (CMS)</span>
                </label>
              </div>
            </div>
            <div class="item">
              <div class="form-group">
                <label class="checkbox">
                  <input
                    id="services-7"
                    name="services[]"
                    value="7"
                    type="checkbox"
                  />
                  <span class="checkmark"></span>
                  <span>Dijital Reklam Yönetimi</span>
                </label>
              </div>
            </div>
            <div class="item">
              <div class="form-group">
                <label class="checkbox">
                  <input
                    id="services-8"
                    name="services[]"
                    value="8"
                    type="checkbox"
                  />
                  <span class="checkmark"></span>
                  <span>Kurumsal Kimlik Tasarımı</span>
                </label>
              </div>
            </div>
            <div class="item">
              <div class="form-group">
                <label class="checkbox">
                  <input
                    id="services-9"
                    name="services[]"
                    value="9"
                    type="checkbox"
                  />
                  <span class="checkmark"></span>
                  <span>Logo Tasarımı</span>
                </label>
              </div>
            </div>
            <div class="item">
              <div class="form-group">
                <label class="checkbox">
                  <input
                    id="services-10"
                    name="services[]"
                    value="10"
                    type="checkbox"
                  />
                  <span class="checkmark"></span>
                  <span>Arama Motoru Optimizasyonu (SEO)</span>
                </label>
              </div>
            </div>
            <div class="item">
              <div class="form-group">
                <label class="checkbox">
                  <input
                    id="services-13"
                    name="services[]"
                    value="13"
                    type="checkbox"
                  />
                  <span class="checkmark"></span>
                  <span>Destek &amp; Bakım Hizmetleri</span>
                </label>
              </div>
            </div>
            <div class="item">
              <div class="form-group">
                <label class="checkbox">
                  <input
                    id="services-14"
                    name="services[]"
                    value="14"
                    type="checkbox"
                  />
                  <span class="checkmark"></span>
                  <span>Sosyal Medya Yönetimi</span>
                </label>
              </div>
            </div>
          </div>
          <div class="md:col-span-3 sm:col-span-2">
            <span class="message"></span>
          </div>
        </div>
        <div class="form-group">
          <button type="submit">Gönder</button>
        </div>
      </div>

      <!--Social Icons-->
      <div class="social-style-one">
        <a href="#"><i class="fab fa-twitter"></i></a>
        <a href="#"><i class="fab fa-facebook-f"></i></a>
        <a href="#"><i class="fab fa-instagram"></i></a>
        <a href="#"><i class="fab fa-pinterest-p"></i></a>
      </div>
    </div>
  </section>
  <!--End Hidden Sidebar -->
</template>

<script>
export default {
  name: "Sidebar",
  methods: {
    toggleSidebar() {
      document.querySelector("body").classList.toggle("side-content-visible");
    },
  },
};
</script>
