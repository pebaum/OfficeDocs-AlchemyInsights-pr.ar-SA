---
title: التقاعد من أدوات eDiscovery القديمة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: c4632b52dde579b7d5b2e6e15f1583300a0bd136
ms.sourcegitcommit: a7c17217c170ead24571421baaf5a14f1525b1a6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/20/2020
ms.locfileid: "42157492"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="2dc19-102">التقاعد من أدوات eDiscovery القديمة</span><span class="sxs-lookup"><span data-stu-id="2dc19-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="2dc19-103">نتيجة لوظائف eDiscovery الجديدة والمحسنة في مركز الامتثال Microsoft 365، سيتم سحب أدوات eDiscovery القديمة التالية والأوامر في الأشهر المقبلة:</span><span class="sxs-lookup"><span data-stu-id="2dc19-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="2dc19-104">[في مكان eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) وفي [مكان يحمل](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) في مركز إدارة Exchange.</span><span class="sxs-lookup"><span data-stu-id="2dc19-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="2dc19-105">Cmdlets PowerShell Exchange عبر الإنترنت التي تدعم eDiscovery في المكان ويحمل في المكان.</span><span class="sxs-lookup"><span data-stu-id="2dc19-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="2dc19-106">(يتم تعريف هذه cmdlets بشكل جماعي كـ \*-MailboxSearch cmdlets.) وهذا يشمل cmdlets التالية:</span><span class="sxs-lookup"><span data-stu-id="2dc19-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="2dc19-107">بحث جديد في علب ة البريد</span><span class="sxs-lookup"><span data-stu-id="2dc19-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="2dc19-108">بدء البحث في علبة البريد</span><span class="sxs-lookup"><span data-stu-id="2dc19-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="2dc19-109">إيقاف علبة البريد البحث</span><span class="sxs-lookup"><span data-stu-id="2dc19-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="2dc19-110">تعيين علبة البريد البحث</span><span class="sxs-lookup"><span data-stu-id="2dc19-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="2dc19-111">[cmdlet البحث علبة البريد](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) في PowerShell تبادل عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="2dc19-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="2dc19-112">العمليات التالية في API خدمات ويب Exchange:</span><span class="sxs-lookup"><span data-stu-id="2dc19-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="2dc19-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="2dc19-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="2dc19-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="2dc19-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="2dc19-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="2dc19-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="2dc19-116">Office 365 eDiscovery متقدم v1.0</span><span class="sxs-lookup"><span data-stu-id="2dc19-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="2dc19-117">**الجدول الزمني للتقاعد:**</span><span class="sxs-lookup"><span data-stu-id="2dc19-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="2dc19-118">1 أبريل 2020: لن تتمكن من إنشاء عمليات بحث والاحتفاظ جديدة، ولكن لا يزال بإمكانك تشغيل عمليات البحث الحالية وتعديلها وحذفها على مسؤوليتك الخاصة.</span><span class="sxs-lookup"><span data-stu-id="2dc19-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="2dc19-119">لن يدعم دعم Microsoft بعد الآن & في EـDiscovery في EAC.</span><span class="sxs-lookup"><span data-stu-id="2dc19-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="2dc19-120">1 يوليو 2020: سيتم وضع وظيفة eDiscovery & في EWHATفي EDISCOVERy في EAC في وضع القراءة فقط.</span><span class="sxs-lookup"><span data-stu-id="2dc19-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="2dc19-121">وهذا يعني أنك ستتمكن فقط من إزالة عمليات البحث وقائمة.</span><span class="sxs-lookup"><span data-stu-id="2dc19-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="2dc19-122">**لمزيد من المعلومات، راجع:**</span><span class="sxs-lookup"><span data-stu-id="2dc19-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="2dc19-123">ترحيل عمليات البحث عن eDiscovery القديمة وإمكانية حملها إلى مركز الامتثال Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="2dc19-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="2dc19-124">التقاعد من أدوات eDiscovery القديمة</span><span class="sxs-lookup"><span data-stu-id="2dc19-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="2dc19-125">الأسئلة الشائعة حول eDiscovery في المكان ويحمل في مكان</span><span class="sxs-lookup"><span data-stu-id="2dc19-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/en-us/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)


