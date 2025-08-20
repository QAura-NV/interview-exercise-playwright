# helpers/

In deze map komen **losse hulpfuncties** die in meerdere tests of pagina’s nodig zijn.  
Voorbeelden:
- `priceParser.ts` → parse “€12,99” naar een float
- `cookieHandler.ts` → cookiebanner accepteren/sluiten
- `interceptors.ts` → netwerkcalls blokkeren (bv. naar checkout)

Houd helpers klein en doelgericht. Vermijd businesslogica in helpers; die hoort in flows of pages.
