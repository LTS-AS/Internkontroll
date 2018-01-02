# Rutiner for økonomistyring

## Plassering av journalvedlegg
### Journalregistreringer
- 5 DIV Diverse journal
- 6 OPEJ Opening Entries Journal
- 7 BNK1 Kontant
- 8 BNK2 Bank
### Leverandører
- 2 EXJ Innkjøpsjournal
- 4 ECNJ Leverandør kreditnota-journal
### Trenger ikke vedlegg
- 1 SAJ Salgsjournal
- 3 SCNJ Refusjonsjournal
- 9 STJ Varelager-journal

## Registrere regninger (ved mottak)
- Klikk "Opprett" i leverandørfakturaer. (hvis ikke faktura eksisterer)
- Velg kunde, legg inn fakturanummer, legg til fakturalinje(r), velg fakturadato, oppdater MVA, sjekkk totalbeløp, klikk "Valider"
- Legg ved faktura, slett faktura lokalt

## Betale regninger ()
- Gå til leverandørfaktura, finn fakturaer med status "Åpne"
- Betal åpne fakturaer i nettbank, last ned kvitteringer
- Klikk "Betalt", betalingsmetode, dato, registrer betaling
- Gå til journalregistreringer, postèr, legg inn vedlegg, slett vedlegg fra pc

## Registrere innbetalinger
- Finn relevant faktura, velg registrer betaling, Sjekk beløp, velg betalingsmetode, velg dato, registrer betaling, gjenta for alle
- Gå til journalregistreringer, postèr, legg inn vedlegg, slett vedlegg fra pc, gjenta for alle

## Registrere kvitteringer (DIV)
- Gå til journalregistreringer, finn en eksisterende journal med samme skattebase, ta en kopi
- Juster periode, referanse, dato, partner, konto, beløp, skattebeløp
- Lagre, postèr, legg til vedlegg, slett vedlegg fra PC

## Lønn (siste dag i måned)
- Fyll ut excel-mal for lønnsrapport. En fil per ansatt. Legg ferdige filer i L:\accounting\Lønn.
- Kopier en eksisterende lønnsjournal, DIV/xxxx/xxxx
- Skriv filnavn i referansefeltet, oppdater periode, oppdater dato, sjekk partner på alle linjer
- kjør write_payment.py for å lese inn journallinjer
- Kjør utbetalinger

## Statusovervåking (nattjobb)
- Inkommende fakturaer skal vedlegges (EXJ)
- Inkommende kreditnotaer skal vedkegges (ECNJ)
- Diversejournaler skal ha vedlegg (DIV)
- Kontantjournaler skal ha vedlegg (BNK1)
- Bankjournaler skal ha vedlegg (BNK2)
- Ingående fakturaer nær forfall
- Utgående fakturaer som har forfalt

## Ønskeliste statusovervåking
- Innlesing av lønnsrapport
- Oppdatering av referanser på lts.no
- Levering av a-melding

## MVA (Slutten av måned {1,3,5,7,9,11})
- Skriv ut kontoutskrifter
- Rapportering, Avgiftsrapport, Regnskapsrapporter, Hovedbok
- Stem av rapport og kontoutskrift

- Rapportering, Generiske rapporter, Avgifter, Avgiftsrapport
- Lag en ny DIV-journal med referansen MVA<nummer>

## For årsrapport
- Rapportering, Avgiftsrapport, Regnskapsrapporter, Balanse
