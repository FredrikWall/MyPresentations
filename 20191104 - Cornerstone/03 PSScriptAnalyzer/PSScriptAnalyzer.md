# 03 PSScriptAnalyzer

## Vad är PSScriptAnalyzer?

- PSScriptAnalyzer är kod kontroll
- För PowerShell moduler och skript
- PSScriptAnalyzer kontrollerar kvalitén genom regler
- Reglerna baseras på PowerShell best practices
- Från PowerShell teamet och från PowerShell communityn
- Går att lägga till eller exkludera regler

## Installera och använda

Behövs inte installeras manuellt om man Installerat Visual Studio Code + PowerShell Extension

Annars finns den på PowerShell Gallery

Install-Module PSScriptAnalyzer
Import-Module PSScriptAnalyzer

Och för att lista kommandona:

Get-Command -Module PSScriptAnalyzer

Om vi sedan kör Invoke-ScriptAnalyzer .\mittskript.ps1  
så kommer vi få hjälp med vad vi kan förbättra i skriptet.

## Visual Studio Code och PSScriptAnalyzer

Om vi använder Visual Studio Code och PowerShell extensionen så har vi PSScriptAnalyzer installerat.

Dock är det endast några regler som är aktiverade som standard.

Tryck på Shift + Ctrl + P och skriv PSScriptAnalyzer.  
Välj "Select PSScriptAnalyzer Rules"

Här kan du sedan välja vilka regler du ska använda.
Klicka på Confirm innan du stänger ner rutan, annars sparas det inte.

Nu när du skriver PowerShell kod i Visual Studio Code så kommer du få hjälp där det behövs.

T ex så får man hjälp med att undvika Alias, man får även hjälp om man skapar en variabel men inte använder den i skriptet.

Texten får en orange vågigunderlinje och drar man musen över så får man hjälp med vad som är fel och i många fall får man även frågan om man vill ha hjälp att ändra.
