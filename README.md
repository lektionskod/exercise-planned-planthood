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

  <pre><code>
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
          &lt;button class="info-section-button"&gt;Så-Tips&


