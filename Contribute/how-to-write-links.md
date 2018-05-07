---
title: Používání odkazů v dokumentaci
description: Tento článek obsahuje pokyny k vytváření odkazů na obsah na webu docs.microsoft.com.
author: bryanla
ms.author: bryanla
manager: mbaldwin
ms.date: 06/29/2017
ms.prod: non-product-specific
ms.topic: contributor-guide
ms.custom: external-contributor-guide
ms.openlocfilehash: 1699e57ac6a4dc4c5a1ef099ea183b3cbc6307cd
ms.sourcegitcommit: de6e6b6ca641fdd5b30eb46deee9ac3a500089ef
ms.translationtype: HT
ms.contentlocale: cs-CZ
ms.lasthandoff: 04/26/2018
---
# <a name="using-links-in-documentation"></a><span data-ttu-id="31cf0-103">Používání odkazů v dokumentaci</span><span class="sxs-lookup"><span data-stu-id="31cf0-103">Using links in documentation</span></span>
<span data-ttu-id="31cf0-104">Tento článek popisuje způsob používání hypertextových odkazů ze stránek hostovaných na webu docs.microsoft.com. Odkazy se snadno přidávají do markdownu pomocí několika různých konvencí.</span><span class="sxs-lookup"><span data-stu-id="31cf0-104">This article describes how to use hyperlinks from pages hosted at docs.microsoft.com. Links are easy to add into markdown with a few varying conventions.</span></span> <span data-ttu-id="31cf0-105">Odkazy přesměrovávají uživatele na obsah na stejné stránce, na jiné sousední stránky nebo na externí weby a adresy URL.</span><span class="sxs-lookup"><span data-stu-id="31cf0-105">Links point users to content in the same page, point off into other neighboring pages, or point to external sites and URLs.</span></span>

<span data-ttu-id="31cf0-106">Back-end webu docs.microsoft.com používá systém OPS (Open Publishing Services), který implementuje DFM (DocFX Flavored Markdown).</span><span class="sxs-lookup"><span data-stu-id="31cf0-106">The docs.microsoft.com site backend uses Open Publishing Services (OPS) which implements DocFX Flavored Markdown (DFM).</span></span> <span data-ttu-id="31cf0-107">DFM je vysoce kompatibilní s GFM (GitHub Flavored Markdown) a přidává další funkce prostřednictvím rozšíření Markdownu.</span><span class="sxs-lookup"><span data-stu-id="31cf0-107">DFM is highly compatible with GitHub Flavored Markdown (GFM), and DFM adds additional functionality through Markdown extensions.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="31cf0-108">Všechny odkazy musí být zabezpečené (`https` versus `http`), když to cíl podporuje (což by měla drtivá většina).</span><span class="sxs-lookup"><span data-stu-id="31cf0-108">All links must be secure (`https` vs `http`) whenever the target supports it (which the vast majority should).</span></span>

## <a name="link-text"></a><span data-ttu-id="31cf0-109">Text odkazu</span><span class="sxs-lookup"><span data-stu-id="31cf0-109">Link text</span></span>

<span data-ttu-id="31cf0-110">Slova, která použijete v textu odkazu, by měla být popisná.</span><span class="sxs-lookup"><span data-stu-id="31cf0-110">The words that you include in link text should be friendly.</span></span> <span data-ttu-id="31cf0-111">Jinými slovy by mělo jít o normální slova nebo název stránky, na kterou odkazujete.</span><span class="sxs-lookup"><span data-stu-id="31cf0-111">In other words, they should be normal English words or the title of the page that you're linking to.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="31cf0-112">Nepoužívejte „klikněte sem“.</span><span class="sxs-lookup"><span data-stu-id="31cf0-112">Do not use "click here."</span></span> <span data-ttu-id="31cf0-113">Není to dobré pro SEO a nepopisuje to dostatečně cíl odkazu.</span><span class="sxs-lookup"><span data-stu-id="31cf0-113">It's bad for SEO and doesn't adequately describe the target.</span></span>

<span data-ttu-id="31cf0-114">**Správně:**</span><span class="sxs-lookup"><span data-stu-id="31cf0-114">**Correct:**</span></span>

- `For more information, see the [contributor guide index](https://github.com/Azure/azure-content/blob/master/contributor-guide/contributor-guide-index.md).`

- `For more details, see the [SET TRANSACTION ISOLATION LEVEL](https://msdn.microsoft.com/library/ms173763.aspx) reference.`

<span data-ttu-id="31cf0-115">**Nesprávně:**</span><span class="sxs-lookup"><span data-stu-id="31cf0-115">**Incorrect:**</span></span>

- `For more details, see [https://msdn.microsoft.com/library/ms173763.aspx](https://msdn.microsoft.com/library/ms173763.aspx).`

- `For more information, click [here](https://github.com/Azure/azure-content/blob/master/contributor-guide/contributor-guide-index.md).`

## <a name="links-from-one-article-to-another"></a><span data-ttu-id="31cf0-116">Odkazy z jednoho článku na druhý</span><span class="sxs-lookup"><span data-stu-id="31cf0-116">Links from one article to another</span></span>

<span data-ttu-id="31cf0-117">Pokud chcete vytvořit hotlink z technického článku na webu Docs na jiný technický článek webu Docs v rámci stejné sady docset, použijte následující syntax pro odkazy:</span><span class="sxs-lookup"><span data-stu-id="31cf0-117">To create an inline link from a Docs technical article to another Docs technical article within the same docset, use the following link syntax:</span></span>

- <span data-ttu-id="31cf0-118">Článek v adresáři odkazuje na jiný článek ve stejném adresáři:</span><span class="sxs-lookup"><span data-stu-id="31cf0-118">An article in a directory links to another article in the same directory:</span></span>

  `[link text](article-name.md)`

- <span data-ttu-id="31cf0-119">Článek z podadresáře odkazuje na článek v kořenovém adresáři:</span><span class="sxs-lookup"><span data-stu-id="31cf0-119">An article links from a subdirectory to an article in the root directory:</span></span>

  `[link text](../article-name.md)`

- <span data-ttu-id="31cf0-120">Článek v kořenovém adresáři odkazuje na článek v podadresáři:</span><span class="sxs-lookup"><span data-stu-id="31cf0-120">An article in the root directory links to an article in a subdirectory:</span></span>

  `[link text](./directory/article-name.md)`

- <span data-ttu-id="31cf0-121">Článek v podadresáři odkazuje na článek v jiném podadresáři:</span><span class="sxs-lookup"><span data-stu-id="31cf0-121">An article in a subdirectory links to an article in another subdirectory:</span></span>

  `[link text](../directory/article-name.md)`

- <span data-ttu-id="31cf0-122">Článek odkazující na různé sady docset (i ve stejném úložišti): `[link text](./directory/article-name)`</span><span class="sxs-lookup"><span data-stu-id="31cf0-122">An article linking across docsets (even if in the same repository): `[link text](./directory/article-name)`</span></span>
  
## <a name="links-to-anchors"></a><span data-ttu-id="31cf0-123">Odkazy na ukotvení</span><span class="sxs-lookup"><span data-stu-id="31cf0-123">Links to anchors</span></span>

<span data-ttu-id="31cf0-124">Ukotvení vytvářet nemusíte.</span><span class="sxs-lookup"><span data-stu-id="31cf0-124">You do not have to create anchors.</span></span> <span data-ttu-id="31cf0-125">Generují se automaticky pro všechny nadpisy H2 při publikování.</span><span class="sxs-lookup"><span data-stu-id="31cf0-125">They're automatically generated at publishing time for all H2 headings.</span></span> <span data-ttu-id="31cf0-126">Jediné, co musíte udělat, je vytvořit odkazy na oddíly H2.</span><span class="sxs-lookup"><span data-stu-id="31cf0-126">The only thing you have to do is create links to the H2 sections.</span></span>

- <span data-ttu-id="31cf0-127">Vytvoření odkazu na nadpis ve stejném článku:</span><span class="sxs-lookup"><span data-stu-id="31cf0-127">To link to a heading within the same article:</span></span>

  `[link](#the-text-of-the-H2-section-separated-by-hyphens)`
  `[Create cache](#create-cache)`

- <span data-ttu-id="31cf0-128">Vytvoření odkazu na ukotvení z jiného článku ve stejném podadresáři:</span><span class="sxs-lookup"><span data-stu-id="31cf0-128">To link to an anchor in another article in the same subdirectory:</span></span>

  `[link text](article-name.md#anchor-name)`
  `[Configure your profile](media-services-create-account.md#configure-your-profile)`

- <span data-ttu-id="31cf0-129">Vytvoření odkazu na ukotvení v jiném podadresáři služby:</span><span class="sxs-lookup"><span data-stu-id="31cf0-129">To link to an anchor in another service subdirectory:</span></span>

  `[link text](../directory/article-name.md#anchor-name)`
  `[Configure your profile](../directory/media-services-create-account.md#configure-your-profile)`

## <a name="links-from-includes"></a><span data-ttu-id="31cf0-130">Odkazy z vložených souborů</span><span class="sxs-lookup"><span data-stu-id="31cf0-130">Links from includes</span></span>

<span data-ttu-id="31cf0-131">Jelikož jsou vložené soubory umístěné v jiném adresáři, musíte použít delší relativní cesty.</span><span class="sxs-lookup"><span data-stu-id="31cf0-131">Because include files are located in another directory, you must use longer relative paths.</span></span> <span data-ttu-id="31cf0-132">Pokud chcete vytvořit odkaz na článek z vloženého souboru, použijte tento formát:</span><span class="sxs-lookup"><span data-stu-id="31cf0-132">To link to an article from an include file, use this format:</span></span>

    [link text](../articles/folder/article-name.md)

## <a name="links-in-selectors"></a><span data-ttu-id="31cf0-133">Odkazy v selektorech</span><span class="sxs-lookup"><span data-stu-id="31cf0-133">Links in selectors</span></span>

<span data-ttu-id="31cf0-134">Pokud máte selektory, které jsou vložené do vloženého souboru, jak to má tým dokumentace Azure, použijte následující strukturu odkazu:</span><span class="sxs-lookup"><span data-stu-id="31cf0-134">If you have selectors that are embedded in an include--as does the Azure documentation team--use the following link structure:</span></span>

    > <span data-ttu-id="31cf0-135">[AZURE.SELECTOR-LIST (Dropdown1 | Dropdown2 )]</span><span class="sxs-lookup"><span data-stu-id="31cf0-135">[AZURE.SELECTOR-LIST (Dropdown1 | Dropdown2 )]</span></span>
    - [<span data-ttu-id="31cf0-136">(Text1 | Example1 )</span><span class="sxs-lookup"><span data-stu-id="31cf0-136">(Text1 | Example1 )</span></span>](../articles/folder/article-name1.md)
    - [<span data-ttu-id="31cf0-137">(Text1 | Example2 )</span><span class="sxs-lookup"><span data-stu-id="31cf0-137">(Text1 | Example2 )</span></span>](../articles/folder/article-name2.md)
    - [<span data-ttu-id="31cf0-138">(Text2 | Example3 )</span><span class="sxs-lookup"><span data-stu-id="31cf0-138">(Text2 | Example3 )</span></span>](../articles/folder/article-name3.md)
    - <span data-ttu-id="31cf0-139">[(Text2 | Example4 )](../articles/folder/article-name4.md) --></span><span class="sxs-lookup"><span data-stu-id="31cf0-139">[(Text2 | Example4 )](../articles/folder/article-name4.md) --></span></span>

## <a name="reference-style-links"></a><span data-ttu-id="31cf0-140">Odkazy z referencí</span><span class="sxs-lookup"><span data-stu-id="31cf0-140">Reference-style links</span></span>

<span data-ttu-id="31cf0-141">Pokud chcete, aby byl váš zdrojový obsah lépe čitelný, můžete použít odkazy z referencí.</span><span class="sxs-lookup"><span data-stu-id="31cf0-141">You can use reference-style links to make your source content easier to read.</span></span> <span data-ttu-id="31cf0-142">Odkazy z referencí nahradí syntax hotlinku jednodušší syntaxí, která vám umožní přesunout dlouhé adresy URL na konec článku.</span><span class="sxs-lookup"><span data-stu-id="31cf0-142">Reference-style links replace inline link syntax with simplified syntax that allows you to move the long URLs to the end of the article.</span></span> <span data-ttu-id="31cf0-143">Zde je příklad z webu [Daring Fireball](https://daringfireball.net/projects/markdown/):</span><span class="sxs-lookup"><span data-stu-id="31cf0-143">Here's [Daring Fireball](https://daringfireball.net/projects/markdown/) 's example:</span></span>

<span data-ttu-id="31cf0-144">Vložený text:</span><span class="sxs-lookup"><span data-stu-id="31cf0-144">Inline text:</span></span>

    I get 10 times more traffic from [Google][1] than from [Yahoo][2] or [MSN][3].

<span data-ttu-id="31cf0-145">Odkazy referencí na konci článku:</span><span class="sxs-lookup"><span data-stu-id="31cf0-145">Link references at the end of the article:</span></span>

    <!--Reference links in article-->
    [1]: http://google.com/
    [2]: http://search.yahoo.com/
    [3]: http://search.msn.com/

<span data-ttu-id="31cf0-146">Nezapomeňte mezi dvojtečkou a odkazem vytvořit mezeru.</span><span class="sxs-lookup"><span data-stu-id="31cf0-146">Make sure that you include the space after the colon, before the link.</span></span> <span data-ttu-id="31cf0-147">Pokud odkazujete na ostatní technické články a zapomenete mezeru vytvořit, odkaz nebude v publikovaném článku fungovat.</span><span class="sxs-lookup"><span data-stu-id="31cf0-147">When you link to other technical articles, if you forget to include the space, the link will be broken in the published article.</span></span>

## <a name="links-to-pages-that-are-not-part-of-the-technical-documentation-set"></a><span data-ttu-id="31cf0-148">Odkazování na stránky, které nejsou součástí sady technické dokumentace</span><span class="sxs-lookup"><span data-stu-id="31cf0-148">Links to pages that are not part of the technical documentation set</span></span>

<span data-ttu-id="31cf0-149">Pokud chcete vytvořit odkaz na jiný web ve vlastnictví Microsoftu (jako je stránka s ceníkem, stránka SLA nebo cokoli jiného, co není článek dokumentace), použijte absolutní adresu URL, ale vynechejte národní prostředí.</span><span class="sxs-lookup"><span data-stu-id="31cf0-149">To link to a page on another Microsoft property (such as a pricing page, SLA page, or anything else that is not a documentation article), use an absolute URL, but omit the locale.</span></span> <span data-ttu-id="31cf0-150">Cílem je, aby odkazy fungovaly v GitHubu a na zobrazené stránce:</span><span class="sxs-lookup"><span data-stu-id="31cf0-150">The goal here is that links work in GitHub and on the rendered site:</span></span>

    [link text](https://azure.microsoft.com/pricing/details/virtual-machines/)

## <a name="links-to-third-party-sites"></a><span data-ttu-id="31cf0-151">Odkazy na weby třetích stran</span><span class="sxs-lookup"><span data-stu-id="31cf0-151">Links to third-party sites</span></span>

<span data-ttu-id="31cf0-152">Nejlepší uživatelské prostředí minimalizuje odchod uživatelů na jiný web.</span><span class="sxs-lookup"><span data-stu-id="31cf0-152">The best user experience minimizes sending users to another site.</span></span> <span data-ttu-id="31cf0-153">Odkazy na weby třetích stran, které jsou občas potřeba, proto vytvářejte na základě těchto informací:</span><span class="sxs-lookup"><span data-stu-id="31cf0-153">So base any links to third-party sites, which we do sometimes need, on this info:</span></span>

- <span data-ttu-id="31cf0-154">**Odpovědnost:** Na obsah třetích stran odkazujte, když jde o informace, které má sdílet třetí strana.</span><span class="sxs-lookup"><span data-stu-id="31cf0-154">**Accountability**: Link to third-party content when it's the third-party's information to share.</span></span> <span data-ttu-id="31cf0-155">Úkolem Microsoftu například není říkat lidem, jak používat vývojářské nástroje pro Android – to má udělat Google.</span><span class="sxs-lookup"><span data-stu-id="31cf0-155">For example, it's not Microsoft's place to tell people how to use Android developer tools--that is Google's story to tell.</span></span> <span data-ttu-id="31cf0-156">Pokud je to potřeba, můžeme vysvětlit, jak vývojářské nástroje pro Android používat *se* službou Azure, ale jak tyto nástroje celkově používat by měl vysvětlit Google.</span><span class="sxs-lookup"><span data-stu-id="31cf0-156">If we need to, we can explain how to use Android developer tools *with* Azure, but Google should tell the story of how to use their tools.</span></span>
- <span data-ttu-id="31cf0-157">**Schválení od PM**: Požádejte Microsoft o schválení obsahu třetí strany.</span><span class="sxs-lookup"><span data-stu-id="31cf0-157">**PM signoff**: Request that Microsoft sign off on third-party content.</span></span> <span data-ttu-id="31cf0-158">Odkazování na takový obsah znamená, že mu důvěřujeme, a zahrnuje odpovědnost, pokud se lidé těmito pokyny budou řídit.</span><span class="sxs-lookup"><span data-stu-id="31cf0-158">By linking to it, we are saying something about our trust in it and our obligation if people follow the instructions.</span></span>
- <span data-ttu-id="31cf0-159">**Ověření čerstvosti:** Ověřte, že informace třetí strany jsou stále aktuální, správné a relevantní a že se odkaz nezměnil.</span><span class="sxs-lookup"><span data-stu-id="31cf0-159">**Freshness reviews**: Make sure that the third-party info is still current, correct, and relevant, and that the link hasn’t changed.</span></span>
- <span data-ttu-id="31cf0-160">**Přesměrování ven:** Informujte uživatele, že budou přesměrováni na jiný web.</span><span class="sxs-lookup"><span data-stu-id="31cf0-160">**Offsite**: Make users aware that they are going to another site.</span></span> <span data-ttu-id="31cf0-161">Pokud to není jasné z kontextu, přidejte vysvětlení.</span><span class="sxs-lookup"><span data-stu-id="31cf0-161">If the context does not make that clear, add a qualifying phrase.</span></span> <span data-ttu-id="31cf0-162">Například: „Požadavky zahrnují vývojářské nástroje pro Android, které si můžete stáhnout z webu Android Studio“.</span><span class="sxs-lookup"><span data-stu-id="31cf0-162">For example: “Prerequisites include the Android Developer Tools, which you can download on the Android Studio site.”</span></span>
- <span data-ttu-id="31cf0-163">**Další kroky:** V sekci Další kroky můžete přidat odkaz například na blog MVP.</span><span class="sxs-lookup"><span data-stu-id="31cf0-163">**Next steps**: It’s fine to add a link to, say, an MVP blog in a "Next steps" section.</span></span> <span data-ttu-id="31cf0-164">Jen uživatele znovu nezapomeňte informovat, že budou přesměrováni na jiný web.</span><span class="sxs-lookup"><span data-stu-id="31cf0-164">Again, just make sure that users understand they’ll be leaving the site.</span></span>
- <span data-ttu-id="31cf0-165">**Právní náležitosti:** Jsme právně krytí částí **Odkazy na weby třetích stran** v **Podmínkách použití** uvedených v zápatí každé stránky ms.com.</span><span class="sxs-lookup"><span data-stu-id="31cf0-165">**Legal**: We are covered legally under **Links to Third Party Sites** in the **Terms of Use** footer on every ms.com page.</span></span>

## <a name="links-to-msdn-or-technet"></a><span data-ttu-id="31cf0-166">Odkazy na MSDN nebo TechNet</span><span class="sxs-lookup"><span data-stu-id="31cf0-166">Links to MSDN or TechNet</span></span>

<span data-ttu-id="31cf0-167">Když budete potřebovat odkázat na MSDN nebo Technet, použijte celý odkaz na téma a odeberte z odkazu jazyk národního prostředí „en-us“.</span><span class="sxs-lookup"><span data-stu-id="31cf0-167">When you need to link to MSDN or TechNet, use the full link to the topic, and remove the "en-us" language locale from the link.</span></span>

## <a name="links-to-azure-powershell-reference-content"></a><span data-ttu-id="31cf0-168">Odkazy na referenční obsah Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="31cf0-168">Links to Azure PowerShell reference content</span></span>

<span data-ttu-id="31cf0-169">Referenční obsah Azure PowerShell prošel od listopadu 2016 několika změnami.</span><span class="sxs-lookup"><span data-stu-id="31cf0-169">The Azure PowerShell reference content has been through several changes since November 2016.</span></span> <span data-ttu-id="31cf0-170">Pro odkazování na tento obsah z jiných článků na webu docs.microsoft.com použijte následující pokyny.</span><span class="sxs-lookup"><span data-stu-id="31cf0-170">Use the following guidelines for linking to this content from other articles on docs.microsoft.com.</span></span>

<span data-ttu-id="31cf0-171">Struktura adresy URL:</span><span class="sxs-lookup"><span data-stu-id="31cf0-171">Structure of the URL:</span></span>

* <span data-ttu-id="31cf0-172">Pro rutiny:</span><span class="sxs-lookup"><span data-stu-id="31cf0-172">For cmdlets:</span></span>
  - `/powershell/module/<module-name>/<cmdlet-name>[?view=<moniker-name>]`
* <span data-ttu-id="31cf0-173">Pro koncepční témata:</span><span class="sxs-lookup"><span data-stu-id="31cf0-173">For conceptual topics:</span></span>
  - `/powershell/azure/<topic-file-name>[?view=<moniker-name>]`
  - `/powershell/azure/<service-name>/<topic-file-name>[?view=<moniker-name>]`

<span data-ttu-id="31cf0-174">Část &lt;moniker-name&gt; je volitelná.</span><span class="sxs-lookup"><span data-stu-id="31cf0-174">The &lt;moniker-name&gt; portion is optional.</span></span> <span data-ttu-id="31cf0-175">Pokud ji vynecháte, budete přesměrováni na nejnovější verzi obsahu.</span><span class="sxs-lookup"><span data-stu-id="31cf0-175">If it's omitted, you will be directed to the latest version of the content.</span></span> <span data-ttu-id="31cf0-176">Část &lt;service-name&gt; je jedním z příkladů uvedených v následujících základních adresách URL:</span><span class="sxs-lookup"><span data-stu-id="31cf0-176">The &lt;service-name&gt; portion is one of the examples shown in the following base URLs:</span></span>

- <span data-ttu-id="31cf0-177">Obsah Azure PowerShell (AzureRM): https://docs.microsoft.com/powershell/azure/</span><span class="sxs-lookup"><span data-stu-id="31cf0-177">Azure PowerShell (AzureRM) content: https://docs.microsoft.com/powershell/azure/</span></span>
- <span data-ttu-id="31cf0-178">Obsah Azure PowerShell (ASM): https://docs.microsoft.com/powershell/azure/_servicemanagement_</span><span class="sxs-lookup"><span data-stu-id="31cf0-178">Azure PowerShell (ASM) content: https://docs.microsoft.com/powershell/azure/_servicemanagement_</span></span>
- <span data-ttu-id="31cf0-179">Obsah Azure Active Directory (AzureAD) PowerShell: https://docs.microsoft.com/powershell/azure/_active-directory_</span><span class="sxs-lookup"><span data-stu-id="31cf0-179">Azure Active Directory (AzureAD) PowerShell content: https://docs.microsoft.com/powershell/azure/_active-directory_</span></span>
- <span data-ttu-id="31cf0-180">Azure Service Fabric PowerShell: https://docs.microsoft.com/powershell/azure/_service-fabric_</span><span class="sxs-lookup"><span data-stu-id="31cf0-180">Azure Service Fabric PowerShell: https://docs.microsoft.com/powershell/azure/_service-fabric_</span></span>
- <span data-ttu-id="31cf0-181">Azure Information Protection PowerShell: https://docs.microsoft.com/powershell/azure/_aip_</span><span class="sxs-lookup"><span data-stu-id="31cf0-181">Azure Information Protection PowerShell: https://docs.microsoft.com/powershell/azure/_aip_</span></span>
- <span data-ttu-id="31cf0-182">Azure Elastic DB Jobs PowerShell: https://docs.microsoft.com/powershell/azure/_elasticdbjobs_</span><span class="sxs-lookup"><span data-stu-id="31cf0-182">Azure Elastic DB Jobs PowerShell: https://docs.microsoft.com/powershell/azure/_elasticdbjobs_</span></span>

<span data-ttu-id="31cf0-183">Když tyto adresy URL použijete, budete přesměrováni na nejnovější verzi obsahu.</span><span class="sxs-lookup"><span data-stu-id="31cf0-183">When you use these URLs, you will be redirected to the latest version of the content.</span></span> <span data-ttu-id="31cf0-184">Tímto způsobem nemusíte určovat verzi parametru moniker.</span><span class="sxs-lookup"><span data-stu-id="31cf0-184">This way, you don't have to specify a version moniker.</span></span> <span data-ttu-id="31cf0-185">Nebudete tak mít odkazy na koncepční obsah, které se musí při změně verze aktualizovat.</span><span class="sxs-lookup"><span data-stu-id="31cf0-185">And you won't have links to conceptual content that must be updated when the version changes.</span></span>

<span data-ttu-id="31cf0-186">Pokud chcete vytvořit odkaz, najděte ve svém prohlížeči stránku, na kterou chcete odkázat, a zkopírujte její adresu URL.</span><span class="sxs-lookup"><span data-stu-id="31cf0-186">To create the correct link, find the page that you want to link to in your browser, and copy the URL.</span></span>
<span data-ttu-id="31cf0-187">Potom odeberte https://docs.microsoft.com a informace o národním prostředí.</span><span class="sxs-lookup"><span data-stu-id="31cf0-187">Then, remove "https://docs.microsoft.com" and the locale info.</span></span>

<span data-ttu-id="31cf0-188">Když odkazujete z obsahu stránky, musíte použít celou adresu URL bez informace o národním prostředí.</span><span class="sxs-lookup"><span data-stu-id="31cf0-188">When you're linking from a TOC, you must use the full URL without the locale information.</span></span>

<span data-ttu-id="31cf0-189">Příklad Markdownu:</span><span class="sxs-lookup"><span data-stu-id="31cf0-189">Example markdown:</span></span>

```markdown
[Get-AzureRmResourceGroup](/powershell/module/azurerm.resources/get-azurermresourcegroup)
[Get-AzureRmResourceGroup](/powershell/module/azurerm.resources/get-azurermresourcegroup?view=azurermps-4.1.0)
[New-AzureVM](/powershell/module/azure/new-azurevm?view=azuresmps-4.0.0)
[New-AzureRmVM](/powershell/module/azurerm.compute/new-azurermvm)
[Install Azure PowerShell for Service Management](/powershell/azure/servicemanagement/install-azurerm-ps)
[Install Azure PowerShell](/powershell/azure/install-azurerm-ps)
```