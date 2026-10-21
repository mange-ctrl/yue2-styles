# STYLES — vad du kan skriva i YuE2:s style-fält

*Referens för YuE2 Studio. Bygger på YuE2:s egen skrivguide (`writing_guide`), våra
testade stilar och mätningar på riktiga låtar. Uppdaterad 2026-10-21.*

---

## Snabbversionen

```
Språk, genre, sångröst, instrument, känsla, produktion, N BPM
```

Ett fält, engelska, kommaseparerat, **12–50 ord**, tempot **sist**. Inga instruktioner,
inga artister, inga låttitlar, ingen text.

---

## Reglerna (ordagrant från guiden)

> *"the style prompt YuE2 reads verbatim under its [Tags] header … comma-separated
> descriptors, 12-50 words, in this order … the language the vocals are sung in first;
> genre and subgenre; the lead vocal (gender, timbre, delivery) or 'instrumental'; the key
> instruments and textures; the mood and melodic character; the tempo as '<n> BPM' last."*

> *"Be concrete and musical — instruments and textures, not adjectives about quality."*

> *"The request has no tempo, key, negative-prompt or instruction field, so everything
> about the sound lives in these descriptors: never write instructions to the model
> ('make it…', 'the song should…') or anything that is not a descriptor."*

> *"Never put lyric lines, a song title or section instructions in the style."*

Tre saker som följer av det:

- **Ingen negativ prompt.** Vill du undvika något — beskriv det du vill höra i stället.
  Inte `no drums` utan `a cappella` eller `solo piano`.
- **Bara BPM får vara en siffra.** Inga `80 Hz`, inga `4 bars`, inga årtal som inte är genre.
- **Inga artister.** Inte `Fröken Snusk style` — beskriv ljudet i stället (det var just det
  som gled fel i en av dina låtar; se "Ord som inte funkar").

---

## 1. Språk — alltid först

| Ord | Vad det gör |
|---|---|
| `English` | säkrast, modersmål i träningen |
| `Mandarin` / `Japanese` / `Korean` | officiellt stödda |
| `Swedish` | **fungerar bra** (testat 2026-10-21), icke-officiellt men användbart |
| `instrumental` | ingen sång alls — står då där språket skulle stå |

Skriv språket som **adjektiv först i raden**. Övriga språk med latinska bokstäver
(spanska, italienska, tyska) brukar gå igenom eftersom modellen sjunger bokstäverna
den ser, men svenska är det vi verifierat.

---

## 2. Genre — inte paraplyord

Guiden: aldrig ett bart paraply som `rock` eller `pop` — var specifik, gärna med era-ord.

| Term | Drar mot |
|---|---|
| `Epadunk` / `Raggardunk` | svensk epa-traktor, 4x4, busig sång |
| `Eurodance` | 90-tal, supersaw, stor refräng |
| `Nordic Russmusik` | norsk/svensk russefest, hög energi |
| `Swedish pop` | ren, melodisk, radiovänlig |
| `synthpop` / `dark synth-pop` | syntdriven, 80-tal, ofta kall |
| `pop-punk` / `early 2000s pop-punk` | snabb, gitarr, tonår |
| `melodic death metal` | growl, dubbelkagge, melodi |
| `hip-hop` / `oldschool hiphop` | tal, break, sampling |
| `disco-funk` | 70-tal, livlig bas, stråkar |
| `afrobeats` | polyrytmik, percussion, varm |
| `reggaeton` | dembow-rytm, latin |
| `kpop` | polerad, hooks, gruppsång |
| `lofi` | dämpad, vinyl, mjuk |
| `country` | akustiskt, steel guitar, berättande |
| `indie rock` | gitarr, livekänsla |
| `house` | 4x4, klubb, sångsampling |
| `epic trailer` | orkester, stora trummor |
| `qawwali` | sydasiatisk devotional, harmonium |
| `chanson française` | fransk visa, dragspel |
| `canzone italiana` | italiensk schlager, stor röst |

---

## 3. Sångröst — kön, register, klang, leverans

**Kön / register**

`male vocal` · `female vocal` · `male and female duet` · `choir` · `gang vocals` ·
`child voice`

**Klang**

`bright` · `warm` · `airy` · `nasal` · `husky` · `gritty` · `smooth` · `deep` ·
`high-pitched` · `raspy` · `bell-like` · `breathy`

**Leverans**

`clean` · `shouted` · `spoken` · `whispered` · `belted` · `crooned` · `rapid-fire` ·
`unhurried phrasing` · `legato` · `staccato`

**Exempel på hela röst-delen**

```
gritty male tenor with shouted delivery
warm female pop vocal, unhurried phrasing
male and female duet, warm baritone and airy soprano
gang vocals with a bright female lead
```

Modellen har **inga rösttaggar i texten** — allt om rösten hör här. Två sångare
beskrivs här, aldrig som `[Male singer]` i låttexten.

---

## 4. Instrument

**Syntar**

| Term | Ljud |
|---|---|
| `supersaw synth lead` | 90-talets breda, sågiga lead |
| `hoover synth` | rave-hoover, aggressiv |
| `FM bell synth` | glasklocka, 80-tal |
| `arpeggiated synth` | pumpande arpeggio |
| `pluck synth` | kort, studsig |
| `synth pad` | lång, mjuk bakgrund |
| `square lead` | chip/retro |
| `wobble bass` | dubstep-vobbel |

**Bas**

| Term | Ljud |
|---|---|
| `sub-heavy club mix` | mastring med mycket under 120 Hz |
| `deep pumping offbeat bassline` | bas på offbeat, pumpar mellan kickarna |
| `808 sub bass with long sustain` | lång, djup 808 |
| `sidechained sub bass` | bas som duckar under kicken |
| `arpeggiated synth bass` | rullande basfigur |
| `slap bass` | funkig, perkussiv |
| `fingerstyle bass` | rund, akustisk känsla |
| `Reese bass` | bred, skev, dnb/techno |

**Trummor**

| Term | Ljud |
|---|---|
| `four-on-the-floor kick drum` | kick på varje slag |
| `4x4 kick` | samma sak, kortare |
| `punchy live drums` | riktiga trummor, hårt |
| `gated snare` | 80-talsvirvel med kort svans |
| `LinnDrum` / `TR-909` | klassiska trummaskiner |
| `breakbeat` | sampling av uppbrutet beat |
| `hand percussion` | congas, shaker, tamburin |
| `stomping drums` | fotstamp, stort |

**Gitarr**

`distorted power chords` · `crunchy overdriven electric guitars` · `clean jangle guitar` ·
`acoustic guitar` · `slide guitar` · `palm-muted riffs` · `fingerpicked`

**Klaviatur & folk**

`acoustic piano` · `Rhodes piano` · `church organ` · `accordion` · `harmonium` ·
`synthesizer strings` · `full string section` · `brass section` · `flute` · `banjo` ·
`sitar`

---

## 5. Produktion / mix

| Term | Vad det gör |
|---|---|
| `sub-heavy club mix` | mest energi under 120 Hz — **den enda basfras som bevisat sig** |
| `loud brickwall master` | hårt pressad, jämn, klubb |
| `dry mix` / `little reverb` | torrt, nära |
| `reverb-drenched` | stort, drömmigt |
| `wide stereo` | brett, pampigt |
| `tape saturation` | varm, mättad |
| `lo-fi` | dämpat, brusigt |
| `polished production` | rent, radiomässigt |
| `cheap but powerful` | B-känsla, kul |
| `sidechained` | duckar under kicken |
| `gated, punchy` | kort och hårt |

---

## 6. Känsla — två till fyra enkla ord

`rowdy` · `energetic` · `playful` · `party anthemic` · `nostalgic` · `melancholic` ·
`restless` · `sarcastic` · `buoyant` · `dreamy` · `menacing` · `triumphant` ·
`intimate` · `sweaty` · `late-night`

Skriv **känsla**, inte betyg: `rowdy energetic` funkar, `awesome vibes` gör inget.

---

## 7. Tempo — alltid sist, alltid `N BPM`

| Genre | Typiskt |
|---|---|
| ballad / visa | 60–90 |
| hip-hop / trap | 70–100 (halvtempo) |
| pop | 100–125 |
| disco / funk | 110–125 |
| house | 120–128 |
| Eurodance | 130–145 |
| **epadunk / raggardunk** | **135–150** |
| russmusik | 140–160 |
| pop-punk | 160–185 |
| metal | 160–220 |

---

## 8. Ord som **inte** funkar

| Skriv inte | Varför | Skriv i stället |
|---|---|---|
| `Deep bass` | värdeord — säger inget om vad som låter | `sub-heavy club mix` + `808 sub bass` |
| `phat`, `huge`, `massive` | samma sak | namnge instrumentet |
| `make the bass deep` | instruktion, inte beskrivning | beskriv ljudet |
| `Fröken Snusk style` | artistnamn — guiden förbjuder | `bright female vocal, Epadunk, 145 BPM` |
| `summer hit 2024` | låttitel/år | `Eurodance, party anthemic, 140 BPM` |
| `no drums`, `utan gitarr` | ingen negativ prompt finns | beskriv det som ska höras |
| `rock, pop, metal, jazz` | motstridiga genrer späder ut | välj en, låt instrumenten göra resten |
| 20 instrument på rad | över 50 ord tappar modellen fokus | 4–6 instrument räcker |

**Mätt bevis:** en låt med `Deep bass` i stilen landade på −22,4 dB i 90 Hz-bandet.
Våra låsta stilar som säger `sub-heavy club mix` + `deep pumping offbeat bassline`
ligger på −19 dB. Samma mjukvara, samma kedja — bara orden skiljer.

---

## 9. Våra låsta stilar (fungerar, ändra inte i onödan)

```
epadunk_v2 — 147 BPM
English, Eurodance, Nordic party anthem, 90s supersaw synth lead, four-on-the-floor kick drum,
deep pumping offbeat bassline, sub-heavy club mix, {vocal}, catchy pop hook, rowdy energetic, 147 BPM

mid_bass_party — 140 BPM
English, Epadunk, Swedish Raggardunk, Eurodance, Nordic Russmusik, heavy pumping bassline,
4x4 kick, 90s synth lead, catchy pop melody, {vocal}, party anthemic chorus, 140 BPM

sv_epadunk_v2 — 147 BPM
Swedish, Eurodance, Nordic party anthem, 90s supersaw synth lead, four-on-the-floor kick drum,
deep pumping offbeat bassline, sub-heavy club mix, {vocal}, catchy pop hook, rowdy energetic, 147 BPM

sv_mid_bass_party — 140 BPM
Swedish, Epadunk, Swedish Raggardunk, Eurodance, Nordic Russmusik, heavy pumping bassline,
4x4 kick, 90s synth lead, catchy pop melody, {vocal}, party anthemic chorus, 140 BPM
```

`{vocal}` byts per låt: `bright female alto` · `deep male baritone` · `airy female soprano` ·
`gritty male tenor` · `warm female pop` · `male and female duet, warm baritone and airy soprano`.

---

## 10. Färdiga mallar att klistra in

**Epadunk, svensk**
```
Swedish, Epadunk, Swedish Raggardunk, four-on-the-floor kick drum, deep pumping offbeat
bassline, sub-heavy club mix, bright female vocal, catchy pop hook, rowdy energetic, 145 BPM
```

**Eurodance-anthem**
```
English, Eurodance, 90s supersaw synth lead, four-on-the-floor kick drum, offbeat bass,
gritty male tenor with shouted delivery, party anthemic chorus, loud club mix, 140 BPM
```

**Ballad**
```
Swedish, piano ballad, warm female vocal, acoustic piano, soft string section,
intimate and unhurried, dry close mix, 72 BPM
```

**Pop-punk**
```
English, early 2000s pop-punk, nasal male tenor lead with gang-vocal shouts, distorted
power chords, driving eighth-note bass, punchy live drums, restless and buoyant,
tight dry mix, 172 BPM
```

**Hiphop**
```
Swedish, oldschool hiphop, conversational male voice, sampled soul loop, boom-bap drums,
upright bass, laid-back and confident, dusty tape mix, 92 BPM
```

**Synthwave**
```
English, dark synth-pop, breathy female vocal, arpeggiated synth bass, FM bell synth,
gated snare, dreamy and nostalgic, wide stereo reverb, 108 BPM
```

**Instrumental**
```
instrumental, epic trailer, full string section, brass section, stomping drums,
triumphant and menacing, huge reverb, 90 BPM
```

---

## 11. Felsökning

| Symptom | Trolig orsak | Åtgärd |
|---|---|---|
| Låten blev fel genre | paraplyord eller motstridiga genrer | en genre + konkreta instrument |
| Ingen botten | `deep bass`-typ av värdeord | `sub-heavy club mix`, `808 sub` |
| Rösten låter fel kön | rösten för vagt beskriven | `female vocal` / `male vocal` först i röst-delen |
| Allt låter likadant | samma stil varje gång | byt 1–2 instrument + röst, behåll resten |
| Modellen sjunger orden i stilen | style-texten råkade hamna i lyrikfältet | stilen hör i Style, bara sångrader i Lyrics |
| Låten blev för lång/kort | `duration` är ett tak, inte ett mål | antal sektioner styr längden |
| Svenska låter norskt | engelska lånord i texten | skriv om raden på ren svenska |

---

## 12. Vad style-fältet **inte** styr

Style beskriver ljudet och rösten — inget annat.

| Vill du styra | Hör i |
|---|---|
| Vers / refräng / instrumental / outro | låttextens taggar `[Verse 1]`, `[Chorus]`, `[Instrumental Break]` |
| Längd | antal sektioner (10 ≈ 2:45, 14 ≈ 4:10, 21 ≈ 5:20 vid 140–147 BPM) |
| Exakt melodi, ackord, taktart | ABC-noterna (`cot: "full"` eller egen score) |
| Hur slumpig harmoniken är | `harmony`: `strength`, `section_strength`, `outside_bonus` |
| Två sångare som turas om | röst i style + verser i texten — inga rösttaggar i lyriken |
| Mix, mastring, loudness | mastringskedjan efteråt (se §15) |
| Antal tagningar | `synth_batch_size`, `seed` |

Style kan alltså inte göra en låt kortare, byta taktart eller lägga in ett instrumentbreak —
det är taggarna och noterna.

---

## 13. Svensk → engelsk ordlista

Style skrivs alltid på engelska, även när låten sjungs på svenska.

| Du tänker | Skriv |
|---|---|
| djup bas | `sub-heavy`, `808 sub bass` |
| pumpande bas | `pumping bassline`, `offbeat bassline` |
| bas som duckar för kicken | `sidechained sub bass` |
| fyra på golvet | `four-on-the-floor kick` |
| virvel med kort svans | `gated snare` |
| 90-talssynt | `90s supersaw synth lead` |
| arpeggio | `arpeggiated synth` |
| mjuk matta | `synth pad` |
| skrikig sång | `shouted delivery` |
| viskande | `whispered` |
| ren och nära | `dry close mix` |
| stort och drömmigt | `reverb-drenched`, `wide stereo` |
| pressat och högt | `loud brickwall master` |
| ruffigt och billigt | `cheap but powerful production` |
| glad fest | `party anthemic`, `buoyant` |
| busig | `rowdy`, `playful` |
| nostalgisk | `nostalgic`, `melancholic` |
| suggestiv | `menacing`, `late-night` |

---

## 14. Mätbank — vad stilarna faktiskt ger

Uppmätta exempel från riktiga filer (samma motor, samma mastringskedja där inget annat sägs):

| Fil / stil | Loudness | True peak | LRA | 90 Hz-band |
|---|---|---|---|---|
| Källa `supa som riktiga män` (rå) | −14,2 LUFS | +0,3 dBFS | 3,4 LU | — |
| `supa` — mastrad, **bas-kedja** | −9,2 LUFS | +0,1 dBFS | 1,4 LU | −22,4 dB |
| `supa` — mastrad, **mid_bass_party** (+1 dB @ 90 Hz) | −9,2 LUFS | +0,1 dBFS | 1,4 LU | −21,9 dB |
| `Nattkörning` — mastrad epadunk_v2 | −9,5 LUFS | +0,1 dBFS | 2,1 LU | — |
| `Nattkörning` — mastrad mid_bass_party | — | — | — | −19,0 dB |

Två saker att dra slutsatser av:

1. **Loudness landar alltid på −9,2 till −9,5 LUFS** oavsett stil — det är mastringen som
   sätter nivån, inte style-texten.
2. **90 Hz-bandet skiljer sig åt.** `Deep bass` i stilen gav −22,4; `sub-heavy club mix` +
   `deep pumping offbeat bassline` gav −19,0 på en annan låt. Skillnaden är orden.

### Bastest 2026-10-21 — fem varianter

Samma text (Köksfesten), samma röst (`warm female pop`), samma tempo, alla mastrade med
baskedjan så loudness är utjämnad. Bara basfrasen byttes. Två tagningar per variant.
`diff` = 90 Hz-bandet minus 1 kHz-bandet — hur mycket basen sticker ut mot resten.

| Variant | Basfras i style | Längd | 90 Hz | 1 kHz | diff |
|---|---|---|---|---|---|
| **A** | `heavy pumping bassline, 4x4 kick` | 2:47 | −19,9 | −20,5 | **+0,6** |
| **B1** | `deep pumping offbeat bassline, sub-heavy club mix` | 3:20 | −19,4 | −22,9 | **+3,5** |
| **B2** | samma som B1 | 2:21 | −19,0 | −22,1 | **+3,1** |
| **C1** | `sidechained 808 sub bass under a four-on-the-floor kick` | 2:58 | −20,7 | −20,2 | **−0,5** |
| **C2** | samma som C1 | 2:19 | −21,0 | −21,4 | **+0,4** |

**Vad testet visar:**

- **B vinner klart:** +2,7 dB mer bas mot mellanregistret än grundstilen (A), och +3,3 dB
  mer än C. Skillnaden hörs, den är inte mätbrus.
- **C blev sämre än ingen basfras alls.** `sidechained` betyder att basen duckar för
  kicken — orden gjorde precis det de säger, och sänkte botten.
- **Längden påverkade inte resultatet:** B2 är kortast av alla (2:21) och har näst mest bas.
- **Slutsats:** `deep pumping offbeat bassline` + `sub-heavy club mix` är den formulering
  som ger mest botten i YuE2. Den bor i `epadunk_v2` — och kan lånas in i andra stilar.

Mästarna från testet ligger i `bastest/` om du vill lyssna själv.



---

## 15. Mastring som hör ihop med stilen

Stilarna har egna kedjor — de är en del av "stilen" och ska inte blandas.

**Baskedja (epadunk_v1, epadunk_v2, sv_epadunk_v2)**

```
equalizer=f=200:t=q:w=1:g=-2.5,
equalizer=f=500:t=q:w=1:g=2,
equalizer=f=3500:t=q:w=1.2:g=-2,
equalizer=f=9000:t=h:w=1:g=-3,
acompressor=threshold=-20dB:ratio=3:attack=8:release=120:makeup=2,
loudnorm=I=-9.6:TP=-0.3:LRA=6,
alimiter=limit=0.97
```

**mid_bass_party / sv_mid_bass_party** = `equalizer=f=90:t=q:w=1:g=1,` + baskedjan.

Historik: 90 Hz-höjningen var **+4 dB** först. Två nya generationer låg cirka 40 % högre i
sub-bas rå, så den sänktes till **+1 dB** 2026-10-20. Höjningen äts dessutom delvis upp av
kompressor och limiter — +1 dB på EQ:n gav **+0,5 dB** i mätningen.

Praktiskt vid export: `-ar 48000` (loudnorm arbetar internt i 192 kHz och ffmpeg behåller
den rate:en annars), `-c:a flac -compression_level 8`, `-vn` om du vill ha ren audio utan
coverbild.

---

## 16. Längd — antal sektioner, inte `duration`

`duration_seconds` är ett **tak**, inte ett mål. Modellen slutar när texten tar slut.
Uppmätt vid 140–147 BPM:

| Sektioner | Brukar bli |
|---|---|
| 10 | 2:41–2:48 |
| 14 | ca 4:10 |
| 21 | ca 5:21 |

Riktmärke: 10 sektioner ≈ 3 min, 14 ≈ 4 min, 18 ≈ 5 min, 24 ≈ 6 min.

**Padderregel när låten blir för kort:** om sista refrängen har **≤ 6 rader** sätts
`[Instrumental Break]` + en upprepad `[Chorus]` in före `[Outro]`. Det lyfte typiskt
162 s → 228 s. Är sista refrängen redan utskriven/exploderad (t.ex. 16 rader) hoppas
padden över — annars blir det för långt.

---

## 17. Röster — rotationen vi använt

| Röst | Karaktär | Passar |
|---|---|---|
| `bright female alto` | ljus, tydlig, pigg | epadunk, eurodance |
| `warm female pop` | mjuk, rund, radiovänlig | pop, mid_bass_party |
| `airy female soprano` | luftig, hög | duetter, ballad |
| `deep male baritone` | mörk, tung | raggardunk, allvar |
| `gritty male tenor` | raspig, busig | epadunk, rock |
| `male and female duet, warm baritone and airy soprano` | två röster | refränglyft |

Regler vi landat i:

- **Byt röst mellan låtarna** — annars smälter en 29-låtars batch ihop.
- **Samma text, olika röst** i de två stilarna ger tydlig A/B.
- **Perspektiv styr kön**: texter skrivna ur kvinnligt perspektiv (t.ex. "hennes mun",
  "tungan") fick kvinnlig röst i båda versionerna, oavsett stil.
- **Duett** användes på låtar med två personer i handlingen (t.ex. `Nattkörning`,
  `Två blir tre`).
- Rösten står **bara i style** — aldrig som `[Male singer]` i texten.

---

## 18. Adaptrar / LoRA — styrs utanför style

En LoRA är ett separat lager, inte en del av style-texten:

```
adapters: [{ id: "yue2-sv-billie", scales: { ar: 1, nar: 1 } }]
```

| Sak | Vad den gör |
|---|---|
| `scales` | styrka per slot, 0–1. Utelämnad = LoRans egna |
| `ar`-slot | påverkar komposition/melodi |
| `nar`-slot | påverkar ljud/sångklang |
| `companion_scale` | realaudio-dekodern, 0 = ren YuE2-checkpoint |

Installerat i studion: `yue2-sv-billie` (trigger `sv_billie`), ett gäng **slider-LoRAs**
(`yue2-slider-female`, `-male`, `-pop`, `-rock` … rank 8, lätta att smyga in) samt
genre-LoRAs (bulgarian-voices, canzone-italiana, dark-sufi, qawwali, militant-reggae …).

Två saker vi **inte** vet än, och som ska testas:

- om trigger-ordet `sv_billie` ska stå i **style** eller i **texten** för att slå till;
- om `yue2-sv-billie` gör svenskan bättre eller bara ändrar klangen.

Tills det är testat: behandla LoRA som en krydda, inte som en förutsättning — svenskan
fungerar redan utan.

**Testat 2026-10-21:** `yue2-sv-billie` sjunger **mumligt** — orden tappar
tydlighet. Använd den inte för texter där uttalet spelar roll. (Ingen mätning gjord, bara
lyssning — men det räcker för att prioritera bort den.)

---

## 19. När låtarna låter likadana

Ordningen att angripa det, från störst effekt till minst:

1. **Byt 1–2 instrument i style** — behåll genre och tempo, byt t.ex. `supersaw` mot
   `FM bell synth`, eller `four-on-the-floor` mot `breakbeat`.
2. **Byt röst** (se §17) — billigaste variationen som hörs direkt.
3. **Variera `seed` / `lm_seed`** — samma seed ger samma komposition.
4. **Rör harmoniken:** `harmony.strength` 6–10 bryter en loopande ackordföljd,
   `section_strength` ger varje sektion egen öppning, `outside_bonus` tar in ackord
   utanför tonarten.
5. **`cot`:** `"full"` låter modellen skriva melodi + ackord (mer variation mellan låtar),
   `"off"` hoppar över notplaneringen.
6. **Tempot 3–5 BPM** upp eller ner byter känsla utan att byta genre.

---

## 20. Så testar du en stiländring så att svaret betyder något

En enda låt säger ingenting — modellen varierar. Gör så här:

1. **Samma allt utom en sak.** Samma text, samma röst, samma längd, samma `steps`.
   Ändra bara frasen du vill mäta.
2. **Två tagningar per variant** (olika `seed`) — annars mäter du slumpen.
3. **Mät, lyssna inte bara:**

```powershell
# 90 Hz-bandet (basenergi)
ffmpeg -i fil.flac -af "bandpass=f=90:width_type=q:w=3,astats=metadata=1:reset=0" -f null -

# loudness + true peak
ffmpeg -i fil.flac -af ebur128=peak=true -f null -
```

4. **Lyssna blindt** på tre saker: sitter betoningen, hörs ändelserna, låter det svenskt.
5. **Skriv in resultatet i §14** — då växer mätbanken och nästa beslut blir billigare.

Det var så `Deep bass` åkte ut: fyra tagningar, samma kedja, 3 dB skillnad i 90 Hz-bandet.

---

## 21. Historik — beslut och datum

| Datum | Beslut |
|---|---|
| 2026-10-20 | `epadunk_v2` låst (147 BPM, sub-tung) och `mid_bass_party` (140 BPM, mid-tung) |
| 2026-10-20 | 90 Hz-höjningen sänkt **+4 → +1 dB** (råa tagningar låg 40 % högre i sub) |
| 2026-10-21 | 29 låtar × 2 stilar = 58 mästare klara; 5 texter medvetet överhoppade |
| 2026-10-21 | Svensktest godkänt — "fungerar jättebra" |
| 2026-10-21 | `sv_epadunk_v2` och `sv_mid_bass_party` sparade i `stilar.txt` (stil 4 och 5) |
| 2026-10-21 | Stil 6 `sv_raggardunk_power` och stil 7 `sv_epadunk_dark` låsta (från style-test 3e/4e) |
| 2026-10-21 | Stil 8 `sv_epadunk_v2b` — stil 4 + bastestets bas, fast röstprofil och inbyggt dropprecept |
| 2026-10-21 | `styles.md` skriven — den här filen |

---

## 22. Vilken stil ska jag välja?

| Mål | Stil | Varför |
|---|---|---|
| Epadunk/raggardunk, svensk | `sv_mid_bass_party` | mest igenkänd genre, 140 BPM |
| Hårdast möjliga klubbtryck | `sv_epadunk_v2` | 147 BPM, sub-heavy, fyra på golvet |
| Klubbtryck + garanterad drop | `sv_epadunk_v2b` | stil 4 + tydlig röst + tom break före sista refrängen |
| Partylåt med stor refräng | `mid_bass_party` | `party anthemic chorus` |
| Snabb, aggressiv, busig | `epadunk_v2` | `rowdy energetic`, högre tempo |
| Testa om en text funkar | `sv_mid_bass_party` | mildast smak, avslöjar uttalet tydligast |
| Ren instrumental | `instrumental` + genre | ingen sång, modellen komponerar fritt |

---

## Checklista före man trycker Create

- [ ] Språket först, tempot sist
- [ ] 12–50 ord
- [ ] En genre, inte fem
- [ ] Rösten beskriven med kön + klang + leverans
- [ ] 4–6 konkreta instrument
- [ ] Bara beskrivningar — inga instruktioner, artister eller titlar
- [ ] Inga siffror utom BPM
- [ ] Ingen negativ prompt (`no drums`) — beskriv det du vill höra i stället
- [ ] Basen beskriven med instrument + rörelse, inte med `deep`
- [ ] Längden styrd av antal sektioner, inte av hopp om `duration_seconds`
- [ ] Rätt mastringskedja vald (§15) — och `-ar 48000` vid export

---

## Se även

Filerna nedan hör till det lokala projektet och publiceras inte här — de står med som
referens till var recepten kommer ifrån.

| Fil | Innehåll |
|---|---|
| `stilar.txt` | snabbval: de fyra färdiga stilarna + mastringskommandon |
| `epadunk_v2.md`, `epadunk_v1.md` | låsta recept för epadunk |
| `mid_bass_party.md` | låst recept för mid_bass_party |
| `PROJEKT.md` | hela projektet: batch, motor, svenska, lärdomar |
