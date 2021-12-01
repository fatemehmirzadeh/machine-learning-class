<div dir="rtl">
  **9)با توجه به داده های زیر این جدول را با کمک الگوریتم find-s حل کنید.**
  </div>
  
| Example | Color  | Toughness | Fungus | Appearance | Poisonous |
|---------|--------|-----------|--------|------------|-----------|
| 1       | Green  | Soft      | no     | Wrinkled   | yes       |
| 2       | Green  | Soft      | yes    | Smooth     | no        |
| 3       | Brown  | Hard      | no     | Smooth     | yes       |
| 4       | Green  | Soft      | yes    | Smooth     | no        |
| 5       | Orange | Soft      | yes    | Wrinkled   | yes       |

<div dir="rtl">
در این الگوریتم فرضیه h0 را به عنوان فرضیه اولیه در نظر می گیریم و با توجه به داده های آموزشی مثبت آن را تغییر می دهیم.
<br/>
h0 = (0,0,0,0)
<br/>
حال سطر اول داده یعنی مثال اول را بررسی می کنیم و چون اولین سطر مثبت است  همان را در فرضیه h1 می نویسیم    
<br/>
h1 = (Green,Soft,N0,Wrinkled)
<br/>
سطر دوم (مثال دوم) بر روی فرضیه بی تاثیر است چون جواب no است پس h2 برابر با h1 خواهد بود
<br/>
h2 = (Green,Soft,N0,Wrinkled)
<br/>
در مثال سوم  لیبل مثبت است پس باعث تغییر در فرضیه می شود و هر جا که ویژگی متفاوت با فرضیه قبل است باید علامت سوال قرار دهیم،پس خواهیم داشت:
<br/>
h3 = (?,?,No,?)
<br/>
در مثال چهارم لیبل منفی است پس فرضیه بدون تغییر  باقی می ماند یعنی h4 برابر با h3 است
<br/>
h4 = (?,?,No,?)
<br/>
در فرضیه آن ها که علامت سوال هستند تغییری نمیکنند، سراغ مثال 5 می رویم و ویژگی FUNGUS  yes است پس باید علامت سوال شود.
<br/>
h5 = (?,?,?,?)
<br/>
این فرضیه همه ی مثال ها را مثبت جواب می دهد در عمل یعنی هیچ هوشمندی ای ایجاد نشده است که به این مفهوم خواهد بود که تعداد ویژگی ها برای حل مساله کافی نیست
<br/>
و این فرضیه ی خاص ما مناسب نیست. 