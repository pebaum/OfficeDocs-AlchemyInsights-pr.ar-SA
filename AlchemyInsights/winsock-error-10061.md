---
title: خطأ Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: f44ed42906b85e63f1f694813f54710906969904
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30772429"
---
# <a name="winsock-error-10061"></a>خطأ Winsock 10061

رمز الخطأ هذا يعني أن Office 365 تعذر إنشاء مأخذ توصيل TCP (اتصال) مع المضيف الهدف. السبب المحتمل لهذا الخطأ مشكلة في تكوين جدار الحماية الخاص بك. لحل هذه المشكلة، تحقق من هذه الإعدادات:
  
- تحقق من تكوين جدار الحماية الخاص بك باستخدام المعلومات الموجودة في [Office 365 URLs ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)
    
- إذا كان الخطأ خاص إلى Exchange عبر إنترنت الحماية (البرنامج)، قد يجب أن تم مسبقاً إعلامك لتغيير [عناوين IP في حماية Exchange عبر إنترنت](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).
    
- تأكد من أن موفر خدمة إنترنت (ISP) لا يقوم بحظر المنفذ.
    
- تحقق من إعدادات الخادم المضيف والهدف الذكية في الموصلات.
    
لاحظ أن Office 365 لا منع الاتصالات *الواردة* على هذا النحو. 
  
