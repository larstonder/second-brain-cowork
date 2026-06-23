# Øvelser

> To øvelser. Øvelse 1 er **Fang**. Øvelse 2 er **Tilpass**. Begge er åpne i begge ender, det er meningen. Står du fast, flagg ned en på gulvet.

---

## Øvelse 1: Fang en YouTube-video inn i kunnskapsbasen

**Leveranse:** ett nytt notat i `Learning/` med frontmatter, ekte innhold (sammendrag + nøkkelpunkter + et "Slik bruker jeg dette"-avsnitt), og minst én ekte `[[lenke]]` til noe beslektet. Kvaliteten på lenken betyr mer enn antallet.

### Slik gjør du det (uten terminal)

Cowork kan ikke laste ned video selv slik en koder ville gjort. Den enkle veien for ikke-kodere er å lime inn teksten:

1. **Velg en video.** 5 til 20 minutter, noe du faktisk vil huske. Trenger du en demo-video å følge med på: spør crewet om dagens forslag.
2. **Hent transkripsjonen fra YouTube.** Under videoen: trykk **... (mer) ▸ Vis transkripsjon** (eng: *Show transcript*). Marker teksten og kopier den. (Vil du slippe tidsstemplene: skru dem av i transkripsjons-panelet først.)
3. **Lim den inn i Cowork** sammen med lenken til videoen, og be om en personlig uthenting. For eksempel:
   > *"Her er transkripsjonen av denne videoen [lim inn lenke]. Trekk ut det viktigste for meg som [din rolle] som akkurat nå er opptatt av [ditt fokus], og lag et Learning-notat."*

   Personaliseringen er poenget: den gjør et generisk sammendrag til noe du faktisk leser igjen.
4. **La agenten skrive notatet** i `Learning/` med malen `Templates/Learning.md`. Sjekk at det har:
   - riktig frontmatter (`type: learning`, dagens dato, `source:` med lenken, `author:` med kanalnavn, `status: draft`),
   - minst én ekte `[[lenke]]`, og ikke flere enn det som faktisk henger sammen,
   - et "Slik bruker jeg dette"-avsnitt som er konkret, ikke generisk.
5. **Har du et eldre notat som faktisk hører sammen**, legg til en lenke begge veier. Er vault-en tom eller ingenting hører ekte sammen, hopp over. En påtvunget lenke er bare støy.

> Bruker du `youtube-to-note`-ferdigheten du lastet opp i oppsettet, gjenkjenner den at du limer inn en transkripsjon og følger samme flyt automatisk.

### Level-up (valgfritt): la agenten hente transkripsjonen selv via MCP

Vil du slippe paste-runden, kan du gi Cowork en **connector** som henter YouTube-transkripsjoner for deg. Da limer du bare inn lenken til videoen, så gjør agenten resten.

1. I Cowork: **Customize ▸ Connectors ▸ +**.
2. Lim inn navn og URL til en hosted YouTube-transkripsjon-MCP (crewet deler en testet URL på workshopen).
3. Lagre, og koble til.

Dette er en fin måte å se hva en "connector" (MCP) faktisk er: agenten får en ny evne uten at du installerer noe. Men paste-flyten over funker alltid, så bruk den hvis connectoren kludrer.

### Sånn ser "ferdig" ut

Åpne **Graph View** i Obsidian. Det nye `learning`-notatet skal henge sammen med minst ett annet notat. Det er din første ekte nervebane.

---

## Øvelse 2: Lag din egen tilpasning

**Leveranse:** én tilpasning du faktisk vil bruke, som former hvordan agenten jobber for deg. To gode former, velg én (eller begge om du har tid):

### Form A: en "skill" du lager og laster opp

En skill er en liten instruks Cowork laster inn når den passer. Be agenten hjelpe deg:

> *"Bruk `skill-creator` til å hjelpe meg lage en liten skill. Bruk `brainstorming` hvis vi trenger å tenke gjennom hva den skal gjøre."*

Eksempel som funker godt for ikke-kodere: **`devils-advocate`**, en skeptisk tenkepartner.
- Trigger: "spill djevelens advokat", "finn hullene i dette", "hva er galt med denne planen".
- Oppførsel: bytt fra hjelpsom assistent til streng, men konstruktiv skeptiker. List de sterkeste motargumentene, de skjulte antakelsene, og det du ikke vet. Avslutt med ett ærlig råd: "Hadde jeg vært deg, ville jeg stresstestet X først."

Når den er laget: pakk skill-mappen som en ZIP, last den opp under **Customize ▸ Skills**, skru den på, og test at den trigger på en naturlig setning.

### Form B: en lagret instruks (enklest)

Vil du slippe ZIP-runden: legg tilpasningen som en **instruks på Cowork-prosjektet** i stedet (**Instructions**). Samme effekt, formet til denne kunnskapsbasen. For eksempel en fast måte å oppsummere møtenotater på, eller en personlig tone.

### Sånn ser "ferdig" ut

Du har én tilpasning som trigger på en naturlig setning og gjør noe du faktisk vil ha. Du har kjørt den minst én gang.

---

## Del med de andre (siste delen av workshopen)

Noen frivillige viser:

- hva de fanget i øvelse 1 (skjermbilde av grafen),
- hvilken tilpasning de lagde i øvelse 2, og en live-kjøring.

Hold det kort, under 3 minutter hver. Så peker vi alle mot [`07-going-further.md`](07-going-further.md) for å holde vanen i gang.
