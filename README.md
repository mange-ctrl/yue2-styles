# YuE2 styles

En praktisk referens för **style-fältet i YuE2 Studio** — vad man skriver, i vilken ordning, vilka ord som faktiskt gör något och vilka som bara låter bra i huvudet.

Bygger på YuE2:s egen skrivguide (`writing_guide`), egna A/B-tester och mätningar på riktiga filer (loudness, true peak, 90 Hz-band).

## Innehåll

| Fil | Vad den är |
|---|---|
| [`styles.md`](styles.md) | Hela guiden på svenska: regler, ordlistor, låsta stilar, mätbank, mastringskedjor, felsökning |
| [`styles.en.md`](styles.en.md) | Samma guide på engelska |

## Kort version

```
Språk, genre, sångröst, instrument, känsla, produktion, N BPM
```

Ett fält, engelska, kommaseparerat, 12–50 ord, tempot sist. Bara beskrivningar — inga instruktioner, artistnamn eller låttitlar. Ingen negativ prompt finns, så beskriv ljudet du vill höra i stället för att förbjuda det du inte vill ha.

## Låsta stilar

| Stil | Tempo | Karaktär |
|---|---|---|
| `epadunk_v2` | 147 BPM | English, sub-tung epadunk/eurodance |
| `sv_epadunk_v2` | 147 BPM | samma på svenska |
| `mid_bass_party` | 140 BPM | English, mid-tung raggardunk/party |
| `sv_mid_bass_party` | 140 BPM | samma på svenska |
| `sv_epadunk_v2b` | 142 BPM | sv_epadunk_v2 + fast röst och inbyggt dropprecept |

## Vad som är mätt, inte tyckt

- `deep pumping offbeat bassline` + `sub-heavy club mix` gav **+3,5 dB** mer bas mot mellanregistret än ingen basfras alls. `sidechained`-formuleringen gav **mindre** bas än ingen basfras — orden gör precis vad de säger.
- Loudness landar på **−9,2 till −9,5 LUFS** oavsett style-text: nivån sätts av mastringen, inte av orden.
- Längden styrs av **antal sektioner**, inte av `duration_seconds` (som är ett tak).

Detaljer, tabeller och mastringskedjor finns i [`styles.md`](styles.md) (svenska) och [`styles.en.md`](styles.en.md) (English).

## Licens

Texten är licensierad under [CC BY 4.0](LICENSE) — använd, ändra och dela fritt, även kommersiellt, så länge du anger källa och länk till licensen. Se [`LICENSE`](LICENSE).

