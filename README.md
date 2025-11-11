# Planned Planthood

Våren nalkas (ish) och det är dags att börja planera sina planteringar!
En kund har bett om en enklare lösning för att få bättre koll på vilken planta som skall sås på vilken dag på vårkanten.
Kunden är ett kollektiv som har en stor gemensam kolonilott på innergården och det kan lätt bli oordning bland odlingar och odlare. Därför efterfrågar de en lösning på detta!

## Instruktioner

Du skall efter bästa förmåga konstruera **startsidan** i följande [Figma-skiss](https://www.figma.com/file/Hbrk29Q2rVzXiXcFWdTXDA/planned-planthood?type=design&node-id=0%3A1&mode=design&t=9CHtB0GGoxLhWLYf-1) i HTML och CSS. Till ert förfogande har ni lite [startkod](./startkod). Klona hem detta repo och sätt igång!

## Specifikationer

- Sidan har en max-bredd på 1000px.

## Övrigt

I mappen assets hittar ni de svg-ikoner som behövs för att återskapa Figma-skissen, och dessa får ni använda hur mycket ni vill. Bakgrundsbilderna däremot är "snodda" från Unsplash, vilket innebär att man i ett riktigt live-projekt som publiceras publikt måste credda fotografen. Detta är ingenting ni behöver bry er om i denna uppgift eftersom att lägga upp sin kod på Github för skolprojekt inte riktigt räknas, men det kan vara bra att ha det i åtanke framöver. Länkar till bilderna hittar ni i kommentarerna till varje bild i Figma-skissen.

## Fusk

Nedan finner ni dropdowns där jag gömt mina lösningsförslag för html-koden. Öppna på egen risk! :)

<details>
  <summary>Flexbox Header</summary>

  <pre><code>
  &lt;header class="header"&gt;
      &lt;section class="header-left-container"&gt;
          &lt;img
              src="./assets/plannedplanthoodlogo.svg"
              alt="Planned Planthood logotype"
              class="header-image"
          /&gt;
      &lt;/section&gt;
      &lt;section class="header-right-container"&gt;
          &lt;section class="header-top-container"&gt;
              &lt;img
                  src="./assets/seedling.svg"
                  alt="Seedling"
                  class="header-image"
              /&gt;
          &lt;/section&gt;
          &lt;section class="header-bottom-container"&gt;
              &lt;img
                  src="./assets/spade.svg"
                  alt="Spade"
                  class="header-image"
              /&gt;
          &lt;/section&gt;
      &lt;/section&gt;
  &lt;/header&gt;
  </code></pre>

</details>

<details>
  <summary>Grid Header</summary>

  <pre><code>
  &lt;header class="header"&gt;
      &lt;!-- Grid Header --&gt;
      &lt;section class="header-box header-box-large"&gt;
          &lt;img
              src="./assets/plannedplanthoodlogo.svg"
              alt="Planned Planthood logotype"
              class="header-image"
          /&gt;
      &lt;/section&gt;
      &lt;section class="header-box header-box-brown"&gt;
          &lt;img
              src="./assets/seedling.svg"
              alt="Seedling"
              class="header-image"
          /&gt;
      &lt;/section&gt;
      &lt;section class="header-box header-box-green"&gt;
          &lt;img
              src="./assets/spade.svg"
              alt="Spade"
              class="header-image"
          /&gt;
      &lt;/section&gt;
  &lt;/header&gt;
  </code></pre>

</details>

<details>
  <summary>Navigation</summary>

  <pre><code>
  &lt;nav class="navigation"&gt;
      &lt;a href="#" class="navigation-link"&gt;Planer&lt;/a&gt;
      &lt;a href="#" class="navigation-link"&gt;Historik&lt;/a&gt;
      &lt;a href="#" class="navigation-link"&gt;Tips&lt;/a&gt;
      &lt;a href="#" class="navigation-link"&gt;Logga in&lt;/a&gt;
  &lt;/nav&gt;
  </code></pre>

</details>

<details>
  <summary>Säsong att så</summary>

  <pre><code class="language-html">
  &lt;!-- Info Section "Säsong att så" --&gt;
  &lt;section class="info-section"&gt;
      &lt;h1 class="info-section-title"&gt;Planned Planthood&lt;/h1&gt;
      &lt;figure class="info-section-image-container"&gt;
          &lt;img
              src="./assets/seedpackage.svg"
              alt="Seed package"
              class="info-section-image"
          /&gt;
      &lt;/figure&gt;
      &lt;article class="info-section-article"&gt;
          &lt;h2 class="info-section-subtitle"&gt;Säsong att så&lt;/h2&gt;
          &lt;p class="info-section-text"&gt;
              Våren är äntligen här i kollektivet! &lt;br /&gt;
              Lorem ipsum, dolor sit amet consectetur adipisicing
              elit. Ullam magnam quod earum dignissimos delectus rem!
          &lt;/p&gt;
          &lt;button class="info-section-button"&gt;Så-Tips&lt;/button&gt;
      &lt;/article&gt;
  &lt;/section&gt;
  </code></pre>

</details>

<details>
  <summary>Planerade planteringar</summary>

  <pre><code class="language-html">
  &lt;!-- Planned plants section --&gt;
  &lt;section class="plants-section"&gt;
      &lt;h2 class="plants-section-title"&gt;
          Våra planerade planteringar
      &lt;/h2&gt;
      &lt;section class="plants-grid"&gt;
          &lt;!-- Plant card --&gt;
          &lt;article class="plant"&gt;
              &lt;figure class="plant-image-container plant-cucumber"&gt;
                  &lt;img
                      src="./assets/plant.svg"
                      alt="Plant"
                      class="plant-logo"
                  /&gt;
              &lt;/figure&gt;
              &lt;section class="plant-details"&gt;
                  &lt;h3 class="plant-title"&gt;Gurka&lt;/h3&gt;
                  &lt;p class="plant-date"&gt;15 april 2024&lt;/p&gt;
                  &lt;p class="plant-user"&gt;Rico Coolio&lt;/p&gt;
                  &lt;button class="plant-button"&gt;Ta bort&lt;/button&gt;
              &lt;/section&gt;
          &lt;/article&gt;
          &lt;!-- Plant card --&gt;
          &lt;article class="plant"&gt;
              &lt;figure class="plant-image-container plant-tomato"&gt;
                  &lt;img
                      src="./assets/plant.svg"
                      alt="Plant"
                      class="plant-logo"
                  /&gt;
              &lt;/figure&gt;
              &lt;section class="plant-details"&gt;
                  &lt;h3 class="plant-title"&gt;Tomat&lt;/h3&gt;
                  &lt;p class="plant-date"&gt;1 april 2024&lt;/p&gt;
                  &lt;p class="plant-user"&gt;Jocke&lt;/p&gt;
                  &lt;button class="plant-button"&gt;Ta bort&lt;/button&gt;
              &lt;/section&gt;
          &lt;/article&gt;
          &lt;!-- Plant card --&gt;
          &lt;article class="plant"&gt;
              &lt;figure class="plant-image-container plant-tomato-2"&gt;
                  &lt;img
                      src="./assets/plant.svg"
                      alt="Plant"
                      class="plant-logo"
                  /&gt;
              &lt;/figure&gt;
              &lt;section class="plant-details"&gt;
                  &lt;h3 class="plant-title"&gt;Tomat&lt;/h3&gt;
                  &lt;p class="plant-date"&gt;1 april 2024&lt;/p&gt;
                  &lt;p class="plant-user"&gt;Majvor och P-Å&lt;/p&gt;
                  &lt;button class="plant-button"&gt;Ta bort&lt;/button&gt;
              &lt;/section&gt;
          &lt;/article&gt;
          &lt;!-- Plant card --&gt;
          &lt;article class="plant"&gt;
              &lt;figure class="plant-image-container plant-sugar-snaps"&gt;
                  &lt;img
                      src="./assets/plant.svg"
                      alt="Plant"
                      class="plant-logo"
                  /&gt;
              &lt;/figure&gt;
              &lt;section class="plant-details"&gt;
                  &lt;h3 class="plant-title"&gt;Sockerärtor&lt;/h3&gt;
                  &lt;p class="plant-date"&gt;15 april 2024&lt;/p&gt;
                  &lt;p class="plant-user"&gt;Frippe&lt;/p&gt;
                  &lt;button class="plant-button"&gt;Ta bort&lt;/button&gt;
              &lt;/section&gt;
          &lt;/article&gt;
          &lt;!-- Plant card --&gt;
          &lt;article class="plant"&gt;
              &lt;figure class="plant-image-container plant-turnip"&gt;
                  &lt;img
                      src="./assets/plant.svg"
                      alt="Plant"
                      class="plant-logo"
                  /&gt;
              &lt;/figure&gt;
              &lt;section class="plant-details"&gt;
                  &lt;h3 class="plant-title"&gt;Majrova&lt;/h3&gt;
                  &lt;p class="plant-date"&gt;1 april 2024&lt;/p&gt;
                  &lt;p class="plant-user"&gt;Emma på 4an&lt;/p&gt;
                  &lt;button class="plant-button"&gt;Ta bort&lt;/button&gt;
              &lt;/section&gt;
          &lt;/article&gt;
          &lt;!-- Plant card --&gt;
          &lt;article class="plant"&gt;
              &lt;figure class="plant-image-container plant-squash"&gt;
                  &lt;img
                      src="./assets/plant.svg"
                      alt="Plant"
                      class="plant-logo"
                  /&gt;
              &lt;/figure&gt;
              &lt;section class="plant-details"&gt;
                  &lt;h3 class="plant-title"&gt;Squash&lt;/h3&gt;
                  &lt;p class="plant-date"&gt;15 april 2024&lt;/p&gt;
                  &lt;p class="plant-user"&gt;Perra J&lt;/p&gt;
                  &lt;button class="plant-button"&gt;Ta bort&lt;/button&gt;
              &lt;/section&gt;
          &lt;/article&gt;
      &lt;/section&gt;
      &lt;button class="plants-more-button"&gt;Visa fler&lt;/button&gt;
  &lt;/section&gt;
  </code></pre>

</details>


<details>
  <summary>Våra tidigare odlingar</summary>

  <pre><code class="language-html">
  &lt;!-- Info Section "Våra tidigare odlingar" --&gt;
  &lt;section class="info-section"&gt;
      &lt;article class="info-section-article"&gt;
          &lt;h2 class="info-section-subtitle"&gt;
              Våra tidigare odlingar
          &lt;/h2&gt;
          &lt;p class="info-section-text"&gt;
              Våren är äntligen här i kollektivet! &lt;br /&gt;
              Lorem ipsum, dolor sit amet consectetur adipisicing
              elit. Ullam magnam quod earum dignissimos delectus rem!
          &lt;/p&gt;
          &lt;button
              class="info-section-button info-section-button-left"
          &gt;
              Planterade plantor
          &lt;/button&gt;
      &lt;/article&gt;
      &lt;figure class="info-section-image-container"&gt;
          &lt;img
              src="./assets/seedpackage.svg"
              alt="Seed package"
              class="info-section-image"
          /&gt;
      &lt;/figure&gt;
  &lt;/section&gt;
  </code></pre>

</details>


<details>
  <summary>Footer</summary>

  <pre><code class="language-html">
  &lt;footer class="footer"&gt;
      &lt;section class="footer-top"&gt;
          &lt;section class="footer-left-container"&gt;
              &lt;h2 class="footer-title"&gt;Vi hörs!&lt;/h2&gt;
              &lt;p class="footer-text"&gt;
                  &lt;i class="fa-solid fa-phone"&gt;&lt;/i&gt;
                  070-123 45 67
              &lt;/p&gt;
              &lt;p class="footer-text"&gt;
                  mail@mail.se &lt;i class="fa-solid fa-envelope"&gt;&lt;/i&gt;
              &lt;/p&gt;
          &lt;/section&gt;
          &lt;section class="footer-right-container"&gt;
              &lt;img
                  src="./assets/plannedplanthoodlogo.svg"
                  alt="Heart logo"
                  class="footer-image"
              /&gt;
          &lt;/section&gt;
      &lt;/section&gt;
      &lt;section class="footer-bottom"&gt;
          &lt;a href="/" class="footer-to-top-link"&gt;Till toppen av sidan&lt;/a&gt;
      &lt;/section&gt;
  &lt;/footer&gt;
  </code></pre>

</details>




