# pages/

In deze map komen **Page Objects** volgens het **Page Object Model (POM)**.  
Voorbeelden:
- `HomePage.ts` → zoekbalk, cookiebanner
- `SearchResultsPage.ts` → filters, sorteeropties, resultatenlijst
- `PDP.ts` → producttitel, prijs, beschikbaarheid, add-to-cart knop

Alle selectors en interacties zitten hier.  
Tests in `/tests` roepen alleen methodes uit de pages aan.
