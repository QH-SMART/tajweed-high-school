<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <script src="https://cdn.tailwindcss.com"></script>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Noto+Naskh+Arabic:wght@700&family=Vazirmatn:wght@700&display=swap');
        body {
            font-family: 'Noto Naskh Arabic', sans-serif;
            background-color: #1E3A8A; /* Dark Blue */
            color: #F8F5F0;
        }
        h1 {
            font-family: 'Vazirmatn', sans-serif;
        }
    </style>
</head>
<body class="min-h-screen flex flex-col items-center relative">
    <div class="dark-overlay absolute inset-0 bg-black opacity-50 z-0"></div>
    
    <div class="header text-center text-gold relative w-full p-4 bg-opacity-10 bg-white rounded-lg shadow-lg mt-5">
        <div class="absolute top-4 right-4 cursor-pointer" onclick="toggleMenu()">
            <i class="fas fa-bars text-2xl" style="color: #C9A66B;"></i>
        </div>
    </div>

    <div class="container mx-auto text-center relative z-10 mt-8">
        <h1 class="text-xl font-bold mb-4" style="color: #C9A66B;">خوش آمدید به لیسه عالی خصوصی تجوید</h1>
        <p class="mb-4">به لیسه عالی خصوصی تجوید خوش آمدید! اینجا جایی است که دانش‌آموزان با استعداد و پرانگیزه می‌توانند به بهترین نحو ممکن رشد کنند و به اهداف خود دست یابند.</p>
        <h2 class="text-xl font-bold mb-2">ویژگی‌های ما:</h2>
        <ul class="list-disc list-inside mb-4">
            <li><strong>آموزش با کیفیت:</strong> ما به ارائه آموزش‌های با کیفیت و متناسب با نیازهای دانش‌آموزان متعهد هستیم.</li>
            <li><strong>محیط حمایتی:</strong> در فضایی دوستانه و حمایتی، به یادگیری و پیشرفت شما کمک خواهیم کرد.</li>
            <li><strong>فعالیت‌های فوق برنامه:</strong> با شرکت در فعالیت‌های فرهنگی و ورزشی، توانمندی‌های خود را گسترش دهید.</li>
        </ul>
        <p class="mb-8">ما به شما اطمینان می‌دهیم که در لیسه عالی خصوصی تجوید، بهترین تجربه آموزشی را خواهید داشت.</p>
        <p class="font-bold">به جمع ما خوش آمدید و با هم به سوی موفقیت حرکت کنیم!</p>
    </div>

    <div class="container mx-auto grid grid-cols-1 gap-8 text-center relative z-10 mt-8">
        <div class="flex flex-col items-center p-6 mx-auto cursor-pointer" onclick="showModal('schoolModal')">
            <i class="fas fa-globe text-5xl" style="color: #C9A66B;"></i> <!-- Gold Color -->
            <p class="mt-4 text-lg">مکتب ما</p>
        </div>
        <div class="flex flex-col items-center p-6 mx-auto cursor-pointer" onclick="showModal('teacherModal')">
            <i class="fas fa-chalkboard-teacher text-5xl" style="color: #C9A66B;"></i> <!-- Gold Color -->
            <p class="mt-4 text-lg">استادان ما</p>
        </div>
        <div class="flex flex-col items-center p-6 mx-auto cursor-pointer" onclick="showModal('studentModal')">
            <i class="fas fa-user-graduate text-5xl" style="color: #C9A66B;"></i> <!-- Gold Color -->
            <p class="mt-4 text-lg">شاگردان ما</p>
        </div>
        <div class="flex flex-col items-center p-6 mx-auto cursor-pointer" onclick="showModal('messageModal')">
            <i class="fas fa-envelope text-5xl" style="color: #C9A66B;"></i> <!-- Gold Color -->
            <p class="mt-4 text-lg">پیام مدیریت</p>
        </div>
    </div>

    <!-- Modals -->
    <div id="schoolModal" class="modal fixed inset-0 bg-opacity-10 bg-white backdrop-blur-lg p-8 shadow-lg z-20 overflow-y-auto hidden text-right">
        <div class="close-btn absolute top-5 left-5 bg-opacity-10 bg-white border border-opacity-20 rounded-full w-10 h-10 flex items-center justify-center cursor-pointer" onclick="hideModal('schoolModal')">
            <i class="fas fa-times text-white"></i>
        </div>
        <h2 class="text-2xl mb-4" style="color: #C9A66B;">لیسه عالی خصوصی تجوید</h2>
        <p>لیسه عالی خصوصی تجوید به عنوان یک مؤسسه آموزشی پیشرو در افغانستان، با هدف ارتقاء کیفیت آموزش و پرورش و پاسخگویی به نیازهای روزافزون جامعه تأسیس شده است. این مؤسسه از سال ۱۳۸۸ با رویکردی نوین و علمی به ارائه آموزش‌های با کیفیت پرداخته و در تلاش است تا نسل آینده را برای چالش‌های زندگی آماده سازد. با توجه به تغییرات سریع در دنیای امروز و نیاز به مهارت‌های جدید، لیسه تجوید همواره در تلاش است تا برنامه‌های آموزشی خود را به‌روز کند و دانش‌آموزان را با مهارت‌های لازم برای موفقیت در دنیای امروز مجهز سازد.</p>
        <h3 class="text-xl mt-4">اطلاعات کلی</h3>
        <p><strong>نام مؤسسه:</strong> لیسه عالی خصوصی تجوید</p>
        <p><strong>تأسیس:</strong> این مؤسسه در سال ۱۳۸۸ تأسیس شده و از آن زمان به عنوان یکی از مراکز معتبر آموزشی در کابل شناخته می‌شود.</p>
        <p><strong>محل:</strong> لیسه تجوید در کابل، پایتخت افغانستان واقع شده و به راحتی برای دانش‌آموزان و والدین قابل دسترسی است.</p>
        <p><strong>نوع مؤسسه:</strong> این مؤسسه به صورت خصوصی اداره می‌شود و هدف آن ارائه آموزش با کیفیت به دانش‌آموزان است.</p>
        <p><strong>مؤسس:</strong> مسعود پوپل، مؤسس و مدیرعامل این مؤسسه، با تجربه و تخصص در زمینه آموزش و پرورش، نقش کلیدی در رشد و توسعه این مؤسسه ایفا کرده است.</p>
        <p><strong>تعداد دانش‌آموزان:</strong> لیسه تجوید با بیش از ۱۰۰۰ دانش‌آموز، یکی از بزرگ‌ترین مؤسسات آموزشی در کابل به شمار می‌آید.</p>
        <p><strong>تعداد معلمان:</strong> این مؤسسه دارای ۵۰ معلم مجرب و متخصص است که با روش‌های نوین تدریس آشنا هستند.</p>
        <p><strong>مدیر عامل:</strong> فاطمه رسولی به عنوان مدیرعامل، رهبری مؤسسه را بر عهده دارد و در پی ارتقاء کیفیت آموزش و پرورش دانش‌آموزان است.</p>
        <h3 class="text-xl mt-4">مأموریت</h3>
        <p>مأموریت لیسه عالی خصوصی تجوید، ارائه آموزش با کیفیت و جامع به دانش‌آموزان است. ما به دنبال ایجاد فضایی مثبت و حمایتی هستیم که در آن دانش‌آموزان بتوانند استعدادهای خود را شناسایی و پرورش دهند. ما به ارتقاء مهارت‌های تفکر انتقادی، حل مسئله و خلاقیت در دانش‌آموزان تأکید داریم. این مأموریت نه تنها به یادگیری علمی بلکه به رشد شخصی و اجتماعی دانش‌آموزان نیز توجه دارد.</p>
    </div>

    <div id="teacherModal" class="modal fixed inset-0 bg-opacity-10 bg-white backdrop-blur-lg p-8 shadow-lg z-20 overflow-y-auto hidden text-right">
        <div class="close-btn absolute top-5 left-5 bg-opacity-10 bg-white border border-opacity-20 rounded-full w-10 h-10 flex items-center justify-center cursor-pointer" onclick="hideModal('teacherModal')">
            <i class="fas fa-times text-white"></i>
        </div>
        <h2 class="text-2xl mb-4" style="color: #C9A66B;">استادان ما</h2>
        <p><strong>کادر آموزشی:</strong> تیم ما شامل استادان مجرب و متخصص در زمینه‌های مختلف است. هر یک از آن‌ها با روش‌های تدریس نوین و فلسفه‌های آموزشی خاص خود، به یادگیری مؤثر دانش‌آموزان کمک می‌کنند.</p>
        <p><strong>آموزش و پرورش:</strong> ما به آموزش مستمر استادان تاکید داریم و آن‌ها را در دوره‌های آموزشی و سمینارهای تخصصی شرکت می‌دهیم تا همیشه با جدیدترین متدهای آموزشی آشنا باشند.</p>
        <p><strong>دستاوردها:</strong></p>
        <ul class="list-disc list-inside">
            <li>معرفی مقالات و پژوهش‌های منتشر شده توسط استادان</li>
            <li>همکاری‌های بین‌المللی و پروژه‌های تحقیقاتی</li>
        </ul>
    </div>

    <div id="studentModal" class="modal fixed inset-0 bg-opacity-10 bg-white backdrop-blur-lg p-8 shadow-lg z-20 overflow-y-auto hidden text-right">
        <div class="close-btn absolute top-5 left-5 bg-opacity-10 bg-white border border-opacity-20 rounded-full w-10 h-10 flex items-center justify-center cursor-pointer" onclick="hideModal('studentModal')">
            <i class="fas fa-times text-white"></i>
        </div>
        <h2 class="text-2xl mb-4" style="color: #C9A66B;">شاگردان ما</h2>
        <p><strong>دستآوردها:</strong> در این بخش می‌توانید موفقیت‌های تحصیلی و غیرتحصیلی دانش‌آموزان را مشاهده کنید. از مسابقات علمی گرفته تا فعالیت‌های ورزشی و فرهنگی، ما به تمامی دستاوردهای آن‌ها افتخار می‌کنیم.</p>
        <p><strong>فعالیت‌ها:</strong></p>
        <ul class="list-disc list-inside">
            <li>برگزاری کارگاه‌های آموزشی و سمینارها</li>
            <li>شرکت در مسابقات ملی و بین‌المللی</li>
            <li>پروژه‌های گروهی و فعالیت‌های اجتماعی</li>
        </ul>
        <p><strong>نظرات دانش‌آموزان:</strong> بازخورد و نظرات دانش‌آموزان درباره تجربیاتشان در لیسه، که می‌تواند به دیگران کمک کند تا با فضای آموزشی ما آشنا شوند.</p>
    </div>

    <div id="messageModal" class="modal fixed inset-0 bg-opacity-10 bg-white backdrop-blur-lg p-8 shadow-lg z-20 overflow-y-auto hidden text-right">
        <div class="close-btn absolute top-5 left-5 bg-opacity-10 bg-white border border-opacity-20 rounded-full w-10 h-10 flex items-center justify-center cursor-pointer" onclick="hideModal('messageModal')">
            <i class="fas fa-times text-white"></i>
        </div>
        <h2 class="text-2xl mb-4" style="color: #C9A66B;">پیام مدیریت – لیسه عالی خصوصی تجوید</h2>
        <p>در لیسه عالی خصوصی تجوید، ما به این باور داریم که آموزش باکیفیت و اصولی، زیربنای پیشرفت هر جامعه است. رسالت ما، ایجاد محیطی علمی، فرهنگی و اخلاقی است که در آن دانش‌آموزان بتوانند استعدادهای خود را شکوفا ساخته و برای آینده‌ای روشن و درخشان آماده شوند.</p>
        <h3 class="text-xl mt-4">اهداف و ارزش‌های ما:</h3>
        <ul class="list-disc list-inside">
            <li>✅ ایجاد محیطی سالم و امن: ما فضایی آرام، دوستانه و مجهز را فراهم کرده‌ایم تا دانش‌آموزان با آرامش خاطر به تحصیل بپردازند.</li>
            <li>✅ ارتقای کیفیت آموزشی: بهره‌گیری از روش‌های نوین تدریس، معلمان متخصص و برنامه‌های درسی به‌روز برای یادگیری بهتر.</li>
            <li>✅ توجه به رشد همه‌جانبه: پرورش استعدادهای علمی، اخلاقی، فرهنگی و ورزشی دانش‌آموزان در کنار آموزش دروس رسمی.</li>
            <li>✅ ترویج تفکر خلاق و انتقادی: آموزش مهارت‌های زندگی، پژوهش‌گری و پرورش روحیه‌ی تحلیل و حل مسئله.</li>
            <li>✅ ایجاد ارتباط مؤثر بین مدرسه، دانش‌آموزان و والدین: ارتباط سازنده و مؤثر میان خانواده و مدرسه برای حمایت از مسیر تحصیلی دانش‌آموزان.</li>
        </ul>
        <h3 class="text-xl mt-4">محیط آموزشی و امکانات:</h3>
        <p>ما در لیسه عالی خصوصی تجوید تلاش کرده‌ایم که با ایجاد فضای آموزشی مجهز، کلاس‌های مدرن، کتابخانه‌ای جامع، امکانات ورزشی و آزمایشگاه‌های علمی، شرایطی را فراهم کنیم که دانش‌آموزان در بهترین شرایط به یادگیری بپردازند. همچنین، رعایت اصول بهداشتی و نظافت محیط آموزشی، از اولویت‌های ماست تا محیطی سالم و مناسب برای یادگیری ایجاد شود.</p>
        <h3 class="text-xl mt-4">فعالیت‌های فرهنگی و علمی:</h3>
        <p>ما به برگزاری برنامه‌های فرهنگی، اردوهای علمی و تفریحی، مسابقات علمی، نمایشگاه‌های آموزشی و مراسم تقدیر از دانش‌آموزان برتر توجه ویژه‌ای داریم تا علاوه بر آموزش، استعدادهای دانش‌آموزان را نیز تقویت کنیم.</p>
        <h3 class="text-xl mt-4">پیام ما به والدین و دانش‌آموزان:</h3>
        <p>ما در تلاش هستیم که با همکاری معلمان متخصص، مدیریت پویا و والدین دلسوز، آینده‌ای روشن برای فرزندان این سرزمین بسازیم. حضور شما در این مسیر، ما را در تحقق این هدف یاری خواهد کرد.</p>
        <p>با آرزوی موفقیت و پیشرفت روزافزون برای تمام دانش‌آموزان عزیز،<br>مدیریت لیسه عالی خصوصی تجوید</p>
    </div>

    <div id="menu" class="fixed inset-y-0 right-0 w-1/2 bg-opacity-10 bg-white backdrop-blur-lg p-8 shadow-lg z-30 overflow-y-auto hidden text-right">
        <h2 class="text-2xl mb-4" style="color: #C9A66B;">صفحه اصلی</h2>
        <ul class="list-disc list-inside">
            <li class="mt-2"><a href="#" class="text-lg" onclick="showModal('schoolModal'); toggleMenu();">مکتب ما</a></li>
            <li class="mt-2"><a href="#" class="text-lg" onclick="showModal('teacherModal'); toggleMenu();">استادان ما</a></li>
            <li class="mt-2"><a href="#" class="text-lg" onclick="showModal('studentModal'); toggleMenu();">شاگردان ما</a></li>
            <li class="mt-2"><a href="#" class="text-lg" onclick="showModal('messageModal'); toggleMenu();">پیام مدیریت</a></li>
        </ul>
    </div>

    <div class="container mx-auto text-center relative z-10 mt-8">
        <h2 class="text-xl font-bold mb-4" style="color: #C9A66B;">تماس با ما</h2>
        <p class="mb-4">ما در لیسه عالی خصوصی تجوید به دنبال پرورش نسل‌های آینده با آموزش‌های کیفی و نوین هستیم. هدف ما ایجاد فضایی امن و پویای تحصیلی است تا دانش‌آموزان با بهره‌گیری از بهترین روش‌های آموزشی، مهارت‌های علمی و عملی خود را توسعه دهند و برای چالش‌های فردا آماده شوند.</p>
        <h3 class="text-lg font-bold mb-2">آدرس:</h3>
        <p class="mb-4">کابل، جاده شهید مزاری، ایستگاه تانک تیل، بعد از اولین سه‌راهی به سمت راست، کوچه سوم.</p>
        <h3 class="text-lg font-bold mb-2">تماس:</h3>
        <p class="mb-4">۰۷۹۴۸۲۹۰۹۰</p>
        <h3 class="text-lg font-bold mb-2">ایمیل:</h3>
        <p class="mb-4">tajweed.privateschool@gmail.com</p>
    </div>

    <script>
        function showModal(modalId) {
            document.getElementById(modalId).classList.remove('hidden');
        }

        function hideModal(modalId) {
            document.getElementById(modalId).classList.add('hidden');
        }

        function toggleMenu() {
            const menu = document.getElementById('menu');
            menu.classList.toggle('hidden');
        }
    </script>
</body>
</html>
