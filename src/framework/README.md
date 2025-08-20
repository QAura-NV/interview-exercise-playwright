# framework/

Deze map bevat de **kern van het testframework**. Hier definieer je de basisklassen en configuraties waarop de rest van je tests en page objects steunen.

## Bestanden

- **config.ts**
  - Bevat configuratie voor het framework (bijvoorbeeld environment settings, URL’s, testopties).
  - Kan gebruikt worden om dynamisch instellingen door te geven aan Playwright.

- **test.ts**
  - Wrapper rond `@playwright/test`.
  - Hier definieer je custom fixtures of extensies (bv. logging, reporting, baseURL).
  - Gebruik dit als centrale entrypoint i.p.v. direct `@playwright/test` te importeren.

- **base.component.ts**
  - Abstracte klasse voor herbruikbare UI-componenten.
  - Componenten (zoals headers, footers, zoekbalken) erven hier van en krijgen toegang tot Playwright `Page` object en helpers.

- **base.page.ts**
  - Abstracte basis voor Page Objects.
  - Bevat gedeelde logica (navigatie, algemene selectors, wacht-functies).
  - Alle specifieke pages (HomePage, SearchResultsPage, PDP, …) erven van deze klasse.
