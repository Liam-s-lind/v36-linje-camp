# v36-linje-camp

## Flex vs Grid

Trestegsmetoden: förklara → exemplifiera → motivera.

1. **Förklara:** Flexbox ordnar innehåll längs en huvudaxel, som en rad eller kolumn, och kan låta innehållet radbrytas. Grid ordnar innehåll i ett rutnät med både rader och kolumner.

2. **Exemplifiera:** I [style.css](style.css) använder `.tabla` `display: grid` och `grid-template-columns: 1fr 1fr`, vilket ger avgångarna två lika breda kolumner. Vid skärmbredder på högst 600 px ändrar en media query layouten till en kolumn med `grid-template-columns: 1fr`. Navigationen använder `display: flex` för att lägga länkarna på rad. Även `.kort-rad` använder Flexbox, med `flex-wrap: wrap` så att destinationskorten kan flytta till nästa rad. Kortens `flex: 1 1 200px` betyder att de får växa och krympa med 200 px som basstorlek.

3. **Motivera:** Jag använder Grid för avgångstavlan eftersom avgångarna ska ligga i tydliga, gemensamma kolumner. Flexbox passar navigationen eftersom länkarna följer en rad, och destinationskorten eftersom de ska kunna fördela utrymmet och radbrytas när det behövs. Även när Flexbox skapar flera rader fördelas utrymmet separat på varje rad, medan Grid håller kolumnerna gemensamma mellan raderna.

Jag valde två kolumner för Linje 47 eftersom det ger varje avgång mer utrymme och gör tider och destinationer lätta att läsa.

## Ägarskap

Jag kan förklara varje rad jag har pushat, och AI är ett verktyg — inte en ersättning för förståelse.
