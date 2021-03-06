---
title: ms-date-too-late
description: Vysvětlení a řešení problému sestavení ms-date-too-late na webu Docs
author: meganbradley
ms.author: mbradley
ms.topic: error-reference
ms.date: 1/15/2019
ms.prod: non-product-specific
ms.openlocfilehash: b38392e9f297e4ee4147ca7fc65f938b5cd53403
ms.sourcegitcommit: f374ad2607360f46d88982b4b7ecc63d3ab08235
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/20/2019
ms.locfileid: "56431477"
---
# <a name="ms-date-too-late"></a>ms-date-too-late

**Připravujeme**

## <a name="warning"></a>Upozornění

`Invalid value for ms.date. The freshness date can't be more than five days in the future.`

Atribut `ms.date` se používá k indikaci „aktuálnosti“ – to znamená, kdy byl článek naposledy zkontrolován z hlediska relevance, přesnosti, správných snímků obrazovek a funkčních odkazů. Proto nemůže být v budoucnosti. S pěti dny můžete počítat na dobu vydání – například když je obsah zmrazený kvůli kontrole kvality při přípravě na nějakou důležitou událost.

## <a name="resolution"></a>Řešení

Zadejte `ms.date` ve formátu MM/DD/RRRR. Datum nesmí být od dnešního dne vzdálenější než pět dnů.

```yml
---
ms.date: 02/19/2019
---
```

<!--make sure to add this file to your includes folder and verify the path-->
[!INCLUDE [validation-reference-help](includes/validation-reference-help.md)]
