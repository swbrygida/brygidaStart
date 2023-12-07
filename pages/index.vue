<template>
    <main>
      <Dostepny />
      <Belka />
      <h1>Index</h1>
      <div class="indexMain">
        <div>
          <NuxtLink target="_blank" to="https://brygida-arch.vercel.app"
            ><img 
            alt="obrazek przedstawia starą, grubą księgę w barwach sepi"
            src="../public/foto/01.png" /> katalog zabytków z opisami</NuxtLink
          >
        </div>
        <div>
          <NuxtLink target="_blank" to="https://swbrygida.pl"
            ><img 
            alt="obrazek przedstawia obraz św. Brygidy w pozycji stojącej ze złożonymi do modlitwy rękami"
            src="../public/foto/04.png" />ilustrowana historia
          </NuxtLink>
        </div>
  
        <div>
          <NuxtLink target="_blank" to="https://brygida-model.vercel.app/"
            ><img 
            alt="obrazek przedstawia cyfrowy model pierwszej fazy budowy kościoła rektoralnego"
            src="../public/foto/03.png" />model układu kościoła</NuxtLink
          >
        </div>
  
        <div>
          <NuxtLink target="_blank" to="https://my.matterport.com/show/?m=ZTVZxKyLyMm"
            ><img 
            alt="obrazek przedstawia rzeżbione sklepienie prezbiterium kościoła rektoralnego"
            src="../public/foto/09.png" />spacer 3d po kosciele</NuxtLink
          >
        </div>
  
        <div>
          <NuxtLink target="_blank" to="https://www.youtube.com/embed/yIBfNPO_a6M"
            ><img 
            alt="obrazek przedstawia nawę środkową kościoła rektoralnego z ołtarzem w tle"
            src="../public/foto/05.png" />film o kosciele</NuxtLink
          >
        </div>
        <div>
          <NuxtLink target="_blank" to="/m1"
            ><img 
            alt="obrazek przedstawia makietę obecnej bryły kościoła rektoralnego wykonaną z plastiku"
            src="../public/foto/06.png" />makiety kościoła</NuxtLink
          >
        </div>
        <div>
          <NuxtLink target="_blank" to="https://swbrygida.pl/historia-ekspozycja-historyczna/"
            ><img 
            alt="obrazek przedstawia pełną zbroję rycerza Zakonu Krzyżackiego wraz z dwoma wbitymi obok mieczami"
            src="../public/foto/eh.jpg" />ekspozycja historyczna
          </NuxtLink>
        </div>
        <div>
          <NuxtLink target="_blank" to="https://swbrygida.pl/historia-ekspozycja-archeologiczna/"
            ><img 
            alt="obrazek przedstawia zrekonstruowaną trumnę ostatniej Ksieni Zakonu Brygidek"
            src="../public/foto/ea.jpg" />ekspozycja archeologiczna
          </NuxtLink>
        </div>
        <div>
          <NuxtLink target="_blank" to="https://swbrygida.pl/historia-ekspozycja-numizmatyczna/"
            ><img 
            alt="obrazek przedstawia gablotę z umieszczonymi w niej znaleziskami numizmatycznymi"
            src="../public/foto/en.jpg" />ekspozycja numizmatyczna
          </NuxtLink>
        </div>
        <div>
          <NuxtLink target="_blank" to="https://pobrygidkowski.pl/pl/audio.html"
            ><img 
            alt="obrazek przedstawia słuchawki gotowe do użycia"
            src="../public/foto/10.png" />audio - pełna historia</NuxtLink
          >
        </div>
        <div>
          <NuxtLink target="_blank" to="http://lublublin.pl/oltarz/index.html"
            ><img 
            alt="obrazek przedstawia ołtarz główny kościoła rektoralnego"
            src="../public/foto/08.png" />gigapanoramy ołtarzy</NuxtLink
          >
        </div>
        <div>
          <NuxtLink target="_blank" to="http://lublublin.pl/oltarz/100/index.html"
            ><img 
            alt="obrazek przedstawia widok z lotu ptaka na kościół rektoralny, wykonany w dzień"
            src="../public/foto/07.png" />panorama lotnicza</NuxtLink
          >
        </div>

      </div>
      <Stopka />
    </main>
  </template>
  
  <script setup>
  import gsap from 'gsap'


  onMounted(() => {
  const aa = document.querySelectorAll("a");
  gsap.from("body", 1, { opacity: 0 });
  gsap.from(aa, 1, { stagger: 0.3, delay: 1, opacity: 0 });
});

  </script>
  
  <style>
  h1 {
    display: none;
  }
  @media screen and (orientation: landscape) {
    .indexMain {
      padding: 8em 8em;
    }
  }
  @media screen and (orientation: portrait) {
  }
  .indexMain {
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: center;
    align-content: center;
  }
  .indexMain div {
    width: 246px;
    height: 350px;
    margin: 1em 1em 3em 1em;
    padding: 0;
    box-shadow: var(--shadow);
  }
  .indexMain div:hover {
    box-shadow: rgba(50, 50, 93, 0.25) 0px 50px 100px -20px,
      rgba(0, 0, 0, 0.3) 0px 30px 60px -30px, rgba(10, 37, 64, 0.35) 0px -2px 6px 0px inset;
  }
  .indexMain div img:hover {
    filter: grayscale(100%);
  }
  </style>