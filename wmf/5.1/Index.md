---
ms.date: 08/12/2017
ms.topic: conceptual
keywords: wmf,powershell,setup
title: Anmerkungen zu dieser Version – WMF 5.1
ms.openlocfilehash: 3512d2e80501a596e1fd6d7b33d4d75286cef1b9
ms.sourcegitcommit: 54534635eedacf531d8d6344019dc16a50b8b441
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/16/2018
ms.locfileid: "34189787"
---
# <a name="windows-management-framework-wmf-51"></a>Windows Management Framework (WMF) 5.1 #

WMF ermöglicht es Benutzern, bestehende Windows-Systeme auf die Versionen der Komponenten von PowerShell, WMI, WinRM und der Softwareinventurprotokollierung zu aktualisieren, die mit Windows Server 2016 veröffentlicht wurden.

WMF 5.1 kann auf Windows 7, Windows 8.1, Windows Server 2008 R2, 2012 und 2012 R2 installiert werden und bietet gegenüber WMF 5.0 RTM eine Reihe von Vorteilen. Dazu zählen u. a.:

- Neue Cmdlets: lokale Benutzer und Gruppen; Get-ComputerInfo
- PowerShellGet-Verbesserungen wie z. B. die Durchsetzung von signierten Modulen und die Installation von JEA-Modulen
- Bei PackageManagement wurde Unterstützung für Container, CBS-Setup, EXE-basiertes Setup und CAB-Pakete hinzugefügt
- Debuggingverbesserungen für DSC und PowerShell-Klassen
- Sicherheitsverbesserungen wie u. a. die Durchsetzung von katalogsignierten Modulen vom Pullserver und bei Verwendung von PowerShellGet-Cmdlets
- Antworten auf verschiedene Benutzeranfragen und zu Problemen

Weitere Informationen zu den Neuerungen in dieser Version finden Sie in den Themen, die unter [New Scenarios and Features (Neue Szenarios und Features)](https://docs.microsoft.com/en-us/powershell/wmf/5.1/scenarios-features) aufgelistet sind.

Das Thema [Install and Configure (Installieren und Konfigurieren)](https://docs.microsoft.com/en-us/powershell/wmf/5.1/install-configure) listet die Anforderungen auf und enthält Installationsanweisungen für WMF.

Das Thema [Compatibility (Kompatibilität)](https://docs.microsoft.com/en-us/powershell/wmf/5.1/compatibility) listet auf, welche Versionen von WMF auf welchen Windows-Versionen installiert werden können.

Das Thema [Product Compatibility (Produktkompatibilität)](https://docs.microsoft.com/en-us/powershell/wmf/5.1/productincompat) listet die Microsoft-Anwendungen auf, die derzeit noch nicht für die Verwendung mit WMF 5.1 genehmigt wurden.

Weitere Details zu den Komponenten von WMF finden Sie in der MSDN-Dokumentation:

- [PowerShell 5.1](https://docs.microsoft.com/en-us/powershell/)
- [WMI](https://msdn.microsoft.com/en-us/library/jj152383(v=vs.85).aspx)
- [WinRM](https://msdn.microsoft.com/en-us/library/aa384426(v=vs.85).aspx)
- [Softwareinventurprotokollierung](https://technet.microsoft.com/en-us/library/dn383584(v=ws.11).aspx)
