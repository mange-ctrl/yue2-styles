# STYLES — what you can write in YuE2's style field

*Reference for YuE2 Studio. Based on YuE2's own writing guide (`writing_guide`), our
tested styles and measurements on real songs. Updated 2026-10-21.*

---

## The short version

```
Language, genre, vocal, instruments, mood, production, N BPM
```

One field, English, comma-separated, **12–50 words**, the tempo **last**. No instructions,
no artists, no song titles, no lyrics.

---

## The rules (verbatim from the guide)

> *"the style prompt YuE2 reads verbatim under its [Tags] header … comma-separated
> descriptors, 12-50 words, in this order … the language the vocals are sung in first;
> genre and subgenre; the lead vocal (gender, timbre, delivery) or 'instrumental'; the key
> instruments and textures; the mood and melodic character; the tempo as '<n> BPM' last."*

> *"Be concrete and musical — instruments and textures, not adjectives about quality."*

> *"The request has no tempo, key, negative-prompt or instruction field, so everything
> about the sound lives in these descriptors: never write instructions to the model
> ('make it…', 'the song should…') or anything that is not a descriptor."*

> *"Never put lyric lines, a song title or section instructions in the style."*

Three things follow from that:

- **No negative prompt.** If you want to avoid something — describe what you want to hear
  instead. Not `no drums` but `a cappella` or `solo piano`.
- **Only BPM may be a number.** No `80 Hz`, no `4 bars`, no years that aren't a genre.
- **No artists.** Not `Fröken Snusk style` — describe the sound instead (that was exactly
  what went wrong in one of the songs; see "Words that don't work").

---

## 1. Language — always first

| Word | What it does |
|---|---|
| `English` | safest, the native language of the training |
| `Mandarin` / `Japanese` / `Korean` | officially supported |
| `Swedish` | **works well** (tested 2026-10-21), unofficial but useful |
| `instrumental` | no vocals at all — goes where the language would go |

Write the language as an **adjective at the start of the line**. Other languages with Latin
letters (Spanish, Italian, German) usually get through because the model sings the letters
it sees, but Swedish is the one we have verified.

---

## 2. Genre — not umbrella words

The guide: never a bare umbrella like `rock` or `pop` — be specific, ideally with era words.

| Term | Leans toward |
|---|---|
| `Epadunk` / `Raggardunk` | Swedish epa tractor, 4x4, rowdy vocals |
| `Eurodance` | 90s, supersaw, big chorus |
| `Nordic Russmusik` | Norwegian/Swedish graduation celebration, high energy |
| `Swedish pop` | clean, melodic, radio-friendly |
| `synthpop` / `dark synth-pop` | synth-driven, 80s, often cold |
| `pop-punk` / `early 2000s pop-punk` | fast, guitars, teenage |
| `melodic death metal` | growl, double kick, melody |
| `hip-hop` / `oldschool hiphop` | speech, breaks, sampling |
| `disco-funk` | 70s, lively bass, strings |
| `afrobeats` | polyrhythm, percussion, warm |
| `reggaeton` | dembow rhythm, Latin |
| `kpop` | polished, hooks, group vocals |
| `lofi` | muted, vinyl, soft |
| `country` | acoustic, steel guitar, storytelling |
| `indie rock` | guitars, live feel |
| `house` | 4x4, club, vocal sampling |
| `epic trailer` | orchestra, big drums |
| `qawwali` | South Asian devotional, harmonium |
| `chanson française` | French chanson, accordion |
| `canzone italiana` | Italian schlager, big voice |

---

## 3. Vocal — gender, register, timbre, delivery

**Gender / register**

`male vocal` · `female vocal` · `male and female duet` · `choir` · `gang vocals` ·
`child voice`

**Timbre**

`bright` · `warm` · `airy` · `nasal` · `husky` · `gritty` · `smooth` · `deep` ·
`high-pitched` · `raspy` · `bell-like` · `breathy`

**Delivery**

`clean` · `shouted` · `spoken` · `whispered` · `belted` · `crooned` · `rapid-fire` ·
`unhurried phrasing` · `legato` · `staccato`

**Examples of a whole vocal part**

```
gritty male tenor with shouted delivery
warm female pop vocal, unhurried phrasing
male and female duet, warm baritone and airy soprano
gang vocals with a bright female lead
```

The model has **no vocal tags in the lyrics** — everything about the voice belongs here.
Two singers are described here, never as `[Male singer]` in the lyrics.

---

## 4. Instruments

**Synths**

| Term | Sound |
|---|---|
| `supersaw synth lead` | the wide, saw-toothed lead of the 90s |
| `hoover synth` | rave hoover, aggressive |
| `FM bell synth` | glass bell, 80s |
| `arpeggiated synth` | pumping arpeggio |
| `pluck synth` | short, bouncy |
| `synth pad` | long, soft background |
| `square lead` | chip/retro |
| `wobble bass` | dubstep wobble |

**Bass**

| Term | Sound |
|---|---|
| `sub-heavy club mix` | a master with a lot below 120 Hz |
| `deep pumping offbeat bassline` | bass on the offbeat, pumping between the kicks |
| `808 sub bass with long sustain` | long, deep 808 |
| `sidechained sub bass` | bass that ducks under the kick |
| `arpeggiated synth bass` | rolling bass figure |
| `slap bass` | funky, percussive |
| `fingerstyle bass` | round, acoustic feel |
| `Reese bass` | wide, detuned, dnb/techno |

**Drums**

| Term | Sound |
|---|---|
| `four-on-the-floor kick drum` | kick on every beat |
| `4x4 kick` | the same thing, shorter |
| `punchy live drums` | real drums, hard |
| `gated snare` | 80s snare with a short tail |
| `LinnDrum` / `TR-909` | classic drum machines |
| `breakbeat` | a sample of a chopped-up beat |
| `hand percussion` | congas, shaker, tambourine |
| `stomping drums` | foot stomp, big |

**Guitar**

`distorted power chords` · `crunchy overdriven electric guitars` · `clean jangle guitar` ·
`acoustic guitar` · `slide guitar` · `palm-muted riffs` · `fingerpicked`

**Keyboards & folk**

`acoustic piano` · `Rhodes piano` · `church organ` · `accordion` · `harmonium` ·
`synthesizer strings` · `full string section` · `brass section` · `flute` · `banjo` ·
`sitar`

---

## 5. Production / mix

| Term | What it does |
|---|---|
| `sub-heavy club mix` | most energy below 120 Hz — **the only bass phrase that has proven itself** |
| `loud brickwall master` | hard-pressed, even, club-ready |
| `dry mix` / `little reverb` | dry, close |
| `reverb-drenched` | big, dreamy |
| `wide stereo` | wide, grand |
| `tape saturation` | warm, saturated |
| `lo-fi` | muted, noisy |
| `polished production` | clean, radio-grade |
| `cheap but powerful` | B-movie feel, fun |
| `sidechained` | ducks under the kick |
| `gated, punchy` | short and hard |

---

## 6. Mood — two to four simple words

`rowdy` · `energetic` · `playful` · `party anthemic` · `nostalgic` · `melancholic` ·
`restless` · `sarcastic` · `buoyant` · `dreamy` · `menacing` · `triumphant` ·
`intimate` · `sweaty` · `late-night`

Write **mood**, not ratings: `rowdy energetic` works, `awesome vibes` does nothing.

---

## 7. Tempo — always last, always `N BPM`

| Genre | Typical |
|---|---|
| ballad / folk song | 60–90 |
| hip-hop / trap | 70–100 (half-time) |
| pop | 100–125 |
| disco / funk | 110–125 |
| house | 120–128 |
| Eurodance | 130–145 |
| **epadunk / raggardunk** | **135–150** |
| russmusik | 140–160 |
| pop-punk | 160–185 |
| metal | 160–220 |

---

## 8. Words that **don't** work

| Don't write | Why | Write instead |
|---|---|---|
| `Deep bass` | a value word — says nothing about what actually sounds | `sub-heavy club mix` + `808 sub bass` |
| `phat`, `huge`, `massive` | the same thing | name the instrument |
| `make the bass deep` | an instruction, not a description | describe the sound |
| `Fröken Snusk style` | an artist name — the guide forbids it | `bright female vocal, Epadunk, 145 BPM` |
| `summer hit 2024` | song title/year | `Eurodance, party anthemic, 140 BPM` |
| `no drums`, `utan gitarr` | there is no negative prompt | describe what should be heard |
| `rock, pop, metal, jazz` | contradictory genres dilute | pick one, let the instruments do the rest |
| 20 instruments in a row | past 50 words the model loses focus | 4–6 instruments is enough |

**Measured proof:** a song with `Deep bass` in the style landed at −22,4 dB in the 90 Hz band.
Our locked styles that say `sub-heavy club mix` + `deep pumping offbeat bassline`
sit at −19 dB. Same software, same chain — only the words differ.

---

## 9. Our locked styles (they work, don't change them unnecessarily)

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

`{vocal}` is swapped per song: `bright female alto` · `deep male baritone` · `airy female soprano` ·
`gritty male tenor` · `warm female pop` · `male and female duet, warm baritone and airy soprano`.

---

## 10. Ready-made templates to paste in

**Epadunk, Swedish**
```
Swedish, Epadunk, Swedish Raggardunk, four-on-the-floor kick drum, deep pumping offbeat
bassline, sub-heavy club mix, bright female vocal, catchy pop hook, rowdy energetic, 145 BPM
```

**Eurodance anthem**
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

## 11. Troubleshooting

| Symptom | Likely cause | Action |
|---|---|---|
| The song came out the wrong genre | umbrella words or contradictory genres | one genre + concrete instruments |
| No low end | `deep bass`-type value words | `sub-heavy club mix`, `808 sub` |
| The voice sounds like the wrong gender | the voice described too vaguely | `female vocal` / `male vocal` first in the vocal part |
| Everything sounds the same | the same style every time | change 1–2 instruments + the voice, keep the rest |
| The model sings the words in the style | the style text accidentally ended up in the lyrics field | the style belongs in Style, only sung lines in Lyrics |
| The song came out too long/too short | `duration` is a ceiling, not a target | the number of sections controls the length |
| The Swedish sounds Norwegian | English loanwords in the lyrics | rewrite the line in plain Swedish |

---

## 12. What the style field does **not** control

Style describes the sound and the voice — nothing else.

| If you want to control | It belongs in |
|---|---|
| Verse / chorus / instrumental / outro | the lyric tags `[Verse 1]`, `[Chorus]`, `[Instrumental Break]` |
| Length | the number of sections (10 ≈ 2:45, 14 ≈ 4:10, 21 ≈ 5:20 at 140–147 BPM) |
| Exact melody, chords, time signature | the ABC notes (`cot: "full"` or your own score) |
| How random the harmony is | `harmony`: `strength`, `section_strength`, `outside_bonus` |
| Two singers taking turns | the voice in the style + verses in the lyrics — no vocal tags in the lyrics |
| Mix, mastering, loudness | the mastering chain afterwards (see §15) |
| Number of takes | `synth_batch_size`, `seed` |

Style therefore cannot make a song shorter, change the time signature or insert an
instrumental break — that is the tags and the notes.

---

## 13. Swedish → English glossary

Style is always written in English, even when the song is sung in Swedish.

| You are thinking | Write |
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

## 14. Measurement bank — what the styles actually deliver

Measured examples from real files (same engine, same mastering chain where nothing else is stated):

| File / style | Loudness | True peak | LRA | 90 Hz band |
|---|---|---|---|---|
| Source `supa som riktiga män` (raw) | −14,2 LUFS | +0,3 dBFS | 3,4 LU | — |
| `supa` — mastered, **bass chain** | −9,2 LUFS | +0,1 dBFS | 1,4 LU | −22,4 dB |
| `supa` — mastered, **mid_bass_party** (+1 dB @ 90 Hz) | −9,2 LUFS | +0,1 dBFS | 1,4 LU | −21,9 dB |
| `Nattkörning` — mastered epadunk_v2 | −9,5 LUFS | +0,1 dBFS | 2,1 LU | — |
| `Nattkörning` — mastered mid_bass_party | — | — | — | −19,0 dB |

Two things to draw conclusions from:

1. **Loudness always lands at −9,2 to −9,5 LUFS** regardless of style — it is the mastering
   that sets the level, not the style text.
2. **The 90 Hz band differs.** `Deep bass` in the style gave −22,4; `sub-heavy club mix` +
   `deep pumping offbeat bassline` gave −19,0 on a different song. The difference is the words.

### Bass test 2026-10-21 — five variants

Same lyrics (Köksfesten), same voice (`warm female pop`), same tempo, all mastered with the
bass chain so loudness is levelled. Only the bass phrase was swapped. Two takes per variant.
`diff` = the 90 Hz band minus the 1 kHz band — how much the bass stands out against the rest.

| Variant | Bass phrase in style | Length | 90 Hz | 1 kHz | diff |
|---|---|---|---|---|---|
| **A** | `heavy pumping bassline, 4x4 kick` | 2:47 | −19,9 | −20,5 | **+0,6** |
| **B1** | `deep pumping offbeat bassline, sub-heavy club mix` | 3:20 | −19,4 | −22,9 | **+3,5** |
| **B2** | same as B1 | 2:21 | −19,0 | −22,1 | **+3,1** |
| **C1** | `sidechained 808 sub bass under a four-on-the-floor kick` | 2:58 | −20,7 | −20,2 | **−0,5** |
| **C2** | same as C1 | 2:19 | −21,0 | −21,4 | **+0,4** |

**What the test shows:**

- **B wins clearly:** +2,7 dB more bass against the midrange than the base style (A), and
  +3,3 dB more than C. The difference is audible, it is not measurement noise.
- **C came out worse than no bass phrase at all.** `sidechained` means that the bass ducks
  under the kick — the words did exactly what they say, and lowered the low end.
- **The length did not affect the result:** B2 is the shortest of all (2:21) and has the
  second most bass.
- **Conclusion:** `deep pumping offbeat bassline` + `sub-heavy club mix` is the phrasing that
  gives the most low end in YuE2. It lives in `epadunk_v2` — and can be borrowed into other styles.

The masters from the test are in `bastest/` if you want to listen for yourself.



---

## 15. Mastering that belongs with the style

The styles have their own chains — they are part of the "style" and should not be mixed.

**Bass chain (epadunk_v1, epadunk_v2, sv_epadunk_v2)**

```
equalizer=f=200:t=q:w=1:g=-2.5,
equalizer=f=500:t=q:w=1:g=2,
equalizer=f=3500:t=q:w=1.2:g=-2,
equalizer=f=9000:t=h:w=1:g=-3,
acompressor=threshold=-20dB:ratio=3:attack=8:release=120:makeup=2,
loudnorm=I=-9.6:TP=-0.3:LRA=6,
alimiter=limit=0.97
```

**mid_bass_party / sv_mid_bass_party** = `equalizer=f=90:t=q:w=1:g=1,` + the bass chain.

History: the 90 Hz boost was **+4 dB** at first. Two new generations came in roughly 40 %
higher in sub-bass raw, so it was lowered to **+1 dB** on 2026-10-20. The boost is moreover
partly eaten by the compressor and limiter — +1 dB on the EQ gave **+0,5 dB** in the measurement.

Practical when exporting: `-ar 48000` (loudnorm works internally at 192 kHz and ffmpeg keeps
that rate otherwise), `-c:a flac -compression_level 8`, `-vn` if you want pure audio without a
cover image.

---

## 16. Length — number of sections, not `duration`

`duration_seconds` is a **ceiling**, not a target. The model stops when the lyrics run out.
Measured at 140–147 BPM:

| Sections | Usually becomes |
|---|---|
| 10 | 2:41–2:48 |
| 14 | about 4:10 |
| 21 | about 5:21 |

Rule of thumb: 10 sections ≈ 3 min, 14 ≈ 4 min, 18 ≈ 5 min, 24 ≈ 6 min.

**Padding rule when the song comes out too short:** if the last chorus has **≤ 6 lines**,
an `[Instrumental Break]` + a repeated `[Chorus]` is inserted before `[Outro]`. That typically
lifted 162 s → 228 s. If the last chorus is already written out/exploded (e.g. 16 lines) the
padding is skipped — otherwise it gets too long.

---

## 17. Voices — the rotation we have used

| Voice | Character | Suits |
|---|---|---|
| `bright female alto` | bright, clear, perky | epadunk, eurodance |
| `warm female pop` | soft, round, radio-friendly | pop, mid_bass_party |
| `airy female soprano` | airy, high | duets, ballad |
| `deep male baritone` | dark, heavy | raggardunk, seriousness |
| `gritty male tenor` | raspy, rowdy | epadunk, rock |
| `male and female duet, warm baritone and airy soprano` | two voices | chorus lift |

Rules we have landed on:

- **Change the voice between songs** — otherwise a 29-song batch melts together.
- **Same lyrics, different voice** in the two styles gives a clear A/B.
- **Perspective steers gender**: lyrics written from a female perspective (e.g. "hennes mun",
  "tungan") got a female voice in both versions, regardless of style.
- **Duet** was used on songs with two people in the story (e.g. `Nattkörning`,
  `Två blir tre`).
- The voice goes **only in the style** — never as `[Male singer]` in the lyrics.

---

## 18. Adapters / LoRA — controlled outside the style

A LoRA is a separate layer, not part of the style text:

```
adapters: [{ id: "yue2-sv-billie", scales: { ar: 1, nar: 1 } }]
```

| Thing | What it does |
|---|---|
| `scales` | strength per slot, 0–1. Omitted = the LoRA's own |
| `ar` slot | affects composition/melody |
| `nar` slot | affects sound/vocal timbre |
| `companion_scale` | the realaudio decoder, 0 = pure YuE2 checkpoint |

Installed in the studio: `yue2-sv-billie` (trigger `sv_billie`), a bunch of **slider LoRAs**
(`yue2-slider-female`, `-male`, `-pop`, `-rock` … rank 8, easy to sneak in) plus
genre LoRAs (bulgarian-voices, canzone-italiana, dark-sufi, qawwali, militant-reggae …).

Two things we **don't** know yet, and that should be tested:

- whether the trigger word `sv_billie` should be in the **style** or in the **lyrics** to fire;
- whether `yue2-sv-billie` makes the Swedish better or just changes the timbre.

Until that has been tested: treat LoRA as a spice, not a prerequisite — the Swedish
already works without it.

**Tested 2026-10-21:** `yue2-sv-billie` sings **mumbly** — the words lose
clarity. Don't use it for lyrics where pronunciation matters. (No measurement done, only
listening — but that is enough to deprioritise it.)

---

## 19. When the songs sound the same

The order in which to attack it, from biggest effect to smallest:

1. **Change 1–2 instruments in the style** — keep genre and tempo, swap e.g. `supersaw` for
   `FM bell synth`, or `four-on-the-floor` for `breakbeat`.
2. **Change the voice** (see §17) — the cheapest variation that is heard immediately.
3. **Vary `seed` / `lm_seed`** — the same seed gives the same composition.
4. **Touch the harmony:** `harmony.strength` 6–10 breaks a looping chord progression,
   `section_strength` gives each section its own opening, `outside_bonus` brings in chords
   outside the key.
5. **`cot`:** `"full"` lets the model write melody + chords (more variation between songs),
   `"off"` skips the note planning.
6. **The tempo 3–5 BPM** up or down changes the feel without changing the genre.

---

## 20. How to test a style change so that the answer means something

A single song says nothing — the model varies. Do this:

1. **Everything the same except one thing.** Same lyrics, same voice, same length, same `steps`.
   Change only the phrase you want to measure.
2. **Two takes per variant** (different `seed`) — otherwise you are measuring chance.
3. **Measure, don't just listen:**

```powershell
# 90 Hz band (bass energy)
ffmpeg -i fil.flac -af "bandpass=f=90:width_type=q:w=3,astats=metadata=1:reset=0" -f null -

# loudness + true peak
ffmpeg -i fil.flac -af ebur128=peak=true -f null -
```

4. **Listen blind** to three things: does the stress land, are the word endings audible, does it sound Swedish.
5. **Write the result into §14** — then the measurement bank grows and the next decision gets cheaper.

That is how `Deep bass` got kicked out: four takes, the same chain, 3 dB difference in the 90 Hz band.

---

## 21. History — decisions and dates

| Date | Decision |
|---|---|
| 2026-10-20 | `epadunk_v2` locked (147 BPM, sub-heavy) and `mid_bass_party` (140 BPM, mid-heavy) |
| 2026-10-20 | the 90 Hz boost lowered **+4 → +1 dB** (raw takes came in 40 % higher in sub) |
| 2026-10-21 | 29 songs × 2 styles = 58 masters done; 5 lyrics deliberately skipped |
| 2026-10-21 | Swedish test approved — "works really well" |
| 2026-10-21 | `sv_epadunk_v2` and `sv_mid_bass_party` saved in `stilar.txt` (style 4 and 5) |
| 2026-10-21 | Style 6 `sv_raggardunk_power` and style 7 `sv_epadunk_dark` locked (from style test 3e/4e) |
| 2026-10-21 | Style 8 `sv_epadunk_v2b` — style 4 + the bass from the bass test, fixed vocal profile and built-in drop recipe |
| 2026-10-21 | `styles.md` written — this file |

---

## 22. Which style should I choose?

| Goal | Style | Why |
|---|---|---|
| Epadunk/raggardunk, Swedish | `sv_mid_bass_party` | the most recognisable genre, 140 BPM |
| The hardest possible club pressure | `sv_epadunk_v2` | 147 BPM, sub-heavy, four on the floor |
| Club pressure + a guaranteed drop | `sv_epadunk_v2b` | style 4 + a clear voice + an empty break before the last chorus |
| Party song with a big chorus | `mid_bass_party` | `party anthemic chorus` |
| Fast, aggressive, rowdy | `epadunk_v2` | `rowdy energetic`, higher tempo |
| Test whether a lyric works | `sv_mid_bass_party` | the mildest flavour, reveals the pronunciation most clearly |
| Pure instrumental | `instrumental` + genre | no vocals, the model composes freely |

---

## Checklist before you press Create

- [ ] Language first, tempo last
- [ ] 12–50 words
- [ ] One genre, not five
- [ ] The voice described with gender + timbre + delivery
- [ ] 4–6 concrete instruments
- [ ] Only descriptions — no instructions, artists or titles
- [ ] No numbers except BPM
- [ ] No negative prompt (`no drums`) — describe what you want to hear instead
- [ ] The bass described with instrument + movement, not with `deep`
- [ ] The length controlled by the number of sections, not by hoping for `duration_seconds`
- [ ] The right mastering chain chosen (§15) — and `-ar 48000` on export

---

## See also

The files below belong to the local project and are not published here — they are listed as a
reference to where the recipes come from.

| File | Contents |
|---|---|
| `stilar.txt` | quick pick: the four finished styles + mastering commands |
| `epadunk_v2.md`, `epadunk_v1.md` | locked recipes for epadunk |
| `mid_bass_party.md` | locked recipe for mid_bass_party |
| `PROJEKT.md` | the whole project: batches, engine, Swedish, lessons learned |
