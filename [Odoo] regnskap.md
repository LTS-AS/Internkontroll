# Rutiner for økonomistyring

## Lønn (siste dag i måned)
### Input

### Logikk

### Output

## MVA (Slutten av måned {1,3,5,7,9,11})
### Input

### Logikk

### Output

## Registrere regninger (ved mottak)
- Klikk "Opprett" i leverandørfakturaer. (hvis ikke faktura eksisterer)
- Velg kunde, legg inn fakturanummer som fri referanse, legg til fakturalinje(r), velg fakturadato, oppdater MVA, sjekkk totalbeløp, klikk "Valider"
- Legg ved faktura, slett faktura lokalt

## Betale regninger ()
- Gå til leverandørfaktura, finn fakturaer med status "Åpne"
- Betal åpne fakturaer i nettbank, last ned kvitteringer
- klikk "Betalt", betalingsmetode, dato, registrer betaling, legg inn kvittering

## Statusovervåking (nattjobb)
- Inkommende fakturaer skal vedlegges (EXJ)
- Inkommende kreditnotaer skal vedkegges (ECNJ)
- Diversejournaler skal ha vedlegg (DIV)
- Kontantjournaler skal ha vedlegg (BNK1)
- Bankjournaler skal ha vedlegg (BNK2)

## Ønskeliste statusovervåking
- Innlesing av lønnsrapport
- Levering av a-melding
- Ingående fakturaer nær forfall
- Utgående fakturaer forfalt
