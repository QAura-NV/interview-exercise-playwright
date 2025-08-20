# Take-home opdracht — SDET bol.com automatisering

Voor deze opdracht vragen we je om zelf een klein testautomatiseringsproject op te zetten tegen de live website van [bol.com](https://www.bol.com).

Het doel is om te laten zien:
- hoe jij een testproject structureert,  
- hoe je met Playwright (Typescript) werkt,  
- en hoe je best practices toepast in je code en je CI/CD pipeline.  

---

## Belangrijk
- Dit is een oefenopdracht en staat **volledig los van bol.com**.  
- Voer alleen de gevraagde scenario’s uit en respecteer de site:  
  - **geen bestellingen plaatsen**  
  - **geen accounts aanmaken**  
  - **geen persoonlijke data gebruiken**  

---

## Wat verwachten we van jou?

Je zet vanuit nul een **Node.js + Playwright project** op. In dit project automatiseer je **vier scenario’s**:

### 1. Homepage en zoekfunctie
- Open de homepage, sluit of accepteer de cookiebanner.  
- Controleer dat de zoekbalk zichtbaar is.  
- Zoek op bijvoorbeeld **“lego”**.  
- Controleer dat er resultaten verschijnen met **titel en prijs**.  
- Maak een screenshot van de resultatenpagina.  

### 2. Filteren en sorteren
- Pas een filter toe (bijvoorbeeld categorie of prijs).  
- Controleer dat de filter zichtbaar is (chip of breadcrumb).  
- Sorteer resultaten op **laagste prijs**.  
- Controleer dat de eerste drie prijzen correct oplopend zijn.  
- Maak een screenshot van de gesorteerde pagina.  

### 3. Productdetailpagina (PDP)
- Open het eerste zoekresultaat in een nieuwe tab.  
- Controleer dat **titel, prijs, beschikbaarheid en add-to-cart-knop** zichtbaar zijn.  
- **Intercepteer en blokkeer calls** naar cart/checkout zodat er geen echte acties gebeuren.  
- Klik veilig op add-to-cart en controleer dat je op de PDP blijft.  
- Maak screenshots vóór en na de klik.  

### 4. Paginering
- Verzamel de eerste vijf titels op pagina 1.  
- Ga naar pagina 2 en controleer dat de URL dit weerspiegelt.  
- Verzamel de eerste vijf titels van pagina 2 en controleer dat er **weinig overlap** is met pagina 1.  
- Maak screenshots van beide pagina’s.  

---

## Best practices die we willen zien
- Gebruik van **Page Object Model** en **helpers**.  
- **Robuuste selectors** i.p.v. fragiele CSS/XPath.  
- Rijke assertions met `expect`.  
- Screenshots en HTML-rapportage.  
- Netjes gestructureerde repo met duidelijke naamgeving.  

---

## Oplevering

De repo bevat:
- De code (**tests, pages, helpers**)  
- `README.md` met installatie- en run-instructies  
- `strategy.md` waarin je kort uitlegt hoe je de tests hebt opgezet, welke risico’s je zag, en hoe je flaky tests vermeden hebt  

Daarnaast configureer je een **CI/CD pipeline** (bijv. GitHub Actions) die:  
- Dependencies installeert  
- Playwright installeert  
- De tests uitvoert  
- Het **HTML-rapport en screenshots** als artifact publiceert  
- Gebruikt maakt van environment variabelen