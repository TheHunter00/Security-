
## Objectives
- 1.1 - Compare and contrast various security controls
- 1.2 - Summarize fundamental security concepts

## Fundamentals of Security
- **Information Security**:
  
 يعني حماية البيانات والمعلومات من الوصول أو التعديل أو الكشف أو التدمير بدون إذن.
- **Information Systems Security**:
  
يعني حماية الأنظمة زي الكمبيوترات والسيرفرات وأجهزة الشبكة اللي بتخزن وتتعامل مع البيانات المهمة.

## CIA Triad
- **Confidentiality**:

 يعني التأكد إن المعلومات تكون بس للمصرح لهم بدخولها، زي استخدام **encryption** (تشفير).
- **Integrity**:

 يعني التأكد إن البيانات تظل صحيحة وغير متغيرة إلا من قبل أشخاص مصرح لهم، زي استخدام **checksums** (رموز التحقق).
- **Availability**:

 يعني التأكد إن المعلومات والموارد تكون متاحة وقت الحاجة، زي استخدام **redundancy** (تكرار المكونات).

## Non-repudiation
- يعني التأكد إن أي عمل أو حدث مش ممكن ينكروا الأشخاص اللي كانوا جزء منه، زي استخدام **digital signatures** (التوقيعات الرقمية).

## CIANA Pentagon
- إضافة للـ CIA Triad مع **non-repudiation** و**authentication**.

## Triple A’s of Security
- **Authentication**:


يعني التأكد من هوية الأشخاص أو الأنظمة، زي استخدام **passwords** (كلمات المرور).
- **Authorization**:

يعني تحديد الصلاحيات للأشخاص الموثقين، زي **permissions** (الأذونات).
- **Accounting**:

 يعني تتبع نشاطات المستخدمين واستخدام الموارد، زي **audit logs** (سجلات التدقيق).

## Security Control Categories
- **Technical**: تشمل التكنولوجيا والبرامج.
- **Managerial**: تتعلق بالتخطيط والإدارة.
- **Operational**: تشمل الإجراءات اليومية.
- **Physical**: إجراءات مادية لحماية الأصول.

## Security Control Types
- **Preventive**: إجراءات لمنع حدوث مشاكل أمنية.
- **Deterrent**: إجراءات لردع المهاجمين.
- **Detective**: إجراءات لرصد الأنشطة المشبوهة.
- **Corrective**: إجراءات لتصحيح الأضرار.
- **Compensating**: بدائل للتدابير غير الفعالة.
- **Directive**: إجراءات لتحديد السياسات والمعايير.

## Zero Trust Model
- **Zero Trust**:

 مبدأ إنك ما تفترضش الثقة في أي حد أو جهاز، وكل حاجة لازم تتأكد منها.
  - **Control Plane**:

 إدارة السياسات والتحقق من الهوية.
  - **Data Plane**:

 تنفيذ السياسات، تقليل نطاق التهديدات، وإدارة المناطق المؤمنة.

---

## Threats and Vulnerabilities

- **Threat**:

 أي حاجة ممكن تسبب ضرر أو خسارة للأنظمة التقنية، زي الكوارث الطبيعية أو الهجمات الإلكترونية.
- **Vulnerability**:

 أي ضعف في تصميم أو تنفيذ النظام، زي الأخطاء البرمجية أو إعدادات غير صحيحة.
 لو فيه تهديد لكن مفيش ثغرة، مفيش خطر. ولو فيه ثغرة لكن مفيش تهديد، برضو مفيش خطر.

- **Risk Management**:

 طرق لتقليل احتمال حدوث المخاطر وتحقيق النتائج المطلوبة.

## Confidentiality

- **Confidentiality**:

 حماية المعلومات من الوصول أو الكشف بدون إذن.
 
  - **طرق الحماية**:
    - **Encryption**: تشفير البيانات.
    - **Access Controls**: تحديد من يقدر يدخل على البيانات.
    - **Data Masking**: إخفاء أجزاء من البيانات لحمايتها.
    - **Physical Security**: حماية المستندات والبيانات الرقمية.
    - **Training and Awareness**: تعليم الموظفين كيفية حماية البيانات.

## Integrity

- **Integrity**:

 التأكد إن البيانات تظل صحيحة وغير متغيرة إلا لو تم التعديل عليها بطرق معتمدة.
  - **طرق الحماية**:
    - **Hashing**: تحويل البيانات لقيمة ثابتة للتحقق منها.
    - **Digital Signatures**: تأكيد السلامة والأصالة.
    - **Checksums**: للتحقق من سلامة البيانات أثناء النقل.
    - **Access Controls**: لتقليل التعديلات غير المصرح بها.
    - **Regular Audits**: لمراجعة التعديلات والتأكد من سلامة البيانات.

## Availability

- **Availability**: التأكد إن المعلومات والأنظمة متاحة وقت الحاجة.
  - **Redundancy**: تكرار المكونات لتحسين الاعتمادية.
    - **أنواع**:
      - **Server Redundancy**: استخدام سيرفرات متعددة لتحمل الأحمال.
      - **Data Redundancy**: تخزين البيانات في أماكن متعددة.
      - **Network Redundancy**: توفير مسارات شبكة بديلة.
      - **Power Redundancy**: استخدام مصادر طاقة احتياطية.

## Non-repudiation

- **Non-repudiation**: التأكد من أن أي عمل رقمي لا يمكن إنكاره.
  - **Digital Signatures**: توقيع رقمي يضمن عدم إنكار العمل.

## Authentication

- **Authentication**: التأكد من هوية الأشخاص أو الأنظمة.
  - **Methods**:
    - **Knowledge Factor**: شيء يعرفه المستخدم.
    - **Possession Factor**: شيء مادي زي التوكن.
    - **Inherence Factor**: سمات فريدة للمستخدم.
    - **Action Factor**: إجراء فريد يقوم به المستخدم.
    - **Location Factor**: موقع جغرافي للمستخدم.

  - **Multi-Factor Authentication (MFA)**: يتطلب عدة طرق للتحقق.

## Authorization

- **Authorization**: تحديد ما يمكن للمستخدمين الموثقين الوصول إليه أو القيام به.
  - **Importance**: حماية البيانات الحساسة والحفاظ على سلامة النظام.

## Accounting

- **Accounting**: تتبع وتسجيل نشاطات المستخدمين واستخدام الموارد.
  - **Technologies**:
    - **Syslog Servers**: تجميع السجلات من الأنظمة المختلفة.
    - **Network Analysis Tools**: تحليل حركة الشبكة.
    - **SIEM Systems**: تحليل أمني في الوقت الفعلي.

## Security Control Categories

- **Technical Controls**: تشمل التكنولوجيا والبرامج.
- **Managerial Controls**: تتعلق بالتخطيط والإدارة.
- **Operational Controls**: تشمل الإجراءات اليومية.
- **Physical Controls**: إجراءات مادية لحماية الأصول.

## Security Control Types

- **Preventive Controls**: لمنع الحوادث الأمنية.
- **Deterrent Controls**: لردع المهاجمين.
- **Detective Controls**: لرصد الأنشطة المشبوهة.
- **Corrective Controls**: لتصحيح الأضرار.
- **Compensating Controls**: بدائل للتدابير غير الفعالة.
- **Directive Controls**: لتحديد السياسات والمعايير.

## Gap Analysis

- **Gap Analysis**:

 تقييم الفرق بين الأداء الحالي والمطلوب.
  - **Types**:
    - **Technical Gap Analysis**:
 
 تقييم البنية التحتية التقنية.
    - **Business Gap Analysis**:

 تقييم العمليات التجارية.
  - **Plan of Action and Milestones (POA&M)**:
 
 تحديد الإجراءات اللازمة لمعالجة الثغرات وتوزيع الموارد وتحديد الجداول الزمنية.

## Zero Trust

- **Zero Trust**:

 يتطلب التحقق من كل جهاز ومستخدم ومعاملة داخل الشبكة بدون افتراض الثقة.
- **Control Plane**:
 
  إدارة السياسات والتحقق من الهوية.
- **Data Plane**:

  تنفيذ السياسات، تقليل نطاق التهديدات، وإدارة المناطق المؤمنة.
