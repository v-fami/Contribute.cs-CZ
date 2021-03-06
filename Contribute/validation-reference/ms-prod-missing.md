---
title: ms-prod-missing
description: Vysvětlení a řešení problému sestavení ms-prod-missing na webu Docs
author: meganbradley
ms.author: mbradley
ms.topic: error-reference
ms.date: 2/2/2019
ms.prod: non-product-specific
ms.openlocfilehash: ee29396a20345f6884a5bbc94aa25f48dafaff52
ms.sourcegitcommit: 203ca15fda2d217f082c74ec648c1f1db323f9f1
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 02/04/2019
ms.locfileid: "55713216"
---
# <a name="ms-prod-missing"></a>ms-prod-missing

**Připravujeme**

[!INCLUDE [suggestion-note](includes/suggestion-note.md)]

## <a name="suggestion"></a>Návrh

`Missing attribute: ms.prod. If you specify ms.technology, you must also specify ms.prod.`

K zadání místních produktů používejte `ms.prod`. Pokud chcete o `ms.prod` zadat podrobnější informace, můžete volitelně zadat `ms.technology`, ale pokud zadáte `ms.technology`, musíte také zadat `ms.prod`. Hodnoty `ms.prod` a `ms.technology` musí tvořit platnou dvojici.

## <a name="resolution"></a>Řešení

Ujistěte se, jestli je vámi zadaná hodnota `ms.technology` pro váš článek správná. Potom přidejte příslušnou hodnotu `ms.prod`, která je platným nadřazeným objektem pro `ms.technology`.

Platné hodnoty se dají najít na [tomto interním webu Microsoftu](https://docsmetadatatool.azurewebsites.net/whitelists).

<!--make sure to add this file to your includes folder and verify the path-->
[!INCLUDE [validation-reference-help](includes/validation-reference-help.md)]
