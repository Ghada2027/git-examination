
# Git-examination

## Fråga 1: Versionshantering vs vanliga filer

Versionshantering betyder att man sparar olika versioner av ett projekt och kan se vad som har ändrats över tid. När jag sparar med editorns vanliga sparaknapp ändras filen på datorn, men när jag gör en **commit** sparar Git en version som jag kan gå tillbaka till senare.

Git sparar en tidslinje av **frysta ögonblicksbilder (commits)**. Att min första commit fortfarande innehåller alla tre **TODO** visar att Git behåller den gamla versionen även när jag har ändrat filen senare.

## Fråga 2: Arbetsytan, Staging och Commits

De tre kommandona används så här:

- **git status** visar vilka filer som har ändrats.
- **git add** lägger ändringarna i staging.
- **git commit** sparar ändringarna som en ny version i Git.

Jag tänker på arbetsflödet som tre steg:

1. **Arbetsytan:** Ett ark på skrivbordet där jag arbetar med filen.
2. **Staging:** Ett kuvert där jag lägger de ändringar jag vill spara.
3. **Commit:** En arkivlåda där Git sparar versionen.

Om jag ändrar en fil men inte kör **git add** finns ändringen bara i arbetsytan och är inte redo att committas. Därför kan Git visa **no changes added to commit**, eftersom inga ändringar har lagts i staging.

## Fråga 3: Lådan hemma vs Montern på GitHub

Mappen på datorn innehåller mitt **lokala projekt**, medan GitHub-repot innehåller projektets version online. Kommandot **git push** skickar mina lokala commits till GitHub.

Jag tänker på datorn som en låda hemma och GitHub som en glasmonter online. Det är två olika platser som behöver uppdateras. Om jag ändrar en fil men glömmer att köra **git add** och **git commit** finns ingen ny commit att skicka. Därför kan **git push** svara **Everything up-to-date**, eftersom det inte finns några nya commits att ladda upp.
