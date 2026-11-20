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
- [Three.js r128](https://threejs.org/) laddas från cdnjs, och GLTFLoader från jsDelivr.
- Botens soldatmodell laddas från `Model/terror1.glb` (med skelett och animationer). Om filen inte går att
  ladda används en enkel blockfigur. Banan, vapnen, texturerna och ljuden skapas i koden.

## Tack till

- Botens modell: ["PC Computer - Half-Life - HECU Grunt HD"](https://sketchfab.com/3d-models/pc-computer-half-life-hecu-grunt-hd-ba7e8074bd4345579ede43fa2795ffa3)
  av [8-Bit Play](https://sketchfab.com/8-bit_play), licens [CC-BY-4.0](http://creativecommons.org/licenses/by/4.0/).
  Ändrad: bara en huvudvariant och ett vapen visas, och animationernas förflyttning är borttagen.

Fragment är ett fristående hobbyprojekt och har ingen koppling till Valve eller något annat spelföretag.
