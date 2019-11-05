# 01 Visual Studio Code

## Vad är Visual Studio Code?

- Ersättare för PowerShell ISE

    PowerShell ISE har slutat att utvecklas och Microsoft vill istället att vi använder Visual Studio Code för att editera och köra PowerShell script.

- Source code editor

    Editor för att editera kod av olika slag

- Gratis
 
    Precis som PowerShell ISE är Visual Studio Code gratis.

- Windows, macOS och Linux

    Finns för Windows, macOS och Linux.
    Men behöver laddas ner och installeras.

- InteliSense

    Code completion, parameter information, snabb information och member lists

- Debugging

- Built-in Git

    Inbyggt stöd för Git
    Men man behöver installera Git för att det ska fungera.

- Extensions

    Många tillägg för att få stöd för olika skriptspråk, teman m.m m.m

- Inställningar för att få saker som man vill

    Vi kan styra mycket via settings

## Hämta och Installera

Visual Studio Code finns att ladda ner på
https://code.visualstudio.com

Finns för Windows, macOS och Linux.
För windows i både 32 och 64 bitars varianter.

Dessutom har vi en Stable och en Insiders version av alla varianter.

Stable uppdateras 1 gång / månad

Insiders uppdateras 1 gång / dag

Installera standard men välj högerklick för att öppna filer med Visual Studio Code.

Visual Studio Code går att starta på olika sätt.

- Genvägar
- Högerklicka på filen du vill öppna med Visual Studio Code och välj "Open with code".
- I en PowerShell konsol kan man skriva "Code" för att starta Visual Studio Code eller "Code .\filen.ps1" för att starta Visual Studio Code med filen.ps1 laddad.

## Teman

Vi kan styra utseendet på Visual Studio Code med teman.

- PowerShell ISE tema
    Följer med PowerShell extensionen

- Färgteman

    Ctrl + K Ctrl + T
    Eller File -> Preferences -> Color Theme

    Vill man ha fler så klickar man på Install Additional Color Themes...

    Då öppnas Extensions: Marketplace med teman.

    Här finns det många att välja på.

    Räcker inte dessa så går det att skapa egna.

## Extensions

- Mer funktionalitet

    Med extensions får vi utökad funktionalitet.

- Fler format

    Stöd för fler filformat/skriptspråk

- Hjälp med att formatera

    Med extension för olika filformat så får vi funktionaliteten att formatera vår kod genom att högerklicka och välja "Format Document"

- PowerShell

    För att få stöd för PowerShell i Visual Studio Code behöver vi installera PowerShell eller PowerShell preview extension.

    Klicka på extensions ikonen till vänster.
    Eller File -> Preferences -> Extensions

    Skriv in PowerShell i sökrutan.

    Och klicka på install.

    När vi gjort det får vi hjälp med:

    - Syntax highlighting
    - Code snippets
    - IntelliSense for cmdlets and more
    - Rule-based analysis provided by PowerShell Script Analyzer
    - Go to Definition of cmdlets and variables
    - Find References of cmdlets and variables
    - Document and workspace symbol discovery
    - Run selected selection of PowerShell code using F8
    - Launch online help for the symbol under the cursor using Ctrl+F1
    - Local script debugging and basic interactive console support!

- Settings Sync

    Användbar extension för att synka sina Visual Studio Code settings mellan datorer via GitHub.

- XML tools

    Ger oss bland annat möjligheten att formatera XML filer genom högerklick och Format Document.

- GitLens - Git supercharged

    Jobbar man med Git så är denna extension bra då man får extra information.

- markdownlint

    Hjälper till med editering av markdown

## PowerShell
    
När vi har installerat PowerShell extensionen har vi stöd för PowerShell om vi öppnar ps1 filer.

Dock får vi inte PowerShell stödet laddat för nya filer automatiskt.

Om vi väljer "New File" så får vi en untitle text file som standard.

Om vi då försöker att skriva t ex Get- så händer ingenting.

Vi får då gå ner till höger där det står text file.
Klicka på den och skriva PowerShell.

Om vi nu skriver Get- så får vi upp förslag på cmdlets.
Om vi vill ha mer information, om syntax så får vi tryck på Ctrl + mellanslag. Samma för att få bort extra informationen.

Om vi nu kommer att använda Visual Studio Code till att skapa PowerShell skript
i de flesta fall så kan vi välja PowerShell som Defaul Language. Så att vi slipper välja det för varje "New File".

Tryck på Shift + Ctrl + P för "Command Palette" eller klicka på kugghjulet nere till vänster (Manage)och välj Command Palette.

Skriv User i sökrutan. Välj Preferences: Open User Settings.

Skriv "Default language" i sökrutan.

Leta upp Files: Default Language.
Skriv "powershell" i rutan.
Fungerar inte med "PowerShell".

Om man stänger ner Visual Studio Code nu eller
startar om sessionen genom att trycka Shift + Ctrl + P,
skriver restart och väljer "PowerShell: Restart Current Session" så ska PowerShell vara standard vi nya filer.

## Snippets

Med PowerShell extensionen får vi många färdiga snippets eller kodsnuttar på Svenska.

Om vi t ex börjar skriva comm så kommer Visual Studio Code med förslag och de rader som börjar med en fyrkant är snippets.

Väljer vi comment-help så kommer vi få färdig kodsnutt för kommentarsbaserad hjälp.

Om vi istället skulle trycka Shift + Ctrl + P och skriva 
snip och välja Inster Snippet så får vi upp listan på alla tillgängliga snippets.

Väljer vi t ex If så får vi vi en kodsnutt för hur vi skriver en If-sats.

## Tweaka som PowerShell ISE

Om man har kört PowerShell ISE länge så har man vant sig vid vissa saker som inte är standard i Visual Studio Code.

Jag saknade dessa två på en gång:

- Zooma/Ändra fontstorlek med Mouse Wheel

    Står man i skript delen i PowerShell ISE så kan man hålla inne shift och skrolla med Mouse Wheel för att ändra fontstorleeken.

    Mycket enklare än att behöva gå in isettings och ändra varje gång man vill ändra.

    Detta gör vi genom att lägga till en rad i vår inställnings json fil.

    Shift + Ctrl + P

    Skriv Preferences: Open Settings och välj den med Preferences: Open Settings (JSON)

    Lägg till "    "editor.mouseWheelZoom": true,"

    Nu kan man använda Shift +  Mouse Wheel

- Slå på Tabcompletion

    Tabcompletion finns men är avslagen som standard.

    Shift + Ctrl + P

    Open User Settings

    Sök på Tab

    Under Editor: Tab Completion ändra till On.

    Nu kan du skriva Get- och tabba dig fram om du vill!