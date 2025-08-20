# tests/

Hier schrijf je je **Playwright testbestanden** (`*.spec.ts`).

Verplichte scenario’s:

1. **Homepage & Zoeken**
* Homepage en zoekfunctie
* Open de homepage, sluit of accepteer de cookiebanner.
* Controleer dat de zoekbalk zichtbaar is.
* Zoek op bijvoorbeeld “lego”.
* Controleer dat er resultaten verschijnen met titel en prijs.
* Maak een screenshot van de resultatenpagina.

2. **Filter & Sorteren**
* Pas een filter toe (bijvoorbeeld categorie of prijs).
* Controleer dat de filter zichtbaar is (chip of breadcrumb).
* Sorteer resultaten op laagste prijs.
* Controleer dat de eerste drie prijzen correct oplopend zijn.
* Screenshot van de gesorteerde pagina.

3. **PDP (Product Detail Page)**
* Open het eerste zoekresultaat in een nieuwe tab.
* Controleer dat titel, prijs, beschikbaarheid en de add-to-cart-knop zichtbaar zijn.
* Intercepteer en blokkeer calls naar cart/checkout zodat er geen echte acties gebeuren.
* Klik veilig op add-to-cart en controleer dat je op de PDP blijft.
* Screenshots vóór en na de klik.

4. **Paginering**
* Verzamel de eerste vijf titels op pagina 1.
* Ga naar pagina 2 en controleer dat de URL dit weerspiegelt.
* Verzamel de eerste vijf titels van pagina 2 en controleer dat er weinig overlap is met pagina 1.
* Screenshots van beide pagina’s.



