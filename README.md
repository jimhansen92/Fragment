# Fragment

Ett förstapersonsspel som körs direkt i webbläsaren, byggt med Three.js i en enda HTML-fil.
Du står i en platt sandstensarena med trälådor som skydd och möter en bot. Den som dödar vinner rundan,
och en ny runda börjar efter tre sekunder.

Rörelsen och vapnen är inspirerade av klassiska taktiska skjutspel: friktion och acceleration på marken,
air strafe och bunnyhopp, crouch-jump upp på lådor, sprayrekyl som klättrar och svänger, och spridning
som beror på om du står still, rör dig, hukar eller är i luften.

## Spela

Öppna `index.html` i en webbläsare (Chrome, Edge eller Firefox), eller spela via GitHub Pages om det är påslaget.
Klicka på knappen för att låsa musen. Ingen installation behövs.

## Kontroller

| Tangent | Funktion |
| --- | --- |
| W A S D | Gå |
| Mus | Titta runt |
| Mus1 | Skjut / hugg med kniven |
| Mus2 | Glock: burst · Kniv: stick |
| Space / scrollhjul | Hoppa |
| C eller Ctrl | Huka |
| Shift | Gå tyst |
| R | Ladda om |
| 1 / 2 / 3 | AK-47 / Glock-18 / Kniv |
| Q | Byt till senaste vapnet |
| N | Visa/dölj kompass |
| Esc | Pausa och öppna inställningar |

Tips: använd C för att huka. Ctrl + W stänger fliken i de flesta webbläsare.

## Innehåll

- **Vapen:** AK-47 (automatisk, 30/90), Glock-18 (halvautomat eller burst, 20/120) och kniv (hugg, stick, ryggstick).
- **Skada:** träffzoner (huvud ×4), rustning med hjälm, skada som avtar med avståndet och kulor som går igenom lådor (wallbang).
- **Bot:** rör sig mellan lådorna, ser dig bara med fri siktlinje, skjuter i salvor med rekyl och har tre svårighetsgrader.
- **Feedback:** hitmarker, synliga kulbanor, kulhål, dynamiskt hårkors och syntetiska ljud.
- **Inställningar:** nästan allt går att justera, till exempel rörelse, rekyl, spridning, känslighet, synfält, grafik och ljud.
  Inställningarna sparas i webbläsaren.

## Teknik

- En fil: `index.html` med HTML, CSS och JavaScript.
- [Three.js r128](https://threejs.org/) laddas från cdnjs.
- Alla modeller, texturer och ljud skapas i koden. Inga externa resurser behövs.

Fragment är ett fristående hobbyprojekt och har ingen koppling till Valve eller något annat spelföretag.
