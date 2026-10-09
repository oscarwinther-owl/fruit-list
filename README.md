

## 4. Sådan bruger du ChatGPT som vejleder

### Prøv selv først – AI er din hjælp, når du går i stå

Læs først STEP'et i `js/script.js`, undersøg eksemplet og hintsene, og **skriv og test selv koden**. Brug browserens **Console** og **Elements** til at undersøge, hvad din kode gør.

Du behøver **ikke** bruge generativ AI, hvis du selv kan løse opgaven. Hvis du sidder fast efter et reelt forsøg, kan ChatGPT hjælpe dig videre som **vejleder**.

| Du | ChatGPT som vejleder |
| --- | --- |
| Forsøger selv og tester din kode først | Hjælper kun, når du beder om det |
| Deler din egen kode, fejl og dit forsøg | Giver ét spørgsmål eller et lille hint ad gangen |
| Retter selv og tester igen | Venter på dit svar eller rettelsesforsøg |
| Arbejder videre i VS Code | Giver ikke en færdig løsning eller en fejlliste |

### 4.1 Start en ny chat, hvis du går i stå

Åbn ChatGPT, og start en **ny chat**. Brug denne startprompt som din første besked – **ordret**:

```text
Jeg er nybegynder i JavaScript. Vær min vejleder. Hjælp mig med én fejl ad gangen. Giv ét spørgsmål eller et lille hint, og vent på mit svar eller rettelsesforsøg. Giv ikke en fejlliste, rettede kodelinjer eller en færdig løsning. Forklar begreber, hvis jeg går i stå. Jeg skal selv finde og skrive rettelsen.
```

Indsæt derefter den relevante del af din `js/script.js` (eller upload filen) og forklar, **hvad du prøvede, hvad du forventede, og hvad der skete**. Du kan også dele `index.html`, hvis fejlen handler om HTML-elementerne.

### 4.2 Arbejdsgangen i hvert STEP

```text
1. Læs STEP'et og dets hints
↓
2. Planlæg løsningen selv
↓
3. Skriv kode i VS Code
↓
4. Test i browseren, Console og Elements
↓
5. Virker det? Gå videre til næste STEP
   Går du i stå? Brug AI som vejleder med din egen kode
↓
6. Svar på ét spørgsmål / afprøv ét hint
↓
7. Ret selv og test igen
```

### 4.3 Eksempler på spørgsmål, hvis du sidder fast

| ✅ Godt – viser dit forsøg | ❌ Undgå |
| --- | --- |
| "Her er min forEach. Den viser kun én frugt. Jeg tror, jeg har brugt = i stedet for +=." | "Skriv min forEach." |
| "Min if/else ændrer ikke knapteksten. Her er min kode og mit gæt på hvorfor." | "Lav min if/else." |
| "Jeg får en fejl i Console på linje 32. Jeg tror, jeg har stavet variabelnavnet forkert." | "Ret alle fejl i min kode." |

### 4.4 Når du får en fejl

1. Læs fejlbeskeden og find linjen i Console.
2. Undersøg din egen kode og formulér et gæt.
3. Hvis du stadig sidder fast, så del **koden, fejlbeskeden og dit gæt** med AI-vejlederen.
4. Svar på vejlederens spørgsmål, og skriv selv rettelsen.

### 4.5 Hvis ChatGPT alligevel skriver løsningen

**Kopiér ikke løsningen.** Skriv i stedet:

```text
Husk din rolle som vejleder. Giv ikke kode eller en fejlliste. Stil mig ét spørgsmål eller giv ét lille hint, og vent på mit forsøg.
```

Test altid AI's råd i browseren. AI kan tage fejl. **Målet er, at du selv forstår og kan skrive koden.**

---

## 5. Arbejd med opgaven

Åbn `js/script.js`, og følg kommentarerne fra **STEP 0** til **STEP 5**:

| STEP   | Indhold                                                         |
| ------ | --------------------------------------------------------------- |
| STEP 0 | Forbind `index.html` med `js/script.js` (`use strict` er udleveret)   |
| STEP 1 | Lav et array med objekter med frugternes data                    |
| STEP 2 | Hent listen, knappen og statusfeltet fra HTML'en                 |
| STEP 3 | Brug `forEach` til selv at opbygge frugtlisten                   |
| STEP 4 | Udfyld `if/else` i den udleverede funktion, der viser og skjuler listen          |
| STEP 5 | Tilføj et click-event til knappen                                |


Du skal kun skrive kode, hvor der står **✏️**. **Starterfilen har gyldig syntaks fra begyndelsen, så du kan teste efter hvert STEP.** Følg **de præcise variabelnavne** i `js/script.js`, så de forskellige STEPs hænger sammen. HTML-strukturen og CSS-stylingen er lavet for dig.

**Start med dit eget forsøg.** Eksemplet på en `forEach` i STEP 3 handler om bøger: Brug det til at forstå strukturen, men tilpas selv løkken til frugtlisten. I STEP 4 får du både funktionshovedet og `const isVisible = fruitListElement.classList.toggle("show");` udleveret, men du skal selv skrive `if/else`. **Timer-funktionen og `setTimeout()` er også udleveret** og fjerner automatisk statusbeskeden efter 2 sekunder. Den kode skal du ikke skrive eller ændre.

> **Tip:** Lav et **commit** efter hvert STEP, der virker. Så kan du altid gå tilbage til en version, der fungerede.

---

## 6. Commit og push dit arbejde

Når du har gemt dine filer i VS Code, skal du gemme dit arbejde i Git og sende det op til GitHub.com.

Åbn **GitHub Desktop**.

I venstre side kan du se de filer, du har ændret.

Skriv en kort beskrivelse i feltet **Summary**, fx:

```text
STEP 3: Build fruit list with forEach
```

Klik derefter på:

**Commit to main**

Klik til sidst på:

**Push origin**

Kontrollér på GitHub.com, at dine ændringer er kommet op i dit repository.

---

## 7. Sluttjek

Gennemgå listen, før du afleverer:

- [ ] Script-tagget med `defer` står i `<head>` i `index.html`
- [ ] `use strict` står i toppen af `js/script.js` (udleveret)
- [ ] `fruits` er et array med fem objekter
- [ ] `forEach` bygger ét listeelement for hver frugt med `innerHTML +=`
- [ ] Alle frugter vises med emoji, navn og farve
- [ ] Frugtlisten er skjult, når siden indlæses
- [ ] Knappen viser og skjuler frugtlisten
- [ ] Knappens tekst skifter mellem **Show fruit list** og **Close fruit list**
- [ ] Der er ingen røde fejl i Console
- [ ] Du har prøvet selv først og kun brugt AI som vejleder, hvis du gik i stå
- [ ] Du har brugt de præcise variabelnavne fra `js/script.js`
- [ ] Dit arbejde er committet og pushet til GitHub.com
- [ ] Den udleverede timer sørger for, at statusbeskeden forsvinder igen efter 2 sekunder

### Afsluttende refleksion

Forklar til sidst ChatGPT hele forløbet med dine egne ord:

```text
array → forEach → template literal → innerHTML → click → classList
```

Forklar sammenhængen selv. Hvis du går i stå, kan du bede AI-vejlederen stille dig ét spørgsmål, der hjælper dig videre.

> **Husk:** Prøv selv først. Hvis du sidder fast: Prompt dig klogere – ikke hurtigere.
