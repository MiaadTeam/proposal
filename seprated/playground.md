 
به سه دلیل به سمت طراحی محیطی برای آزمایش ورودی و خروجی‌های درخواست‌های ارسالی به
آدرس /funql (آدرس هدف بستر توسعه فانکیوال رفتیم).

## سهولت توسعه (هم برای بک‌اند - هم برای فرونت‌اند)

در هنگام توسعه بارها نیاز به تست خروجی کد نوشته شده پیدا می‌کنیم و اگر بتوانیم یک
رابط کاربری زیبا با ux و dx خوب برای تست خروجی کد، طراحی کنیم در زمان و هزینه
توسعه‌ي بک‌اند کار صرفه جویی قابل توجه‌ای ایجاد کرده‌ایم.

از طرفی کدنویسی هم که می‌خواهد در سمت مشتری خروجی‌ها را به نرم‌افزار متصل کند نیاز
مکرر به آزمایش داده‌های سرور دارد و با این رابط کار او بسیار ساده‌تر خواهد بود.

## داکیومنت شدن ورودی و خروجی‌های کدنویسی شده

وقتی همه‌ی درخواست‌ها قرار است به یک آدرس ارسال شود، اگر آن آدرس توضیحات لازم برای
ارسال درخواست ارائه نکند پیچیدگی بسیاری در فهم پروژه، بین اعضای توسعه دهنده
ایجاد خواهد شد.

بستر توسعه فان‌کیوال علاوه بر ارسال پیغام‌های کاربردی خطا در خروجی‌های به خاطر
validation-first بودن کدهای نوشته شده، به صورت کامل و گرافیکی در playground برای
تک تک درخواست‌ها و هر کدام از فیلد‌های هر درخواست توضیحات کاملی ارائه می‌کند.

در نهایت به همراه داکیومنتی که برای هر درخواست در playground وجود دارد به خاطر
type-safty طبیعی و وابسته به پلتفرم موجود در این بستر، تمامی تکه کدهای نوشته شده
دارای توضیحات بروز و قابل فهم در این رابط کاربری هستند

## واحد تست E2E گرافیکی

به واسطه تعریف استانداردهای صحیح و قابل فهم برای انسان و ماشین در بستر توسعه
funql توانایی ایجاد یک رابط گرافیکی برای تست‌های نهایی و قبل از خروجی گرفتن از
نرم‌افزارهای نوشته شده با آن فراهم بود. به همین خاطر ما با طراحی یک گراف از
خروجی‌های هر پروژه بر اساس اسنادی که funql cli به صورت خودکار تهیه میکند و نوشتن
کانفیک‌های فایل‌های مختصر، قابلیت تست تمامی خروجی‌های با تمامی شرایط ممکن در هر
پروژه با یک دکمه در playground به صورت گرافیکی را بوجود آوردیم.

