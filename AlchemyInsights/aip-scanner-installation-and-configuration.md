---
title: 'ماسح AIP: التثبيت والتكوين'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357289"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="4c2a8-102">ماسح AIP: التثبيت والتكوين</span><span class="sxs-lookup"><span data-stu-id="4c2a8-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="4c2a8-103">**لتثبيت ماسح AIP، اتبع الإرشادات الموصى بها:**</span><span class="sxs-lookup"><span data-stu-id="4c2a8-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="4c2a8-104">إذا كنت تقوم بالترقية ولا تقوم بإجراء تثبيت نظيف، يرجى التأكد من اتباع الإرشادات الخاصة [بترقية ماسح Azure لحماية المعلومات](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) وعميل وضع العلامات الموحد، راجع [ترقية ماسح حماية المعلومات Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="4c2a8-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="4c2a8-105">تحقق من امتثالك لكافة [متطلبات جدران الحماية وإعدادات البنية التحتية للشبكة](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="4c2a8-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="4c2a8-106">تأكد من [تعيين النُهج](https://docs.microsoft.com/azure/information-protection/configure-policy) إلى وضع العلامات التلقائية أو أن يكون لها تسمية افتراضية في النهج.</span><span class="sxs-lookup"><span data-stu-id="4c2a8-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="4c2a8-107">تأكد من تكوين نوع الملف ذي الصلة للتسمية/الحماية كما هو موضح في [أنواع الملفات التي يدعمها عميل حماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="4c2a8-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="4c2a8-108">بالإضافة إلى ذلك، إذا كنت ترغب في تغيير السلوك الافتراضي، اتبع هذه الإرشادات: [تغيير مستوى الحماية الافتراضي للملفات](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="4c2a8-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="4c2a8-109">تحقق من أن حساب المستخدم الذي تم تكوينه لتشغيل خدمة الماسح الضوئي لديه أذونات للوصول إلى كافة المستودعات التي تم تكوينها.</span><span class="sxs-lookup"><span data-stu-id="4c2a8-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="4c2a8-110">إذا كنت لا تزال تواجه مشكلات، يرجى تصدير سجلات الماسح الضوئي وإضافتها إلى تذكرة الدعم الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="4c2a8-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="4c2a8-111">**تصدير سجلات الماسح الضوئي لحماية المعلومات Azure**</span><span class="sxs-lookup"><span data-stu-id="4c2a8-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="4c2a8-112">انتقل إلى %localappdata%\Microsoft\MSIP ضمن سياق المستخدم الذي يقوم بتشغيل خدمة الماسح الضوئي.</span><span class="sxs-lookup"><span data-stu-id="4c2a8-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="4c2a8-113">قم بإلغاء كافة المحتويات تحت مجلد MSIP.</span><span class="sxs-lookup"><span data-stu-id="4c2a8-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="4c2a8-114">احفظ السجلات على اختيارك للموقع، وإرفاقها بطلب الخدمة الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="4c2a8-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="4c2a8-115">يمكنك أيضا استخدام [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="4c2a8-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="4c2a8-116">**لمزيد من المعلومات، راجع:**</span><span class="sxs-lookup"><span data-stu-id="4c2a8-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="4c2a8-117">نشر ماسح حماية المعلومات Azure لتصنيف الملفات وحمايتها تلقائيًا</span><span class="sxs-lookup"><span data-stu-id="4c2a8-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="4c2a8-118">تحديد واستخدام معلمة الرمز المميز لمجموعة-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="4c2a8-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="4c2a8-119">تشغيل دورة اكتشاف وعرض تقارير للماسح الضوئي</span><span class="sxs-lookup"><span data-stu-id="4c2a8-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="4c2a8-120">مراجعة وثائق حماية المعلومات Azure</span><span class="sxs-lookup"><span data-stu-id="4c2a8-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="4c2a8-121">متطلبات حماية المعلومات اللازوردية</span><span class="sxs-lookup"><span data-stu-id="4c2a8-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="4c2a8-122">تحميل عميل حماية المعلومات Azure</span><span class="sxs-lookup"><span data-stu-id="4c2a8-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)