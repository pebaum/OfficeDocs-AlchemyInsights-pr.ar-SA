---
title: الردهة التفافيه
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2673"
- "9000740"
ms.openlocfilehash: 311af365a94b788182bb6870bca3f67b2ad802d0
ms.sourcegitcommit: 932981641dd8e973e28dfe346bbdf9c923111b13
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/27/2019
ms.locfileid: "40889069"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>ضبط إعدادات اللوبي ومستوي المشاركة في الفرق

إذا كنت ترغب في السماح للجميع ، بما في ذلك المستخدمين الهاتفيين والخارجيين والمجهولين ، **بتجاوز اللوبي**، فاستخدم PowerShell لإنجاز هذه المهمة. في ما يلي مثال علي تعديل نهج الاجتماعات العمومية للمؤسسة الخاصة بك.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

يتطلب هذا cmdlet حاليا استخدام سكايب للوحدة النمطية PowerShell الاعمال. للحصول علي اعداد لاستخدام هذا cmdlet ، تحقق من [أداره السياسات عبر PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

بمجرد اعداد سياسة ، تحتاج إلى تطبيقها علي المستخدمين. أو ، إذا قمت بتعديل النهج العمومي ، سيتم تطبيقه تلقائيا علي المستخدمين. بالنسبة لأي تغيير في السياسة ، تحتاج إلى الانتظار لمده **4 ساعات علي الأقل حتى 24 ساعة حتى** تسري السياسات. 

تاكد من مراجعه الوثائق أدناه قبل اجراء هذه التغييرات لفهم ما يسمح به هذا بالبالضبط.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>فهم فرق التحكم في نهج اللوبي

تتحكم هذه الإعدادات في الاجتماعات التي ينتظرها المشاركون في الردهة قبل قبولهم في الاجتماع ومستوي المشاركة المسموح بها في الاجتماع. يمكنك استخدام PowerShell لتحديث إعدادات نهج الاجتماع التي لم يتم تنفيذها بعد (المسمي "قريبا") في مركز أداره الفرق. انظر أدناه للحصول علي مثال cmdlet PowerShell التي تسمح لجميع المستخدمين لتجاوز الردهة.

- [القبول التلقائي للأشخاص](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) هو نهج لكل منظم يتحكم في ما إذا كان الأشخاص ينضمون إلى الاجتماع مباشره أو ينتظرون في الردهة حتى يتم قبولهم من قبل مستخدم مصادق عليه.

- [السماح للأشخاص المجهولين ببدء اجتماع](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) هو نهج لكل منظم يتحكم في ما إذا كان بإمكان الأشخاص المجهولين ، بما في ذلك المستخدمين B2B والمتحدين ، الانضمام إلى اجتماع المستخدم بدون مستخدم مصادق عليه من المؤسسة في الحضور.

- [السماح لمستخدمي الطلب الهاتفي بتجاوز الردهة](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**قريبا**) هو نهج لكل منظم يتحكم في ما إذا كان الأشخاص الذين يقومون بالاتصال بالهاتف بالانضمام إلى الاجتماع مباشره أو الانتظار في الردهة بغض النظر عن السماح **للأشخاص** بالاعداد تلقائيا.

- [السماح للمنظمين بتجاوز إعدادات اللوبي](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**قريبا**) هو نهج لكل منظم يتحكم في ما إذا كان منظم الاجتماع يمكنه تجاوز إعدادات الردهة التي يقوم المسؤول بتعيينها **تلقائيا** **والسماح لمستخدمي الطلب الهاتفي بتجاوز الردهة** عندما يقومون بجدوله اجتماع جديد.

**ملاحظه:** قراءه [أداره نهج الاجتماع في الفرق](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) للحصول علي نظره عامه كامله حول نهج اجتماع فرق Microsoft.
