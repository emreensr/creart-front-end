<template>
  <!-- Scroll Top Button -->
  <button class="scroll-top scroll-to-target" @click="scrollTop()">
    <span class="far fa-chevron-double-up"></span>
    <svg class="progress-ring" width="60" height="60">
      <circle class="progress-ring__circle" stroke="white" stroke-width="4" fill="transparent" r="28" cx="30" cy="30"/>
    </svg>
  </button>
</template>

<script>
import { ygencyUtilits } from "~/utilits";

export default {
  name: "ScrollTop",
  mounted() {
    ygencyUtilits.scrollTop();
    this.handleScroll(); // Sayfa yüklendiğinde durumu kontrol et
    window.addEventListener("scroll", this.handleScroll);
  },
  beforeDestroy() {
    window.removeEventListener("scroll", this.handleScroll);
  },
  methods: {
    scrollTop() {
      window.scrollTo({ top: 0, behavior: "smooth" });
    },
    handleScroll() {
      const scrollTop = window.scrollY;
      const documentHeight = document.documentElement.scrollHeight;
      const windowHeight = window.innerHeight;
      const scrollPercent = (scrollTop / (documentHeight - windowHeight)) * 100;

      const button = document.querySelector(".scroll-top");
      const circle = document.querySelector(".progress-ring__circle");
      
      // Calculate the stroke-dashoffset based on scroll percentage
      const radius = circle.r.baseVal.value;
      const circumference = 2 * Math.PI * radius;
      const offset = circumference - (scrollPercent / 100) * circumference;

      circle.style.strokeDasharray = `${circumference} ${circumference}`;
      circle.style.strokeDashoffset = offset;

      // Butonun görünür olup olmayacağını kontrol et
      const isActive = scrollTop > 100; // 100px'den fazla kaydırılınca butonu aktif yap
      if (isActive) {
        button.classList.add('active');
      } else {
        button.classList.remove('active');
      }
    },
  },
};
</script>

