---
title: Jak přispívat na docs.microsoft.com
description: Tento článek poskytuje přehled různých způsobů, jak se dá přispívat k obsahu na web docs.microsoft.com.
author: billwagner
ms.author: wiwagn
manager: wpickett
ms.date: 01/17/2018
ms.prod: non-product-specific
ms.topic: contributor-guide
ms.custom: external-contributor-guide
ms.openlocfilehash: bc6f9c314eda5f0d950da049374a7a157f16782a
ms.sourcegitcommit: de6e6b6ca641fdd5b30eb46deee9ac3a500089ef
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/28/2018
---
# <a name="how-to-contribute-to-docsmicrosoftcom"></a><span data-ttu-id="0e731-103">Jak přispívat na docs.microsoft.com</span><span class="sxs-lookup"><span data-stu-id="0e731-103">How to contribute to docs.microsoft.com</span></span>

<span data-ttu-id="0e731-104">Existuje několik způsobů, jak se zúčastnit vylepšování obsahu na [docs.microsoft.com](https://docs.microsoft.com):</span><span class="sxs-lookup"><span data-stu-id="0e731-104">There are several ways to participate in improving the content that makes up [docs.microsoft.com](https://docs.microsoft.com):</span></span>

- <span data-ttu-id="0e731-105">Pokud chcete doporučit nové články nebo vylepšit stávající články, můžete [vytvářet problémy](#create-issues) (nadnést problém).</span><span class="sxs-lookup"><span data-stu-id="0e731-105">You can [create issues](#create-issues) to recommend new articles, or improve existing articles.</span></span>
- <span data-ttu-id="0e731-106">V online editoru GitHubu můžete dělat malé změny a články [rychle upravovat](#quick-edits).</span><span class="sxs-lookup"><span data-stu-id="0e731-106">You can [quickly edit](#quick-edits) articles to make small changes in the GitHub online editor.</span></span>
- <span data-ttu-id="0e731-107">[Revizemi konceptů nových článků](#review-new-articles) zajistíte kvalitu a technickou přesnost.</span><span class="sxs-lookup"><span data-stu-id="0e731-107">You can [review drafts of new articles](#review-new-articles) to ensure quality and technical accuracy.</span></span>
- <span data-ttu-id="0e731-108">Pokud chcete sami podpořit rozšiřování obsahu, můžete k důležitým tématům [vytvářet nové články](#create-new-articles).</span><span class="sxs-lookup"><span data-stu-id="0e731-108">You can [create new articles](#create-new-articles) for topics when you want to help drive the content story.</span></span>
- <span data-ttu-id="0e731-109">[Aktualizací](#update-samples) a [vytvářením](#create-samples) ukázek můžete vylepšovat ukázky kódu, které posilují důležité koncepce.</span><span class="sxs-lookup"><span data-stu-id="0e731-109">You can [update](#update-samples) or [create](#create-samples) samples to improve the code samples that reinforce important concepts.</span></span>

<span data-ttu-id="0e731-110">V tomto článku se seznámíte s různými způsoby přispívání, poznáte, jak se tyto úkoly provádějí, a najdete odkazy na další informace o těchto úkolech.</span><span class="sxs-lookup"><span data-stu-id="0e731-110">In this article, you'll learn the different ways to contribute, see how to accomplish each of those tasks, and find pointers to more information about each of those tasks.</span></span>

<span data-ttu-id="0e731-111">Naše veřejná úložiště jsou hostovaná na [GitHubu](https://wwww.GitHub.com).</span><span class="sxs-lookup"><span data-stu-id="0e731-111">Our public repositories are hosted on [GitHub](https://wwww.GitHub.com).</span></span>  <span data-ttu-id="0e731-112">Pokud se chcete na našich úložištích dokumentace podílet, musíte si na GitHubu vytvořit účet.</span><span class="sxs-lookup"><span data-stu-id="0e731-112">You will need to create an account on GitHub to participate in our documentation repositories.</span></span>

<span data-ttu-id="0e731-113">K aktualizaci dokumentů budete také potřebovat textový editor.</span><span class="sxs-lookup"><span data-stu-id="0e731-113">You'll also need a text editor to update the documents.</span></span> <span data-ttu-id="0e731-114">Doporučujeme editor [Visual Studio Code](https://www.visualstudio.com/code).</span><span class="sxs-lookup"><span data-stu-id="0e731-114">We recommend [Visual Studio Code](https://www.visualstudio.com/code).</span></span> <span data-ttu-id="0e731-115">Měli byste mít základní znalosti syntaxe jazyka [Markdown](https://daringfireball.net/projects/markdown/syntax).</span><span class="sxs-lookup"><span data-stu-id="0e731-115">You should have a basic understanding of [Markdown](https://daringfireball.net/projects/markdown/syntax) syntax.</span></span>

<span data-ttu-id="0e731-116">Pokud chcete přidávat nebo upravovat ukázky, budete potřebovat vývojové prostředí.</span><span class="sxs-lookup"><span data-stu-id="0e731-116">If you are adding or modifying samples, you'll need a development environment.</span></span> <span data-ttu-id="0e731-117">Pro počítače PC nebo Mac doporučujeme [Visual Studio](https://www.visualstudio.com), pro všechny platformy se hodí [Visual Studio Code](https://www.visualstudio.com/code).</span><span class="sxs-lookup"><span data-stu-id="0e731-117">We recommend [Visual Studio](https://www.visualstudio.com) on PC and Mac, or [Visual Studio Code](https://www.visualstudio.com/code) on all platforms.</span></span>

## <a name="create-issues"></a><span data-ttu-id="0e731-118">Vytváření problémů</span><span class="sxs-lookup"><span data-stu-id="0e731-118">Create issues</span></span>

<span data-ttu-id="0e731-119">Pokud v nějakém článku najdete opomenutí nebo nepřesnosti, můžete k tomuto článku vytvořit (nadnést) problém.</span><span class="sxs-lookup"><span data-stu-id="0e731-119">If you find omissions or inaccuracies in a article, create an issue against that article.</span></span> <span data-ttu-id="0e731-120">Správné umístění najdete nejsnadněji tak, že v prohlížeči kliknete na tlačítko Upravit. Tak se dostanete ke zdroji článku ve správném veřejném úložišti GitHubu.</span><span class="sxs-lookup"><span data-stu-id="0e731-120">The easiest way to find the right location is to click the "Edit" button in your browser, which will take you to the article source in the correct public GitHub repository.</span></span> <span data-ttu-id="0e731-121">Na panelu Adresa pak můžete zjistit adresu URL zdroje článku.</span><span class="sxs-lookup"><span data-stu-id="0e731-121">From there, you can retrieve the URL for the source of the article from your address bar.</span></span> <span data-ttu-id="0e731-122">Nový problém k článku vytvoříte kliknutím na tlačítko Vytvořit problém.</span><span class="sxs-lookup"><span data-stu-id="0e731-122">Click "Create Issue" to make a new issue on the article.</span></span>

> [!NOTE]
> <span data-ttu-id="0e731-123">Pokud najdete problémy, které se dají opravit malými úpravami, například překlepy nebo gramatické chyby, můžete ušetřit čas sobě i nám tím, že pomocí prohlížeče [odešlete žádost o opravu](#quick-edits) zdroje.</span><span class="sxs-lookup"><span data-stu-id="0e731-123">If you find issues you can fix with small edits, such as typing mistakes or grammar issues, you can save yourself and us time by [submitting the fix](#quick-edits) using the browser to edit the source.</span></span>

<span data-ttu-id="0e731-124">Většina našich veřejných úložišť obsahuje šablony pro nové problémy, které vás povedou při poskytování informací potřebných k opravě problému.</span><span class="sxs-lookup"><span data-stu-id="0e731-124">Most of our public repos contain templates for new issues that will guide you to provide the information needed to fix the issue.</span></span>

<span data-ttu-id="0e731-125">Novými problémy můžete přispívat také v případech, kdy nemůžete najít potřebné informace.</span><span class="sxs-lookup"><span data-stu-id="0e731-125">You can also contribute new issues where you can't find the information you need.</span></span> <span data-ttu-id="0e731-126">Postup je stejný: Vytvoříte nový problém v jednom z veřejných úložišť dokumentů</span><span class="sxs-lookup"><span data-stu-id="0e731-126">The process is the same: create a new issue on one of the public docs repositories.</span></span> <span data-ttu-id="0e731-127">a sdělíte nám, co hledáte, co jste chtěli udělat a proč vám nepomohly články, které jste našli.</span><span class="sxs-lookup"><span data-stu-id="0e731-127">Tell us what you were searching for, what you wanted to do, and why the articles you found did not help the way you expected.</span></span>

## <a name="review-new-articles"></a><span data-ttu-id="0e731-128">Revize nových článků</span><span class="sxs-lookup"><span data-stu-id="0e731-128">Review new articles</span></span>

<span data-ttu-id="0e731-129">Pokud pracujete s novým softwarem (nejspíš ve verzi CTP nebo beta), může se stát, že v době, kdy se s touto technologií seznamujete, dokumentaci vytváříme.</span><span class="sxs-lookup"><span data-stu-id="0e731-129">If you are working on new, possibly CTP or beta, software, we are likely building the docs as you are exploring the technology.</span></span> <span data-ttu-id="0e731-130">V našich veřejných úložištích tak můžete najít rozpracované dokumenty.</span><span class="sxs-lookup"><span data-stu-id="0e731-130">You can find the in-process docs in our public repositories.</span></span> <span data-ttu-id="0e731-131">Svými komentáři nám můžete pomoct dokumenty vylepšit, než je vydáme.</span><span class="sxs-lookup"><span data-stu-id="0e731-131">If you have comments, you can help us make them better before they are released.</span></span>

<span data-ttu-id="0e731-132">Nové články se revidují veřejně – použitím [pracovního postupu GitHubu](https://guides.github.com/introduction/flow/).</span><span class="sxs-lookup"><span data-stu-id="0e731-132">New articles are reviewed in public, using the [GitHub flow](https://guides.github.com/introduction/flow/) process.</span></span> <span data-ttu-id="0e731-133">Podívejte se na libovolné z našich úložišť dokumentů a zkontrolujte otevřené žádosti o přijetí změn.</span><span class="sxs-lookup"><span data-stu-id="0e731-133">Look at any of our docs repositories, and check the open pull requests (PRs).</span></span> <span data-ttu-id="0e731-134">Komentáře a revize k otevřeným žádostem o přijetí změn vítáme.</span><span class="sxs-lookup"><span data-stu-id="0e731-134">We welcome comments and reviews on any open pull requests.</span></span> <span data-ttu-id="0e731-135">Pomůže nám to publikovat lepší obsah při prvním vydání, místo toho, abychom čekali na vaše názory až po zveřejnění.</span><span class="sxs-lookup"><span data-stu-id="0e731-135">That helps us publish better content on our first release, rather than waiting for feedback after going live.</span></span>

<span data-ttu-id="0e731-136">Hledáme způsoby, jak vylepšit technickou přesnost, srozumitelnost popisů a mluvnickou správnost.</span><span class="sxs-lookup"><span data-stu-id="0e731-136">We are looking for ways to improve technical accuracy, clarity of the descriptions, and grammatical accuracy.</span></span>

## <a name="quick-edits"></a><span data-ttu-id="0e731-137">Rychlé úpravy</span><span class="sxs-lookup"><span data-stu-id="0e731-137">Quick edits</span></span>

<span data-ttu-id="0e731-138">Rychlé úpravy představují způsob, jak dělat malé opravy pomocí editoru založeného na prohlížeči.</span><span class="sxs-lookup"><span data-stu-id="0e731-138">Quick edits are a way to make small fixes using the browser based editor.</span></span> <span data-ttu-id="0e731-139">Pokud najdete drobné pravopisné nebo gramatické chyby nebo chybné názvy rozhraní API, nemusíte vytvářet problém. Uděláte úpravy a odešlete žádost o přijetí změn.</span><span class="sxs-lookup"><span data-stu-id="0e731-139">If you find small spelling or grammar errors, or mis-named APIs, you can skip creating an issue by making the edit and submitting a PR.</span></span>

<span data-ttu-id="0e731-140">V libovolném článku klikněte na tlačítko Upravit (obvykle je poblíž pravého horního rohu stránky), udělejte úpravy a klikněte v dolní části stránky na tlačítko Odeslat žádost o přijetí změn.</span><span class="sxs-lookup"><span data-stu-id="0e731-140">On any article, click the "Edit" button (usually toward the top right-hand side of the page), make your edits, and click "Submit PR" at the bottom of the page.</span></span> <span data-ttu-id="0e731-141">My žádost o přijetí změn v rámci denní revize žádostí zkontrolujeme a začleníme.</span><span class="sxs-lookup"><span data-stu-id="0e731-141">We'll review the PR, and merge it as we do our daily PR review.</span></span>

## <a name="create-new-articles"></a><span data-ttu-id="0e731-142">Vytváření nových článků</span><span class="sxs-lookup"><span data-stu-id="0e731-142">Create new articles</span></span>

<span data-ttu-id="0e731-143">Pokud se vážně zabýváte některými tématy a chcete je vysvětlit ostatním, můžete vytvořit články a odeslat žádosti o přijetí změn.</span><span class="sxs-lookup"><span data-stu-id="0e731-143">If there are concepts you are passionate about, and want to explain to others, you can create the articles and submit a PR.</span></span>

<span data-ttu-id="0e731-144">Vytváření nových článků je časově náročné. Oceňujeme vaše úsilí a příspěvky.</span><span class="sxs-lookup"><span data-stu-id="0e731-144">Creating new articles is time-consuming, and we value your time and contributions.</span></span> <span data-ttu-id="0e731-145">Chceme se tohoto procesu od začátku zúčastnit, abychom se ujistili, že dodržujete naše pokyny a styl.</span><span class="sxs-lookup"><span data-stu-id="0e731-145">We want to be involved early in the process to ensure you're following our guidelines and style from the beginning.</span></span> <span data-ttu-id="0e731-146">Doporučujeme tento postup:</span><span class="sxs-lookup"><span data-stu-id="0e731-146">We recommend the following steps:</span></span>

1. <span data-ttu-id="0e731-147">[Vytvořte problém](#create-issues), který popisuje, co chybí a jak to chcete řešit.</span><span class="sxs-lookup"><span data-stu-id="0e731-147">[Create an issue](#create-issues) describing what's missing and how you'd address it.</span></span>
1. <span data-ttu-id="0e731-148">Okomentujte problém – sdělte nám, jak byste na něm chtěli pracovat, a navrhněte osnovu a obsah článku.</span><span class="sxs-lookup"><span data-stu-id="0e731-148">Comment on the issue, telling us you'd like to work on it, and suggesting an outline and abstract for the article.</span></span>
1. <span data-ttu-id="0e731-149">Budeme reagovat svými návrhy.</span><span class="sxs-lookup"><span data-stu-id="0e731-149">We'll respond with suggestions.</span></span> <span data-ttu-id="0e731-150">Ty můžou zahrnovat odkazy na související články, návrhy ukázek nebo způsob uspořádání článku.</span><span class="sxs-lookup"><span data-stu-id="0e731-150">These may include links to related articles, suggestions for samples, or how the article will be organized.</span></span>
1. <span data-ttu-id="0e731-151">Až osnovu odsouhlasíme, vytvořte fork úložiště a začněte pracovat.</span><span class="sxs-lookup"><span data-stu-id="0e731-151">Once we agree on the outline, fork the repository, and start working.</span></span>
1. <span data-ttu-id="0e731-152">V rané fázi procesu otevřete žádost o přijetí změn s označením „[Rozpracováno]“ na začátku názvu.</span><span class="sxs-lookup"><span data-stu-id="0e731-152">Early in the process, open a PR, with "[WIP]" at the beginning of the title.</span></span>
1. <span data-ttu-id="0e731-153">Jeden z klíčových přispěvatelů vám pošle svůj počáteční názor.</span><span class="sxs-lookup"><span data-stu-id="0e731-153">One of the core contributors will give you initial feedback.</span></span>
1. <span data-ttu-id="0e731-154">Pokračujte v psaní, a až budete připravení na další názory, @-mention osobu, která revidovala první koncept.</span><span class="sxs-lookup"><span data-stu-id="0e731-154">Keep writing, @-mention the person who reviewed the first draft when you're ready for more feedback.</span></span>
1. <span data-ttu-id="0e731-155">Až budete připravení na konečnou revizi, odstraňte z názvu „[Rozpracováno]“.</span><span class="sxs-lookup"><span data-stu-id="0e731-155">Remove the "[WIP]" when you're ready for final review.</span></span>
1. <span data-ttu-id="0e731-156">Reagujte na názory.</span><span class="sxs-lookup"><span data-stu-id="0e731-156">Respond to the feedback</span></span>
1. <span data-ttu-id="0e731-157">Klíčoví přispěvatelé vaši žádost o přijetí změn začlení.</span><span class="sxs-lookup"><span data-stu-id="0e731-157">The core contributors will merge your PR.</span></span>

<span data-ttu-id="0e731-158">Několik bodů tohoto seznamu stojí za to rozepsat podrobněji.</span><span class="sxs-lookup"><span data-stu-id="0e731-158">There are a couple points worth expanding on from that list.</span></span> <span data-ttu-id="0e731-159">Obecně platí, že v souladu s [pracovním postupem GitHubu](https://guides.github.com/introduction/flow/) revidujeme obsah co nejdříve.</span><span class="sxs-lookup"><span data-stu-id="0e731-159">In general, we're following the [GitHub flow](https://guides.github.com/introduction/flow/) process to review content as early as possible.</span></span> <span data-ttu-id="0e731-160">Tímto způsobem odsouhlasíme, kde bude článek zařazený v obsahu, co článek přinese čtenářům a na co se zaměří vytvořené ukázky.</span><span class="sxs-lookup"><span data-stu-id="0e731-160">That way, we agree on where an article should go in the table of contents, what benefit the reader will get from the new article, and the scope of any samples you'll create.</span></span> <span data-ttu-id="0e731-161">Můžeme vás tak včas korigovat, než vynaložíte spoustu času na psaní textu.</span><span class="sxs-lookup"><span data-stu-id="0e731-161">We can make any necessary course corrections early, before you've invested significant time writing.</span></span>

## <a name="update-samples"></a><span data-ttu-id="0e731-162">Aktualizace ukázek</span><span class="sxs-lookup"><span data-stu-id="0e731-162">Update samples</span></span>

<span data-ttu-id="0e731-163">Některé ukázky můžou být původně napsané pro předchozí verze s použitím již nedoporučovaných postupů.</span><span class="sxs-lookup"><span data-stu-id="0e731-163">Some samples may have originally been written several releases ago, using practices no long recommended.</span></span> <span data-ttu-id="0e731-164">Takové ukázky nám můžete pomoct aktualizovat.</span><span class="sxs-lookup"><span data-stu-id="0e731-164">You may want to help us update those samples.</span></span> <span data-ttu-id="0e731-165">Nebo například můžete přijít na to, že jednoduchá změna názvu proměnné může zlepšit srozumitelnost výkladu.</span><span class="sxs-lookup"><span data-stu-id="0e731-165">Or, you may find that a simple variable name change could increase the clarity of an explanation.</span></span>

<span data-ttu-id="0e731-166">Vzorové (ukázkové) kódy zobrazené v jednotlivých článcích jsou součástí programů, které sestavujeme a často testujeme v systému kontinuální integrace (CI).</span><span class="sxs-lookup"><span data-stu-id="0e731-166">The sample code displayed with each article are part of programs that are built and often tested under our CI system.</span></span>

<span data-ttu-id="0e731-167">Pokud chcete udělat malé aktualizace, najděte zdroj v příslušném úložišti, změňte kód v prohlížeči a odešlete žádost o přijetí změny.</span><span class="sxs-lookup"><span data-stu-id="0e731-167">To make small updates, you find the source in the appropriate repository, make the code change in the browser and submit a PR.</span></span> <span data-ttu-id="0e731-168">Náš systém CI změny sestaví, a až skončí, začlení žádost o přijetí změn.</span><span class="sxs-lookup"><span data-stu-id="0e731-168">Our CI system will build the changes, and we'll merge the PR when it finishes.</span></span>

<span data-ttu-id="0e731-169">Pokud chcete udělat rozsáhlejší změny, vytvořte fork úložiště a proveďte změny ve svém oblíbeném vývojovém prostředí.</span><span class="sxs-lookup"><span data-stu-id="0e731-169">For larger scale changes fork the repository and make the changes in your favorite development environment.</span></span> <span data-ttu-id="0e731-170">Nezapomeňte přidat nějaké testy, abyste zajistili, že vaše změny budou fungovat, jak mají.</span><span class="sxs-lookup"><span data-stu-id="0e731-170">Make sure you add some tests to ensure that your changes work as you intended.</span></span> <span data-ttu-id="0e731-171">Odešlete žádost o přijetí změn a my ji zkontrolujeme.</span><span class="sxs-lookup"><span data-stu-id="0e731-171">Submit a PR, and we'll review it.</span></span>

<span data-ttu-id="0e731-172">Při všech změnách kódu dodržujte stávající zásady vzorového (ukázkového) kódu, který upravujete.</span><span class="sxs-lookup"><span data-stu-id="0e731-172">With all code changes, follow the existing code conventions for the sample code you are modifying.</span></span> <span data-ttu-id="0e731-173">Naše standardy kódování úložišť ukázek budou odrážet standardy odpovídajících produktových týmů.</span><span class="sxs-lookup"><span data-stu-id="0e731-173">Our samples repositories coding standards will mirror those of the corresponding product teams.</span></span> <span data-ttu-id="0e731-174">Řiďte se konkrétními pokyny pro každé úložiště.</span><span class="sxs-lookup"><span data-stu-id="0e731-174">Check each repository for specific guidance.</span></span>

> [!NOTE]
> <span data-ttu-id="0e731-175">Pracujeme na tom, abychom i my sami tyto pokyny dodržovali.</span><span class="sxs-lookup"><span data-stu-id="0e731-175">We're working toward following this guidance ourselves.</span></span> <span data-ttu-id="0e731-176">Některé z ukázek jsou staršího data než naše aktuální standardy a zatím se neaktualizovaly.</span><span class="sxs-lookup"><span data-stu-id="0e731-176">Some of the samples predate our current standards ane have not been updated yet.</span></span> <span data-ttu-id="0e731-177">Pracujeme na tom, aby se u všech pracovních, testovaných ukázek zobrazoval jenom aktuální vzorový (ukázkový) kód.</span><span class="sxs-lookup"><span data-stu-id="0e731-177">We are working toward a goal of all running sample code being displayed from working, tested, samples.</span></span>

## <a name="create-samples"></a><span data-ttu-id="0e731-178">Vytváření ukázek</span><span class="sxs-lookup"><span data-stu-id="0e731-178">Create samples</span></span>

<span data-ttu-id="0e731-179">Také můžete vytvářet nové ukázky, které předvádějí koncepce nebo scénáře.</span><span class="sxs-lookup"><span data-stu-id="0e731-179">You can also create new samples that demonstrate concepts or scenarios.</span></span> <span data-ttu-id="0e731-180">Každá ukázka musí být doprovázená článkem, který vysvětluje klíčové informace z ukázky.</span><span class="sxs-lookup"><span data-stu-id="0e731-180">Any samples must be accompanied by a article that explains the key information from the sample.</span></span>

<span data-ttu-id="0e731-181">Pokud vaše nová ukázka doplňuje existující článek, přidejte do tohoto článku odkaz na ukázku.</span><span class="sxs-lookup"><span data-stu-id="0e731-181">If your new sample complements an existing article, add a reference to the sample in that article.</span></span> <span data-ttu-id="0e731-182">Pokud ne, spolupracujte s námi a [napište článek](#create-new-articles), který bude ukázku doprovázet.</span><span class="sxs-lookup"><span data-stu-id="0e731-182">If not, work with us to [write the article](#create-new-articles) that accompanies the sample.</span></span>

<span data-ttu-id="0e731-183">Náš vzorový (ukázkový) kód v každém případě dodržuje zásady kódování používané odpovídajícími produktovými týmy.</span><span class="sxs-lookup"><span data-stu-id="0e731-183">In all cases, our sample code follows the coding conventions used by the related product teams.</span></span> <span data-ttu-id="0e731-184">Jedinou výjimkou je to, že kvůli srozumitelnosti používáme spíše proměnné s explicitně určenými typy než implicitně typované proměnné (deklarované pomocí `var`), když jsou tyto deklarace obsažené v článku.</span><span class="sxs-lookup"><span data-stu-id="0e731-184">One exception is that we are more likely to use explicitly typed varables over implicitly typed (declared with `var`) for clarity when those declarations are included in the article.</span></span>

<span data-ttu-id="0e731-185">Postupujte podle postupu pro ukázky, který je nastíněný v dřívější části popisující [nové články](#create-new-articles), abychom mohli kód revidovat v rané fázi vývojového procesu.</span><span class="sxs-lookup"><span data-stu-id="0e731-185">Follow the sample process outlined in the earlier section for [new articles](#create-new-articles) so that we can review the code early in the development process.</span></span>