# Tillgänglighetslabbet

En komplett, statisk utbildningsmiljö för en heldagsutbildning i digital tillgänglighet. Deltagarna jämför en avsiktligt bristfällig ”före”-version av den fiktiva verksamheten Ådala servicecenter med en förbättrad ”efter”-version.

Webbplatsen använder endast HTML, CSS och vanlig JavaScript. Det finns inga externa beroenden, inga byggsteg och ingen databas.

> **Observera:** `before/` innehåller avsiktliga tillgänglighetsbrister med pedagogiskt syfte.

## Filstruktur

- `index.html` – tillgänglig startsida för utbildningsmiljön
- `assets/` – gemensam CSS, JavaScript och lokala bilder
- `before/` – avsiktligt bristfällig startsida och formulär
- `after/` – förbättrad startsida och formulär
- `facit.html` – utbildarens facit (inte länkat från övningssidorna)

## Öppna lokalt

Det går att dubbelklicka på `index.html`. För en miljö som bättre motsvarar GitHub Pages kan du också starta valfri enkel lokal webbserver i projektmappen, exempelvis med `python3 -m http.server 8000`, och sedan öppna `http://localhost:8000/`.

## Publicera med GitHub Pages

1. Skapa ett tomt repository på GitHub.
2. Lägg in filerna i repositoryts `main`-gren och skicka upp dem till GitHub.
3. Öppna **Settings → Pages** i repositoryt.
4. Under **Build and deployment**, välj **Deploy from a branch**.
5. Välj grenen **main** och mappen **/(root)**, och spara.
6. När publiceringen är klar finns sidan normalt på `https://anvandare.github.io/repositorynamn/`.

Alla interna länkar är relativa och fungerar därför när webbplatsen ligger under en sådan projektsökväg.

## För utbildaren

Facit finns direkt på `facit.html`. Adressen blir exempelvis `https://anvandare.github.io/repositorynamn/facit.html`. Dela inte länken med deltagarna före genomgången.

## Testning

Första versionen har kontrollerats i den Chromium-baserade inbyggda webbläsaren i normal desktopbredd och smala vyer. Den är byggd för aktuella versioner av Chrome, Edge, Firefox och Safari. Genomför gärna en egen kontroll i den webbläsare och skärmläsare som ska användas under utbildningen.

Deltagarna behöver inget GitHub-konto för att använda en publicerad webbplats.

Formuläret är en demonstration. Inga uppgifter skickas eller lagras; JavaScript stoppar inskickningen och visar återkoppling lokalt i webbläsaren. Be ändå deltagarna använda påhittade uppgifter.

## Avsiktliga problem i före-versionen

Före-versionen demonstrerar begränsade och dokumenterade problem med flödesomformning, textförstoring och ökade textavstånd, rubriker, alt-texter, tangentbord, fokus, fokusordning, etikett i namn, formuläretiketter, gruppering, instruktioner, obligatoriska fält, felmeddelanden och statusmeddelanden. Full beskrivning och WCAG-koppling finns i `facit.html`.
