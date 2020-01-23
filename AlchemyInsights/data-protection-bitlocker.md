---
title: DataProtection-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908697"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>تمكين تشفير Bitlocker باستخدام اينتوني

 يمكن استخدام نهج حماية نقطه النهاية اينتوني لتكوين إعدادات تشفير Bitlocker لأجهزه Windows. لمزيد من المعلومات ، راجع [إعدادات Windows 10 (والإصدارات الأحدث) لحماية الاجهزه باستخدام اينتوني](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).
 
يجب ان تدرك ان العديد من الاجهزه الأحدث التي تعمل بنظام التشغيل Windows 10 تدعم تشفير Bitlocker التلقائي ، والذي يتم تشغيله بدون تطبيق نهج MDM. قد يؤثر هذا علي تطبيق النهج إذا تم تكوين الإعدادات غير الافتراضية. راجع الاسئله الشائعة التالية لمزيد من التفاصيل.
 
للحصول علي معلومات حول استكشاف مشكلات bitlocker وإصلاحها ، راجع [استكشاف أخطاء نهج bitlocker وإصلاحها في Microsoft اينتوني](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).
 
 
**الأسئلة المتداولة**

 س: اي إصدارات من Windows دعم تشفير الجهاز باستخدام "نهج حماية نقطه النهاية" ؟<br>
 A: يتم تطبيق الإعدادات في نهج حماية نقطه النهاية اينتوني باستخدام [CSP Bitlocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp). لا تدعم كافة الإصدارات أو البنيات من Windows CSP Bitlocker. <br><br>
      في هذا الوقت ، يتم اعتماد إصدارات Windows التالية: المؤسسة ، التعليم ، الجوال ، المؤسسات المتنقلة ، والمهنية (بناء 1809 والإصدارات الأحدث).
 
س: إذا كان الجهاز مشفرا بالفعل مع Bitlocker باستخدام الإعدادات الافتراضية لنظام التشغيل لأسلوب التشفير وقوه التشفير (اكستس-AES-128) ، فان تطبيق نهج بإعدادات مختلفه يؤدي تلقائيا إلى أعاده تشفير محرك الاقراص مع الإعدادات الجديدة ؟<br>
A: لا. لتطبيق إعدادات التشفير الجديدة ، يجب أولا فك تشفير محرك الاقراص.<br><br>
**ملاحظه:** بالنسبة للاجهزه التي يتم تسجيلها مع الطيار الألى ، لا يتم تشغيل التشفير التلقائي الذي قد يحدث اثناء OOBE حتى يتم تقييم نهج اينتوني ، والذي يسمح باستخدام الإعدادات المستندة إلى النهج بدلا من افتراضيات نظام التشغيل.
 
س: إذا تم تشفير جهاز كنتيجة لتطبيق نهج اينتوني ، سيتم فك تشفير عند أزاله هذا النهج ؟<br>
A: أزاله النهج المتعلقة بالتشفير لا ينتج عن فك تشفير محركات الاقراص التي تم تكوينها.
 
س: لماذا تظهر "سياسة التوافق اينتوني" ان جهازي لم يتم تمكين Bitlocker ، حتى ولو كان ؟<br>
A: يستخدم الاعداد "تمكين Bitlocker" في نهج التوافق اينتوني عميل مصادقه صحة جهاز Windows (DHA). يقيس هذا العميل فقط حاله الجهاز في وقت التمهيد. لذلك إذا لم يتم أعاده تمهيد الجهاز منذ اكتمال تشفير Bitlocker ، لن تقوم خدمه العميل DHA بالإبلاغ عن Bitlocker علي انه نشط.
 
 