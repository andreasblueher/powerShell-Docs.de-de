---
ms.date: 2017-06-05T00:00:00.000Z
keywords: powershell,cmdlet
title: Grundlagen von Windows PowerShell
ms.assetid: 6b3cbbc8-060c-4877-b00b-7300dbbe4e28
ms.openlocfilehash: f8a520f1fbe97737c7d0c2acab0129f88b5ed425
ms.sourcegitcommit: 74255f0b5f386a072458af058a15240140acb294
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/03/2017
---
# <a name="windows-powershell-basics"></a>Grundlagen von Windows PowerShell
Grafische Benutzeroberflächen basieren auf Grundkonzepten, die den meisten Computerbenutzern bekannt sind. Benutzer verlassen sich beim Ausführen von Aufgaben auf die Vertrautheit mit diesen Oberflächen. Betriebssysteme bieten Benutzern eine grafische Darstellung von Elementen, die durchsucht werden können, meist mit Einblendmenüs für den Zugriff auf bestimmte Funktionen und Kontextmenüs für den Zugriff auf kontextspezifische Funktionalität.

Eine Befehlszeilenschnittstelle (Command-Line Interface, CLI) wie Windows PowerShell muss einen anderen Ansatz zum Offenlegen von Informationen befolgen, da sie nicht über Menüs oder grafische Systeme verfügt, die dem Benutzer helfen. Sie müssen Namen von Befehlen kennen, bevor Sie sie verwenden können. Obwohl Sie komplexe Befehle eingeben können, die mit den Features in einer grafischen Umgebung äquivalent sind, müssen Sie sich mit den am häufigsten verwendeten Befehlen und deren Parametern vertraut machen.

Die meisten CLIs bieten keine Muster, die dem Benutzer helfen, die Schnittstelle zu erlernen. Da CLIs die ersten Betriebssystemshells waren, wurden viele Befehls- und Parameternamen nach dem Zufallsprinzip ausgewählt. Dabei erhielten kurze und knappe Befehlsnamen meist den Vorzug vor aussagekräftigeren Namen. Obwohl Hilfesystemen und Befehlsentwurfsstandards in die meisten CLIs integriert wurden, sind diese in der Regel auf Kompatibilität mit den frühesten Befehlen ausgelegt, sodass der Befehlssatz weiter von Entscheidungen geprägt ist, die vor Jahrzehnten getroffen wurden.

Windows PowerShell wurde so entwickelt, dass die historischen CLI-Kenntnisse der Benutzer weiter zum Tragen kommen. In diesem Kapitel beschäftigen wir uns mit einigen grundlegenden Tools und Konzepten, mit deren Hilfe Sie Windows PowerShell schnell erlernen können. Dazu gehören:

-   Verwenden von „Get-Command“

-   Verwenden von „Cmd.exe“ und UNIX-Befehlen

-   Verwenden externer Befehle

-   Verwenden der Vervollständigung mit der TAB-TASTE

-   Verwenden von „Get-Help“
