---
title: included-file-redirected
description: Vysvětlení a řešení problému sestavení included-file-redirected na webu Docs
author: meganbradley
ms.author: mbradley
ms.topic: error-reference
ms.date: 3/1/2019
ms.prod: non-product-specific
ms.openlocfilehash: 8a40f04fe1a7e7f19ab9ee7ce684684184aa4dc7
ms.sourcegitcommit: 89eb357721b26710e00d9b8fdab3e7628c34bdb6
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 03/06/2019
ms.locfileid: "57459066"
---
# <a name="included-file-redirected"></a>included-file-redirected

## <a name="warning"></a>Upozornění

`Included file '{include path}' is redirected to '{target file path}'. Only include files that are not redirected and that are located in an includes folder.`

## <a name="resolution"></a>Řešení

Změňte strukturu obsahu tak, aby se přesměrovaný soubor nezahrnoval. Například vytvořte nový soubor, který se má zahrnout, nebo odeberte zahrnutý odkaz a vytvořte odkaz na obsah nebo ho zadejte jako vložený.

<!--make sure to add this file to your includes folder and verify the path-->
[!INCLUDE [validation-reference-help](includes/validation-reference-help.md)]
