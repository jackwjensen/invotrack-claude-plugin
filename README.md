# InvoTrack til Claude Code

Mål din arbejdstid og dit AI-forbrug i Claude Code — og fakturér det fra
[InvoTrack](https://invotrack.dk).

## Sådan virker det

Første gang du arbejder i en mappe, spørger Claude, hvilken opgave arbejdet hører til, og noterer
svaret i mappens `CLAUDE.local.md` — kun på din computer. Næste gang registrerer Claude sessionen på
samme opgave uden at spørge. InvoTrack måler, hvor længe du selv arbejder, og hvor meget AI Claude
bruger, og Claude giver en kort beskrivelse af arbejdet. Med ét klik bliver det til
tidsregistreringer og AI-forbrug på opgaven, klar til faktura.

## Kun metadata forlader din computer

InvoTrack modtager tidspunkter, session, tokenantal og den korte beskrivelse af arbejdet. Aldrig det,
du skriver til Claude, Claudes svar, dine filer eller hvor de ligger.

## Installation

Log ind på InvoTrack, gå til **Mine AI-enheder → Tilføj enhed**, og følg vejledningen. AI-registrering
skal først slås til af en administrator i din organisation.

Udvidelsen opdaterer sig selv: vejledningen slår automatisk opdatering til for denne markedsplads
(`"autoUpdate": true` under `extraKnownMarketplaces` i `~/.claude/settings.json`).

## Udgiv en ny version

Claude Code henter kun en ny kopi, når versionen skifter. Hæv `version` i både
`plugins/invotrack/.claude-plugin/plugin.json` og `.claude-plugin/marketplace.json` ved hver ændring.

## Krav

- Claude Code og en InvoTrack-konto.
- På Windows: Git for Windows.

---

[invotrack.dk](https://invotrack.dk) ·
[Vejledning](https://invotrack.dk/dokumentation/ai-registrering) ·
Udviklet af [Allegro IT ApS](https://allegroit.dk) · kontakt@allegroit.dk
