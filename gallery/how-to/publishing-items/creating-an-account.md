---
ms.date: 06/12/2017
contributor: JKeithB
keywords: gallery,powershell,cmdlet,psgallery
title: Erstellen eines PowerShell-Katalogkontos
ms.openlocfilehash: 4a44b51967ea8acdd331f6b3c682fc5884bd2f54
ms.sourcegitcommit: 54534635eedacf531d8d6344019dc16a50b8b441
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/17/2018
ms.locfileid: "34219564"
---
## <a name="creating-a-powershell-gallery-account"></a>Erstellen eines PowerShell-Katalogkontos

Bevor Elemente im PowerShell-Katalog veröffentlicht werden können, muss ein PowerShell-Katalogkonto eingerichtet werden.
Das PowerShell-Katalogkonto muss mit einem E-Mail-aktivierten Azure Active Directory-Konto oder mit einem Microsoft-E-Mail-Konto (mit der Domäne outlook.com, hotmail.com usw.) verknüpft werden.

Besuchen Sie https://PowerShellGallery.com, und klicken Sie auf „Register“ (Registrieren), um ein PowerShell-Katalogkonto zu erstellen (siehe Abbildung unten).

![Registrieren eines neuen Kontos](../../Images/CreatingAccount-Register.png)

Verwenden Sie auf der nächsten Seite ein Azure Active Directory-Konto, wählen Sie „Work or School Account“ (Geschäfts-, Schul- oder Unikonto) aus, und melden Sie sich mit Ihrem Konto an.
Um ein Microsoft-Konto zu verwenden – beispielsweise in der Domäne Hotmail.com oder Outlook.com –, wählen Sie „Personal Account“ (Privates Konto) aus, und melden Sie sich an. 

Nach der Anmeldung werden Sie aufgefordert, einen Benutzernamen für den PowerShell-Katalog zu erstellen.
Lesen Sie die verlinkten Nutzungsbestimmungen und die Datenschutzrichtlinie, geben Sie einen Benutzernamen ein, und klicken Sie dann auf „Register“ (Registrieren).

Hinweis: Dieser Kontoname kann nach der Erstellung nicht mehr geändert werden.
Weitere Informationen hierzu finden Sie unter [Verwalten von Elementbesitzern](https://msdn.microsoft.com/powershell/gallery/psgallery/managing-item-owners).

## <a name="recommended-practices-for-powershell-gallery-accounts"></a>Empfohlene Vorgehensweisen für PowerShell-Katalogkonten

Es ist wichtig, dass mit Ihrem PowerShell-Katalogkonto verwendete E-Mail-Konto aktiv zu überwachen.
Die gesamte Kommunikation mit Besitzern von PowerShell-Katalogelementen erfolgt über die E-Mail-Adresse, die Ihrem PowerShell-Katalogkonto zugeordnet ist.
Wenn Sie einen Elementbesitzer nicht erreichen können, kann es unter bestimmten Umständen erforderlich sein, ein Element durch das Team für den Katalogbetrieb löschen zu lassen.

Organisationen, die Elemente im PowerShell-Katalog veröffentlichen, erstellen zu diesem Zweck häufig ein eindeutiges Konto in Outlook.com oder einer anderen Microsoft-Kontodomäne.
Oft wird dieses Konto nicht regelmäßig überwacht.
Eine bewährte Methode ist in diesem Fall die Outlook-Weiterleitung von E-Mails an ein anderes Konto – typischerweise innerhalb der Organisation –, das vom Elementbesitzer überwacht wird.

Wenn einem Element mehrere Besitzer zugeordnet sind, wird die gesamte vom PowerShell-Katalog ausgehende Kommunikation an alle Benutzer gesendet.
Ausführliche Informationen zum Hinzufügen von Besitzern zu einem Element finden Sie unter [Verwalten von Elementbesitzern](https://msdn.microsoft.com/powershell/gallery/psgallery/managing-item-owners).