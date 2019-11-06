# 02 Utöka verktygslådan

Jag brukar säga att PowerShell är en verktygslåda med många bra verktyg och ett sätt för att utöka verktygslådan är att installera moduler.

## Moduler

- Genom att skapa moduler med skript, funktioner och cmdlets kan man utöka funktionaliteten snabbt och enkelt

- Det finns många färdiga moduler

- Många tillverkare skapar moduler som de levererar med sina produkter eller lägger tillgängliga på PowerShell Gallery eller på sina hemsidor.

## Installera och använda

- Install-Module

För att installera via PSGallery

- Get-Module

För att se om modulen finns i sessionen eller är tillgänglig på datorn.

- Import-Module

Lägger till modulen i sessionen

- Get-Command –module %namnet på modulen%

Listar kommandon från modulen

Dessutom finns det leverantörer som har skapat moduler för att stödja sina produkter.

För att t ex få Active Directory modulen från Microsoft på en icke server så behöver vi installera RSAT och välja att lägga till modulen.

## PowerShell Gallery

- Vad är PowerShell gallery?

    Ett centralt arkiv för delning och hämtning av PowerShell moduler, skript och Desired State Configuration (DSC) resurser.

    Idag finns det över 5800 unika paket att hämta hem.

    För att detta ska fungera behöver man modulen PowerShellGet och nyare PowerShell än 3.0.

    Kör man Windows 10 så ingår PowerShellGet.

    För att få reda på vilka kommandon vi har att tillgå via PowerShellGet så skriver vi:

    Get-Command -Module PowerShellGet

- Hur kommer jag åt det som finns där?

    www.powershellgallery.com  
    Eller att föredra via Find-Module  
    Och sedan Install-Module

## Vanliga moduler

Det finns som sagt MÅNGA moduler att använda och vad man har nytta av beror ju helt och hållet på vad man jobbar med eller är intresserad av.

Mina favoriter är:

- PSScriptAnalyzer – Analysera din PowerShell Kod

    Ingår i Visual Studio Code extensionen PowerShell.

    Bygger på best practice regler från PowerShell Teamet och PowerShell communityn.

- PSWindowsUpdate – Jobba med Windows Update

    Få bra kontroll över Windows Update.
    T ex Windows Update History, hur har installationen av uppdateringar gått eller inte gått.

- Pester – Testramverk

    För att köra och validera PowerShell skripts

- Posh-Git – För Git

    Bland annat Git status information och Tab completion för Git

- PSReadline – Utvecklad command line

- PowerCLI - VMWare

- Hyper-V - Microsoft

- Posh-SSH - SSH

    SSH och SCP funktionalitet via PowerShell

- Microsoft Active Directory

    För att managera Active Directory med PowerShell

- Dbatools

    SQL managering

- QRCodeGenerator

    Skapa QR koder för VCard, Geolocation och WiFi

