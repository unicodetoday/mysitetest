---
title: Contextual Rendering @ Complex Shaping For Myanmar Unicode
date: 2016-09-27T10:35:25+00:00
layout: post
categories:
  - Useful
---
Windows အတွက် [Uniscribe][1] ဆိုတဲ့ Shaping Engine ရှိတယ်။ ဒါပေမဲ့ သူက မြန်မာစာအတွက် Support လုပ်ပေးမထားဘူး။ ဒါကြောင့် လက်ရှိမြန်မာစာအတွက် သုံးလို့မရရအောင် [Microsoft Volt][2] သုံးပြီး တခြား Opentype Rule တွေနဲ့ Shaping Rule တွေကို အဆင်ပြေသလို တီထွင်ကြံဆပြီး သုံးထားရတာ။ ဂျပန်က နှစ်ထပ်ကားတွေကို မြန်မာပြည်ရောက်တော့ အမိုးဖြတ်၊ တံခါးပေါက် ဘယ်ညာပြောင်းတပ်ပြီး သုံးရတဲ့သဘောပေါ့။ Windows က မြန်မာစာအတွက် Uniscribe မှာ Support ပေးရင် အဲလို Hack စရာမလိုတော့ဘဲ အလွယ်သုံးနိုင်မယ်။ Shaping အတွက်သုံးရတဲ့ CPU usage လည်း သိသိသာသာ လျော့သွားမယ်။ မြန်မာ၂၊ ၃၊ ပုရပိုဒ်၊ ပိတောက်၊ ယွန်းချို၊ မိုင်မြန်မာ နဲ့ ဝင်းယူနီကုဒ်ဖောင့်တွေ Uniscribe သုံးတယ်။

[1]: http://msdn.microsoft.com/en-us/library/dd374091%28v=vs.85%29.aspx
[2]: http://www.microsoft.com/typography/volt.mspx

Windows အတွက် Uniscribe ဆိုတဲ့ Shaping Engine ရှိတယ်။ ဒါပေမဲ့ သူက မြန်မာစာအတွက် Support လုပ်ပေးမထားဘူး။ ဒါကြောင့် လက်ရှိမြန်မာစာအတွက် သုံးလို့မရရအောင် Microsoft Volt သုံးပြီး တခြား Opentype Rule တွေနဲ့ Shaping Rule တွေကို အဆင်ပြေသလို တီထွင်ကြံဆပြီး သုံးထားရတာ။ ဂျပန်က နှစ်ထပ်ကားတွေကို မြန်မာပြည်ရောက်တော့ အမိုးဖြတ်၊ တံခါးပေါက် ဘယ်ညာပြောင်းတပ်ပြီး သုံးရတဲ့သဘောပေါ့။ Windows က မြန်မာစာအတွက် Uniscribe မှာ Support ပေးရင် အဲလို Hack စရာမလိုတော့ဘဲ အလွယ်သုံးနိုင်မယ်။ Shaping အတွက်သုံးရတဲ့ CPU usage လည်း သိသိသာသာ လျော့သွားမယ်။ မြန်မာ၂၊ ၃၊ ပုရပိုဒ်၊ ပိတောက်၊ ယွန်းချို၊ မိုင်မြန်မာ နဲ့ ဝင်းယူနီကုဒ်ဖောင့်တွေ Uniscribe သုံးတယ်။

Uniscribe Font တွေကို လင်းနက်မှာ [Pango][3]က ဘာသာပြန်ပြီး Shaping ပြန်လုပ်တယ်။ ဆိုလိုတာက လင်းနက်မှာ Shaping က Windows မှာထက်တောင် နှေးနိုင်တယ်၊ သူက နှစ်ဆ အလုပ်လုပ်ရတာကိုး။ ဒါပေမဲ့ Pango မှာ Graphite အတွက် အပြည့်အဝ ထောက်ပံ့ပေးထားတယ်။ Padauk ဖောင့်က Uniscribe နဲ့ Graphite နှစ်ခုလုံး Apply လုပ်ထားတဲ့အတွက် Pango က [Graphite][4] ကို ဦးစားပေးပြီး Shaping လုပ်တဲ့အတွက် Padauk သုံးရတာ ပိုပေါ့ပြီး မြန်တယ်။ Masterpiece Uni Sans ကတော့ Pango ကို တိုက်ရိုက်သုံးတဲ့အတွက် အပေါ့ဆုံးနဲ့ အမြန်ဆုံး ဖြစ်မယ်။ Linux မှာ တိုင်းရင်းသားစာတွေ ဖတ်ဖို့လိုရင် Padauk ကိုသုံးပြီး၊ မလိုရင် Masterpiece Uni Sans ကိုသုံးဖို့ Recommend လုပ်ပါတယ်။ MyMyanmar လည်း Graphite သုံးတယ်ထင်တယ်။ Pango က Graphite ကို Support လုပ်ပေမဲ့ Shaping rule တွေက ဖောင့်ထဲမှာပဲ ရှိတယ်။ Masterpiece သွင်းလိုက်လို့ ပိတောက် အလုပ်မလုပ်ဘူးဆိုတာ မဖြစ်နိုင်ဘူးထင်တယ်။ သေချာစမ်းကြည့်ရဦးမယ်။

[3]: http://www.pango.org/
[4]: http://scripts.sil.org/cms/scripts/page.php?site_id=nrsi&cat_id=RenderingGraphite

သံလွင်ဖောင့်ကတော့ 1mb လောက်ရှိတဲ့အတွက် ဖောင့်ဆိုဒ်အကြီးဆုံးဖြစ်မယ်။ Opentype နဲ့ Graphite ရဲ့ [Ligature][5] ပြောင်းတဲ့ Rule တစ်ခုပဲသုံးထားလို့ CPU Usage အနည်းဆုံးဖောင့် ဖြစ်မယ်။ Windows မှာရော Linux ရဲ့ [Harfbuzz][6] နဲ့ Pango Module တွေမှာပါ အလုပ်လုပ်တယ်။ Windows က Adobe Software တွေမှာ အသုံးပြုလို့ရတဲ့ တစ်ခုတည်းသော ဖောင့် ဖြစ်မယ်။ Adobe က အခြေခံ Opentype Rule တွေကို နားလည်ပေမဲ့ Complex Shaping မှာ Uniscribe နဲ့ အလုပ်မလုပ်ဘူး။  Adobe က သူ့ကိုယ်ပိုင် အင်ဂျင်နဲ့ အလုပ်လုပ်တယ်။ [AFDKO][8] နဲ့ ရေးထားတဲ့ ဖောင့်တွေမှ အပြည့်အဝ Support လုပ်တယ်။ VOLT ထဲမှာ Standard [Opentype][7] Rules တွေသာသုံးပြီးရေးထားရင်လည်း Adobe ဆော့ဝဲတွေမှာ အလုပ်လုပ်တယ်။

[5]: http://typographic%20ligature/
[6]: http://www.freedesktop.org/wiki/Software/HarfBuzz
[7]: http://en.wikipedia.org/wiki/OpenType
[8]: http://www.adobe.com/devnet/opentype/afdko.html

Mac ရဲ့ Native က [AAT][9] ၊ သူက Graphite နဲ့ အလုပ်လုပ်ပုံချင်းတူတယ်။ Masterpiece Uni Sans က အရှေ့တောင်အာရှ ဘာသာစကားတွေမှာ ကိုယ့်အားကိုယ်ကိုး Develop လုပ်ပြီး ပထမဆုံး AAT သုံးနိုင်တဲ့ Opensource Mac Font ဖြစ်မယ်။ သူ့ရှေ့မှာ စီးပွားဖြစ်ဖောင့်တွေဖြစ်တဲ့ Xenotype နဲ့ MyMyanmar နှစ်ခုရှိတယ်။ တိုတိုပြောရရင် မြန်မာစာကို Linux ကလွဲပြီး ဘယ် OS ကမှ Support မလုပ်ပေးသော်ငြား အပတ်တကုပ်နဲ့ အားထုတ်ခဲ့တဲ့ ပညာရှင်တွေကြောင့် မြန်မာယူနီကုဒ်ဖောင့်တွေ ဒီလောက်ထိ အဆင့် မြင့်မြင့် သုံးနေနိုင်တာလို့ ပြောရမယ်။

[9]: http://developer.apple.com/fonts/TTRefMan/RM06/Chap6AATIntro.html

ဒီဖောင့်က မပေါ်ဘူးဆိုရင် ဘယ်နေရာမှာ ဘယ်လိုမပေါ်တာ၊ အလုပ်မလုပ်ဘူးဆိုရင် ဘယ် OS ရဲ့ ဘယ် Software မှာ အလုပ်မလုပ်တာ၊ ဘယ်လို ဘယ်လိုရိုက်လိုက်လို့ မမှန်တာ ဘယ်နေရာမှာ မမှန်တာ စသည်ဖြင့် အသေးစိတ် Bug Report တွေကို Screenshot နဲ့တကွ အကြောင်းကြားပေးရင် Font Developer တွေ Troubleshoot လုပ်ရတာ ပိုအဆင်ပြေမှာ ဖြစ်ပါတယ်။ ကျေးဇူးတင်ပါတယ်။

View Unicode font list [here.](http://www.myanmarlanguage.org/unicode/myanmar-fonts-which-follow-unicode-rules)

Download Myanmar unique syllable list [here.](http://goo.gl/rntUC)

Myanmar unique syllable list ဖိုင်ထဲမှာ ပါတဲ့ ဝဏ္ဏ၊ ဝဏ္ဏတွဲ အကုန်လုံးနဲ့ အမှန်အတိုင်းမြင်ရတယ်ဆိုရင် အဲဒီဖောင့် ၁၀၀ ရာခိုင်နှုန်း အလုပ်လုပ်တယ်လို့ အကြမ်းဖျင်း ပြောလို့ ရပါတယ်။

Credit: myanmarlanguage.org