# Oppsett: Obsidian + Claude Cowork

> Detaljert oppsett, steg for steg. Mål: ca. 5 til 10 minutter. Ingen terminal, ingen git. Hvis noe er uklart, flagg ned en på gulvet.

Når du er ferdig her har du:

1. Startpakken lastet ned og pakket ut.
2. `starter-vault`-mappen åpnet som vault i Obsidian.
3. Et Cowork-prosjekt med tilgang til den samme mappen.
4. De viktigste ferdighetene ("skills") lastet opp i Cowork.
5. Ett ekte notat skrevet, med riktig metadata.

---

## Steg 1: Last ned og pakk ut startpakken

1. På forsiden av dette repoet (GitHub): trykk den grønne **Code**-knappen, så **Download ZIP**.
2. Finn zip-filen (vanligvis i Nedlastinger) og pakk den ut. På Mac: dobbeltklikk. På Windows: høyreklikk, **Pakk ut alle**.
3. Flytt gjerne den utpakkede mappen et sted du finner igjen, for eksempel **Dokumenter**.

Inne i mappen ligger `starter-vault/`. **Det er den mappen som er din kunnskapsbase.** Resten er veiledning.

---

## Steg 2: Åpne vault-en i Obsidian

1. Start Obsidian.
2. Velg **Open folder as vault** (eller **Open another vault ▸ Open folder as vault**).
3. Pek på `starter-vault`-mappen og åpne den.
4. Stol på vault-en hvis Obsidian spør.

Nå ser du mappene i venstremenyen: `Learning`, `Meetings`, `Notes`, `Personal`, `Projects`, `Reference`, `Templates`, `Attachments`.

Tips: skru på **Settings ▸ Files and links ▸ Detect all file extensions** så alle filene vises.

---

## Steg 3: Lag et Cowork-prosjekt på samme mappe

1. Åpne **Claude** desktop-appen og gå til **Cowork**.
2. Lag et nytt **prosjekt** (gi det et navn, for eksempel "Second brain").
3. Gi prosjektet tilgang til den **samme** `starter-vault`-mappen som du åpnet i Obsidian.
4. (Anbefalt) I prosjektets **Instructions**, lim inn én linje: *"Følg konvensjonene i `CLAUDE.md` i denne mappen. Bekreft alltid før du skriver til disk."*

Nå deler du og agenten den samme mappen: du ser endringene i Obsidian, agenten skriver rett inn i den.

---

## Steg 4: Last opp ferdighetene ("skills")

Dette er den ene tingen som er annerledes i Cowork enn i Claude Code: **Cowork plukker ikke opp ferdigheter automatisk fra mappen.** Du legger dem inn én gang:

1. I Cowork: gå til **Customize ▸ Skills**.
2. Trykk **+**, velg **last opp en skill (ZIP)**.
3. Last opp filene fra `skills-to-upload/` i startpakken:
   - `obsidian-vault.zip` (konvensjonene, anbefalt)
   - `capture-to-note.zip` (brukes i øvelse 1)
   - `skill-creator.zip` og `brainstorming.zip` (valgfritt, til øvelse 2)
4. Skru hver av dem **på**.

Skills er knyttet til kontoen din, så dette gjør du bare denne ene gangen, ikke per prosjekt.

---

## Steg 5: Si fra til agenten

I Cowork-prosjektet, skriv for eksempel:

> *"Les `CLAUDE.md` i denne mappa, og hjelp meg lage mitt første notat."*

Agenten leser konvensjonene (`CLAUDE.md` ligger i vault-mappa) og bruker `obsidian-vault`-skillen, og guider deg videre. Be den gjerne først bekrefte at den forstår mappestrukturen og metadata-reglene.

---

## Steg 6: Skriv det første ekte notatet

Velg noe lite du faktisk vil huske (en bok, et møte, noe du lærte denne uka). Be agenten lage notatet. Sjekk at det:

- havner i riktig mappe ut fra type,
- bruker malen fra `Templates/`,
- har frontmatter med dagens dato (`DD.MM.YYYY`),
- kun har `[[lenker]]` der koblingen er ekte (null lenker er helt greit i starten).

Åpne så notatet i Obsidian. Frontmatter vises som et **Properties**-panel øverst, og i **Graph View** (`Cmd/Ctrl+G`) dukker notatet opp som en prikk. Den er ensom nå. Det endrer seg i øvelse 1.

---

## Steg 7: Videre til øvelsene

Gå til [`06-challenges.md`](06-challenges.md).

---

## Hvis noe butter

| Problem | Hva du gjør |
|---------|-------------|
| Agenten finner ikke filene | Sjekk at Cowork-prosjektet har tilgang til `starter-vault`-mappen. |
| Agenten kan ikke reglene | Be den lese `CLAUDE.md` på nytt, eller lim inn innholdet i chatten. |
| Lenker vises som vanlig tekst | Sjekk **Settings ▸ Files and links ▸ Use [[Wikilinks]]** i Obsidian. |
| Obsidian åpnet feil mappe | **File ▸ Open another vault** og velg `starter-vault` på nytt. |
| En skill skrur seg ikke på | Sjekk at du lastet opp riktig ZIP under **Customize ▸ Skills** og at den er toggled på. |
