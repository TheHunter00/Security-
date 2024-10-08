# Network Security Guide

## 1. Secure Network Design

تصميم الشبكة الآمن يعني تخطيط وبناء الشبكة بطريقة تحميها من التهديدات والمشاكل.
- **Planning:** تحديد الأهداف الأمنية للشبكة وإنشاء خطة للبنية التحتية.
- **Network Segmentation:** تقسيم الشبكة إلى أقسام صغيرة (مثل VLANs) لتقليل المخاطر وتحسين الأمان.
- **Security Tools:** استخدام أدوات مثل الجدران النارية (Firewalls) وأجهزة الكشف عن التسلل (IDS) لتعزيز الأمان.

## 2. Weakness

نقاط الضعف هي الأماكن التي يمكن للمهاجمين استغلالها لتهديد الشبكة.
- **Vulnerability Scanning:** فحص الشبكة والأنظمة لتحديد الثغرات المحتملة باستخدام أدوات متخصصة.
- **Vulnerability Assessment:** تحليل تأثير نقاط الضعف على النظام وتقدير المخاطر.
- **Mitigation:** تصحيح الثغرات من خلال تحديث الأنظمة وتعزيز الأمان بطرق مختلفة.

## 3. Network Appliances

### Switch

السويتش هو جهاز يربط بين عدة أجهزة ضمن نفس الشبكة المحلية (LAN).
- **Connecting Devices:** يربط بين أجهزة الكمبيوتر والطابعات في الشبكة.
- **Data Forwarding:** يوجه البيانات مباشرة إلى الجهاز المستهدف باستخدام عنوان MAC.
- **Data Link Layer:** يعمل على مستوى Data Link Layer ويتعامل مع عناوين MAC.
- **Performance Improvement:** يقلل من التصادمات ويزيد من كفاءة نقل البيانات.
- **VLAN Configuration:** يمكن تقسيم الشبكة إلى شبكات افتراضية لتحسين الأمان والأداء.

### Access Point

نقطة الوصول هي جهاز يوفر اتصالاً لاسلكياً بشبكة LAN.
- **Wireless Connectivity:** يسمح للأجهزة بالاتصال بالشبكة بدون كابلات.
- **Network Extension:** يوسع نطاق الشبكة اللاسلكية في المناطق التي يصعب الوصول إليها بالكابلات.
- **Protocol Support:** يدعم بروتوكولات Wi-Fi مثل 802.11b/g/n/ac/ax.
- **Device Management:** يمكنه التعامل مع عدد كبير من الأجهزة المتصلة في وقت واحد.
- **Security:** يوفر خيارات لتأمين الشبكة اللاسلكية مثل WPA2/WPA3.

### Router

الراوتر هو جهاز يربط بين شبكتين مختلفتين، مثل الشبكة الداخلية (LAN) والإنترنت (WAN).
- **Data Routing:** يوجه البيانات بين الشبكات ويحدد أفضل مسار لنقل البيانات.
- **NAT:** يترجم عناوين IP الخاصة بالشبكة الداخلية إلى عنوان IP عام للوصول إلى الإنترنت.
- **Traffic Management:** يحسن أداء الشبكة بتوزيع حركة المرور بفعالية.
- **Network Layer:** يعمل على مستوى Network Layer ويتعامل مع عناوين IP.
- **Network Configuration:** يمكن تكوينه لإعدادات مثل جدار الحماية (Firewall) وإعدادات VPN.
- **Dynamic Routing:** يستخدم بروتوكولات مثل OSPF وBGP لتحديد أفضل مسار للبيانات.

### Firewall

الجدار الناري هو جهاز أو برنامج لحماية الشبكة من التهديدات عن طريق تصفية البيانات.
- **Data Filtering:** يراقب البيانات الواردة والصادرة ويمنع الوصول غير المصرح به.
- **Policy Enforcement:** يحدد أنواع البيانات المسموح بها أو المحظورة بناءً على السياسات الأمنية.
- **Threat Detection:** يحتوي على أدوات لكشف ومنع الهجمات مثل DoS وDDoS.
- **Deployment:** يمكن أن يكون مادي أو برنامج يتم تشغيله على خادم.
- **Custom Rules:** يمكن تكوين قواعد تفصيلية للتحكم في حركة المرور.
- **Reporting:** يوفر تقارير عن الأنشطة المشبوهة وحركة المرور.

### Load Balancer

موازن التحميل هو جهاز أو برنامج يوزع الأحمال بين عدة سيرفرات لتحسين الأداء ومنع التحميل الزائد على سيرفر واحد.
- **Load Distribution:** يوزع الطلبات بين سيرفرات متعددة لضمان استجابة سريعة وكفاءة عالية.
- **High Availability:** يوفر تكراراً وتوافر عالياً للتطبيقات لتفادي الأعطال.
- **Performance Improvement:** يقلل من زمن الاستجابة ويزيد من قدرة معالجة الطلبات.
- **Load Balancing Strategies:** يستخدم استراتيجيات مثل Round Robin، Least Connections، أو IP Hash لتوزيع الأحمال.
- **Health Monitoring:** يراقب حالة السيرفرات ويتأكد من عملها بشكل صحيح قبل توجيه الطلبات إليها.
- **Smart Balancing:** يمكن تكوينه للتعامل مع أنواع مختلفة من البيانات والتطبيقات.

## 4. ACL (Access Control List)

قائمة التحكم في الوصول هي مجموعة من القواعد التي تتحكم في من يمكنه الوصول إلى موارد الشبكة ومتى.
- **Rule Creation:** تحديد من يحق له الوصول إلى الموارد مثل الملفات والطابعات.
- **Rule Implementation:** تنفيذ هذه القواعد على الأجهزة مثل السويتشات والجدران النارية.
- **Flexible Rules:** يمكن تكوين قواعد لتلبية متطلبات أمان محددة.
- **Access Control:** تحكم في الوصول إلى الموارد بناءً على نوع المستخدم، عنوان IP، أو وقت الوصول.
- **Ease of Management:** تُدار عادةً من خلال أدوات الشبكة أو إعدادات الجدار الناري.

## 5. Server

السيرفر هو جهاز حاسوب يوفر خدمات وموارد للأجهزة الأخرى عبر الشبكة.
- **Data Storage:** يخزن البيانات والتطبيقات التي يحتاجها المستخدمون أو التطبيقات الأخرى.
- **Application Hosting:** يدير تشغيل التطبيقات والخدمات مثل مواقع الويب، قواعد البيانات، والبريد الإلكتروني.
- **Resource Management:** يوفر الوصول إلى الموارد المشتركة مثل الطابعات وأجهزة التخزين.
- **Customization:** يمكن تخصيص السيرفرات لتلبية احتياجات محددة مثل سيرفر ويب أو سيرفر قواعد بيانات.
- **Reliability:** يُصمم السيرفرات لتكون موثوقة وتوفر توافرًا عالياً.
- **Security:** يمكن تطبيق سياسات أمان على السيرفرات لحمايتها من الوصول غير المصرح به.

## 6. DoS (Denial of Service)

هجوم إنكار الخدمة هو محاولة لجعل خدمة معينة غير متاحة عن طريق إغراقها بالطلبات.
- **Flooding:** زيادة حجم الطلبات على السيرفر أو الشبكة حتى تصبح غير قادرة على الاستجابة.
- **Impact:** يمكن أن يؤدي إلى توقف الخدمة وتسبب خسائر كبيرة.
- **Ease of Execution:** يمكن أن تكون الهجمات بسيطة ولكن فعالة.

## 7. DDoS (Distributed Denial of Service)

هجوم إنكار الخدمة الموزع هو نوع متقدم من هجوم DoS حيث يأتي الهجوم من عدة مصادر.
- **Distributed Flooding:** يستخدم شبكة من الأجهزة (مثل البوت نت) لإغراق الهدف بالطلبات.
- **Difficulty of Defense:** الهجوم من مصادر متعددة يجعل من الصعب على الدفاعات التصدي له.
- **Devastating Impact:** يزيد من حجم الهجوم ويجعله أكثر صعوبة في التصدي.
- **Identity Concealment:** يصعب تتبع مصدر الهجوم بسبب تعدد الأجهزة المستخدمة.

## 8. OSI (Open Systems Interconnection)

نموذج OSI هو نموذج يوضح كيفية انتقال البيانات عبر الشبكة من خلال 7 طبقات.
1. **Physical Layer:** تتعامل مع الكابلات والأجهزة المادية مثل الأسلاك والمحولات.
2. **Data Link Layer:** مسؤولة عن نقل البيانات بين جهازين على نفس الشبكة من خلال عناوين MAC.
3. **Network Layer:** تتعامل مع توجيه البيانات بين الشبكات المختلفة باستخدام عناوين IP.
4. **Transport Layer:** تضمن وصول البيانات بشكل صحيح وكامل من خلال بروتوكولات مثل TCP وUDP.
5. **Session Layer:** تدير جلسات الاتصال بين التطبيقات.
6. **Presentation Layer:** تتعامل مع تنسيق البيانات وتشفيرها لضمان تقديمها بشكل صحيح للتطبيقات.
7. **Application Layer:** تتعامل مع التطبيقات والخدمات المباشرة مثل البريد الإلكتروني والمتصفحات.

## 9. Active Directory

**Active Directory** هو نظام من مايكروسوفت لإدارة الشبكات، حيث يُستخدم لتنظيم وإدارة الموارد مثل المستخدمين والأجهزة والسياسات عبر الشبكة.
- **Domains:** النطاق هو وحدة تنظيم أساسية في Active Directory، حيث يمثل مجموعة من الأجهزة والمستخدمين ضمن قاعدة بيانات واحدة، ويساعد في إدارة الموارد وتطبيق السياسات الأمنية بشكل مركزي على النطاقات المختلفة.
- **Trees:** الأشجار هي مجموعة من النطاقات المرتبطة بشكل هرمي، حيث تشارك النطاقات في نفس مساحة أسماء DNS، مما يوفر تنظيمًا هرمياً للنطاقات ويسهل إدارة الموارد عبر نطاقات متعددة.
- **Forests:** الغابات هي مجموعة من الأشجار التي تشارك في قاعدة بيانات Active Directory، وتدير الأمان والتكوين عبر الأشجار المختلفة وتتيح التكامل بين النطاقات المختلفة.
- **Organizational Units (OUs):** الوحدات التنظيمية هي تقسيمات داخل النطاقات تُستخدم لتنظيم وإدارة المستخدمين والأجهزة، مما يوفر هيكلًا منطقيًا لتطبيق السياسات وإدارة الموارد بشكل فعال، ويسهم في تسهيل إدارة الأذونات والتكوينات.
- **Groups:** المجموعات هي مجموعات من المستخدمين تُستخدم لتبسيط إدارة الأذونات، وتنقسم إلى أنواع مثل المجموعات المحلية التي تقتصر على النطاق المحلي، والمجموعات العالمية التي تحتوي على مستخدمين من نطاقات مختلفة ضمن نفس الغابة، والمجموعات الشاملة التي تحتوي على مستخدمين من أي نطاق في الغابة.
- **Group Policies:** السياسات الجماعية تُستخدم لتطبيق إعدادات الأمان والتكوينات على مجموعة من المستخدمين أو الأجهزة بشكل مركزي.
- **Authentication and Authorization:** يضمن Active Directory عملية المصادقة (التحقق من الهوية) والتفويض (تحديد الصلاحيات) بشكل آمن للمستخدمين والأجهزة للوصول إلى الموارد.
- **Replication:** عملية تكرار البيانات بين وحدات Active Directory المختلفة لضمان تحديث المعلومات بشكل مستمر وتوفير توافر عالٍ.

