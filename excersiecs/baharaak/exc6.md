# مراحل الگوریتم find-s
1- گام اول الگوریتم مقدار دهی اولیه h با خاص ترین فرضیه است

 
برای مثال میخواهیم در نظر بگیریم در چه روزهایی فرد دوست دارد پیاده روی کند. شش ویژگی در نظر میگیریم که این ویژگی ها شامل time, weather, temperature,company,humidity,wind هستند.


مرحله اول الگوریتم : مقدار دهی اولیه h0

h0=<0,0,0,0,0,0>

مرحله دوم : به سراغ اولین داده جدول میرویم چون فرضیه h0 تمامی مقادیر منفی را درنظر میگیرد با توجه به نمونه ها که نمونه اول نمونه مثبتی است مقادیر h0 با مقادیر کلی تری جایگزین می شود :

x1<morning, sunny, warm, yes, mild, strong> + 

h1<morning, sunny, warm, yes, mild, strong>

مرحله دوم الگوریتم: برای نمونه اموزشی دوم چون نمونه منفی میباشد و پیش فرض الگوریتم روی نمونه های منفی است بنابراین فرضیه h2 با فرضیه h1 برابر میشود

x2<evening, rainy, cold, no, mild, normal>-

h2=h1<morning, sunny, warm, yes, mild, strong>

مرحله سوم : نمونه اموزشی سوم را به الگوریتم میدهیم چون نمونه مثبت است الگوریتم مجبور میشود تا h2 را کلی تر کند بنابراین نمونه سوم ، پنجم و ششم به دلیل اینکه الگوریتم دو نمونه باینری را دیده است از علامت ؟ استفاده میکنیم.

x3<morning, sunny, moderate, yes, normal, normal>+

h3=<morning, sunny, ?, yes, ?, ?>

مرحله چهارم : برای کامل کردن الگوریتم find-s چهارمین داده را نیز بررسی میکنیم چون داده چهارم داده مثبتی است داریم:

x4<evening, sunny, cold, yes, high, strong>+    
h4=<?, sunny, ?, yes, ?, ?>

این الگوریتم چون نمونه های منفی را هم ساپوت میکند پس با تمامی نمونه های ما سازگار است.