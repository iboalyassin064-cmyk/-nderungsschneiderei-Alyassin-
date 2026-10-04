<!DOCTYPE html>
<html lang="de" dir="ltr">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Änderungsschneiderei Alyassin | Saarlouis</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.tailwindcss.com"></script>
    <!-- Font Awesome Icons -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&family=Tajawal:wght@400;500;700&display=swap');
        body { font-family: 'Poppins', 'Tajawal', sans-serif; }
    </style>
</head>
<body class="bg-gray-50 text-gray-800 flex flex-col min-h-screen">

    <!-- Header / Navbar -->
    <header class="bg-white shadow-md sticky top-0 z-50">
        <div class="max-w-6xl mx-auto px-4 py-4 flex justify-between items-center">
            <div class="flex items-center space-x-3 rtl:space-x-reverse">
                <i class="fa-solid fa-scissors text-amber-600 text-2xl"></i>
                <div>
                    <h1 class="font-bold text-xl text-gray-900 leading-none">Alyassin</h1>
                    <span class="text-xs text-amber-700 tracking-wider">ÄNDERUNGSSCHNEIDEREI</span>
                </div>
            </div>
            
            <nav class="hidden md:flex space-x-6 rtl:space-x-reverse text-sm font-semibold">
                <a href="#about" data-i18n="nav_about" class="hover:text-amber-600 transition">Über Uns</a>
                <a href="#services" data-i18n="nav_services" class="hover:text-amber-600 transition">Leistungen</a>
                <a href="#hours" data-i18n="nav_hours" class="hover:text-amber-600 transition">Öffnungszeiten</a>
                <a href="#contact" data-i18n="nav_contact" class="hover:text-amber-600 transition">Kontakt</a>
            </nav>

            <div class="flex items-center space-x-4 rtl:space-x-reverse">
                <!-- Language Switcher Button -->
                <button onclick="toggleLanguage()" class="bg-amber-50 hover:bg-amber-100 text-amber-900 px-3 py-1.5 rounded-lg text-sm font-semibold flex items-center gap-1.5 border border-amber-200 transition">
                    <i class="fa-solid fa-globe text-amber-600"></i>
                    <span id="langBtnText">العربية</span>
                </button>

                <a href="tel:01791172056" class="bg-amber-600 hover:bg-amber-700 text-white px-4 py-2 rounded-lg text-sm font-semibold transition flex items-center gap-2">
                    <i class="fa-solid fa-phone"></i>
                    <span data-i18n="call_us">Anrufen</span>
                </a>
            </div>
        </div>
    </header>

    <!-- Hero Section -->
    <section class="bg-slate-900 text-white py-20 relative overflow-hidden">
        <div class="max-w-6xl mx-auto px-4 text-center relative z-10">
            <div class="inline-block bg-amber-600/20 text-amber-400 px-4 py-1.5 rounded-full text-sm font-semibold mb-4 border border-amber-500/30">
                <i class="fa-solid fa-star text-amber-400 mr-1"></i> <span data-i18n="hero_badge">5.0 / 5 Sterne Top-Bewertung in Saarlouis</span>
            </div>
            <h2 data-i18n="hero_title" class="text-4xl md:text-5xl font-extrabold mb-4">Perfekte Passform & Schnelle Ausführung</h2>
            <p data-i18n="hero_subtitle" class="text-lg md:text-xl text-gray-300 max-w-3xl mx-auto mb-8">
                Ihre verlässliche Änderungsschneiderei in Saarlouis-Roden. Präzise Handarbeit, freundlicher Service und perfekte Anpassung für all Ihre Kleidungsstücke.
            </p>
            <div class="flex justify-center gap-4">
                <a href="#contact" data-i18n="hero_btn" class="bg-amber-600 hover:bg-amber-700 text-white font-bold px-6 py-3 rounded-lg transition">
                    Route auf Google Maps planen
                </a>
            </div>
        </div>
    </section>

    <!-- Info Cards -->
    <section class="max-w-6xl mx-auto px-4 -mt-10 relative z-20 grid grid-cols-1 md:grid-cols-3 gap-6">
        <div class="bg-white p-6 rounded-xl shadow-lg border-t-4 border-amber-600 flex items-start gap-4">
            <i class="fa-solid fa-location-dot text-amber-600 text-2xl mt-1"></i>
            <div>
                <h3 data-i18n="card_address_title" class="font-bold text-gray-900">Adresse</h3>
                <p class="text-sm text-gray-600 mt-1">Lindenstraße 85<br>66740 Saarlouis-Roden</p>
            </div>
        </div>
        <div id="hours" class="bg-white p-6 rounded-xl shadow-lg border-t-4 border-amber-600 flex items-start gap-4">
            <i class="fa-solid fa-clock text-amber-600 text-2xl mt-1"></i>
            <div>
                <h3 data-i18n="card_hours_title" class="font-bold text-gray-900">Öffnungszeiten</h3>
                <p data-i18n="card_hours_desc" class="text-sm text-gray-600 mt-1">Mo - Fr: 08:30 - 18:30 Uhr<br>Sa: 08:30 - 15:00 Uhr<br><span class="text-red-500 font-medium">So: Geschlossen</span></p>
            </div>
        </div>
        <div class="bg-white p-6 rounded-xl shadow-lg border-t-4 border-amber-600 flex items-start gap-4">
            <i class="fa-solid fa-award text-amber-600 text-2xl mt-1"></i>
            <div>
                <h3 data-i18n="card_quality_title" class="font-bold text-gray-900">Qualität & Service</h3>
                <p data-i18n="card_quality_desc" class="text-sm text-gray-600 mt-1">Hohe Kundenzufriedenheit, professionelle Beratung und schnelle Fertigstellung.</p>
            </div>
        </div>
    </section>

    <!-- About Section (Google Description) -->
    <section id="about" class="py-16 max-w-6xl mx-auto px-4">
        <div class="bg-white rounded-2xl shadow-md p-8 border border-gray-100">
            <div class="max-w-3xl mx-auto text-center">
                <span class="text-amber-600 text-sm font-semibold tracking-wider uppercase" data-i18n="about_tag">Über Unseren Betrieb</span>
                <h2 data-i18n="about_title" class="text-3xl font-bold text-gray-900 mt-2 mb-4">Änderungsschneiderei Alyassin in Saarlouis</h2>
                <div class="w-16 h-1 bg-amber-600 mx-auto mb-6"></div>
                <p data-i18n="about_text" class="text-gray-700 leading-relaxed text-base md:text-lg">
                    Willkommen bei der Änderungsschneiderei Alyassin in Saarlouis-Roden! Wir bieten Ihnen erstklassige Schneidereidienstleistungen mit höchster Präzision und Schnelligkeit. Egal ob Anpassungen von Alltagskleidung, Reparaturen oder spezielle Wünsche – bei uns ist Ihre Kleidung in erfahrenen Händen. Unsere Kunden schätzen besonders unsere Zuverlässigkeit, saubere Verarbeitung und faire Preisgestaltung.
                </p>
            </div>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="py-12 bg-gray-100">
        <div class="max-w-6xl mx-auto px-4">
            <div class="text-center mb-12">
                <h2 data-i18n="services_title" class="text-3xl font-bold text-gray-900">Unsere Leistungen</h2>
                <div class="w-16 h-1 bg-amber-600 mx-auto mt-2"></div>
            </div>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
                <div class="bg-white p-6 rounded-xl shadow border border-gray-200 text-center hover:shadow-md transition">
                    <i class="fa-solid fa-shirt text-4xl text-amber-600 mb-4"></i>
                    <h3 data-i18n="service_1_title" class="font-bold text-xl mb-2">Kleidungsänderungen</h3>
                    <p data-i18n="service_1_desc" class="text-gray-600 text-sm">Professionelles Kürzen, Verengern oder Erweitern von Hosen, Jeans, Hemden, Jacken und Mänteln.</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow border border-gray-200 text-center hover:shadow-md transition">
                    <i class="fa-solid fa-scissors text-4xl text-amber-600 mb-4"></i>
                    <h3 data-i18n="service_2_title" class="font-bold text-xl mb-2">Reißverschlüsse & Reparatur</h3>
                    <p data-i18n="service_2_desc" class="text-gray-600 text-sm">Schneller Austausch defekter Reißverschlüsse, Flicken von Nahtrissen und Erneuerung von Futterstoffen.</p>
                </div>
                <div class="bg-white p-6 rounded-xl shadow border border-gray-200 text-center hover:shadow-md transition">
                    <i class="fa-solid fa-user-tie text-4xl text-amber-600 mb-4"></i>
                    <h3 data-i18n="service_3_title" class="font-bold text-xl mb-2">Spezial- & Maßanpassung</h3>
                    <p data-i18n="service_3_desc" class="text-gray-600 text-sm">Exakte Anpassung von Anzügen, Abendkleidern, Vorhängen und Gardinen nach Ihren individuellen Maßen.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- Contact & Map -->
    <section id="contact" class="py-16 max-w-6xl mx-auto px-4">
        <div class="grid grid-cols-1 md:grid-cols-2 gap-8 items-center">
            <div>
                <h2 data-i18n="contact_title" class="text-2xl font-bold text-gray-900 mb-4">Kontakt & Anfahrt</h2>
                <p data-i18n="contact_subtitle" class="text-gray-600 mb-6">Besuchen Sie uns direkt vor Ort in Saarlouis-Roden oder rufen Sie uns an.</p>
                <div class="space-y-4">
                    <div class="flex items-center gap-3 text-gray-700">
                        <i class="fa-solid fa-location-dot text-amber-600 text-xl w-6"></i>
                        <span>Lindenstraße 85, 66740 Saarlouis-Roden</span>
                    </div>
                    <div class="flex items-center gap-3 text-gray-700">
                        <i class="fa-solid fa-phone text-amber-600 text-xl w-6"></i>
                        <a href="tel:01791172056" class="hover:underline font-semibold">0179 1172056</a>
                    </div>
                    <div class="flex items-center gap-3 text-gray-700">
                        <i class="fa-solid fa-star text-amber-600 text-xl w-6"></i>
                        <span data-i18n="contact_rating">Google Bewertung: 5.0 ★★★★★</span>
                    </div>
                </div>
            </div>
            <div class="h-80 bg-gray-200 rounded-2xl overflow-hidden shadow-md">
                <!-- Google Map Embedding -->
                <iframe 
                    class="w-full h-full border-0"
                    src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2602.4!2d6.74!3d49.32!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4795a70181818c99%3A0x1bd1b2cb03be56ae!2sLindenstra%C3%9Fe%2085%2C%2066740%20Saarlouis!5e0!3m2!1sde!2sde!4v1600000000000!5m2!1sde!2sde" 
                    allowfullscreen="" 
                    loading="lazy">
                </iframe>
            </div>
        </div>
    </section>

    <!-- Footer -->
    <footer class="bg-slate-900 text-gray-400 py-6 text-center text-sm border-t border-slate-800">
        <p data-i18n="footer_rights">&copy; 2026 Änderungsschneiderei Alyassin Saarlouis. Alle Rechte vorbehalten.</p>
    </footer>

    <!-- Multilingual Script (Default DE) -->
    <script>
        const translations = {
            de: {
                nav_about: "Über Uns",
                nav_services: "Leistungen",
                nav_hours: "Öffnungszeiten",
                nav_contact: "Kontakt",
                call_us: "Anrufen",
                hero_badge: "5.0 / 5 Sterne Top-Bewertung in Saarlouis",
                hero_title: "Perfekte Passform & Schnelle Ausführung",
                hero_subtitle: "Ihre verlässliche Änderungsschneiderei in Saarlouis-Roden. Präzise Handarbeit, freundlicher Service und perfekte Anpassung für all Ihre Kleidungsstücke.",
                hero_btn: "Route auf Google Maps planen",
                card_address_title: "Adresse",
                card_hours_title: "Öffnungszeiten",
                card_hours_desc: "Mo - Fr: 08:30 - 18:30 Uhr<br>Sa: 08:30 - 15:00 Uhr<br><span class='text-red-500 font-medium'>So: Geschlossen</span>",
                card_quality_title: "Qualität & Service",
                card_quality_desc: "Hohe Kundenzufriedenheit, professionelle Beratung und schnelle Fertigstellung.",
                about_tag: "Über Unseren Betrieb",
                about_title: "Änderungsschneiderei Alyassin in Saarlouis",
                about_text: "Willkommen bei der Änderungsschneiderei Alyassin in Saarlouis-Roden! Wir bieten Ihnen erstklassige Schneidereidienstleistungen mit höchster Präzision und Schnelligkeit. Egal ob Anpassungen von Alltagskleidung, Reparaturen oder spezielle Wünsche – bei uns ist Ihre Kleidung in erfahrenen Händen. Unsere Kunden schätzen besonders unsere Zuverlässigkeit, saubere Verarbeitung und faire Preisgestaltung.",
                services_title: "Unsere Leistungen",
                service_1_title: "Kleidungsänderungen",
                service_1_desc: "Professionelles Kürzen, Verengern oder Erweitern von Hosen, Jeans, Hemden, Jacken und Mänteln.",
                service_2_title: "Reißverschlüsse & Reparatur",
                service_2_desc: "Schneller Austausch defekter Reißverschlüsse, Flicken von Nahtرissen und Erneuerung von Futterstoffen.",
                service_3_title: "Spezial- & Maßanpassung",
                service_3_desc: "Exakte Anpassung von Anzügen, Abendkleidern, Vorhängen und Gardinen nach Ihren individuellen Maßen.",
                contact_title: "Kontakt & Anfahrt",
                contact_subtitle: "Besuchen Sie uns direkt vor Ort in Saarlouis-Roden oder rufen Sie uns an.",
                contact_rating: "Google Bewertung: 5.0 ★★★★★",
                footer_rights: "© 2026 Änderungsschneiderei Alyassin Saarlouis. Alle Rechte vorbehalten.",
                btn_lang: "العربية"
            },
            ar: {
                nav_about: "من نحن",
                nav_services: "الخدمات",
                nav_hours: "أوقات العمل",
                nav_contact: "التواصل",
                call_us: "اتصل بنا",
                hero_badge: "تقييم 5.0 / 5 ممتاز على خرائط جوجل سارلويس",
                hero_title: "تعديل دقيق وسريع لملابسك",
                hero_subtitle: "محل الخياطة والتعديل الموثوق في سارلويس - رودن. خياطة يدوية دقيقة، خدمة ودودة، وتعديل مثالي لجميع أنواع الملابس.",
                hero_btn: "عرض الموقع على خرائط جوجل",
                card_address_title: "العنوان",
                card_hours_title: "أوقات العمل",
                card_hours_desc: "الاثنين - الجمعة: 08:30 - 18:30<br>السبت: 08:30 - 15:00<br><span class='text-red-500 font-medium'>الأحد: مغلق</span>",
                card_quality_title: "الجودة والخدمة",
                card_quality_desc: "رضا تام للعملاء، استشارة مهنية وسرعة في إنجاز الطلبات.",
                about_tag: "نبذة عن المحل",
                about_title: "خياط الياسين في سارلويس",
                about_text: "أهلاً بكم في محل Änderungsschneiderei Alyassin في سارلويس-رودن! نقدم لكم أفضل خدمات الخياطة والتعديل بأعلى درجات الدقة والسرعة. سواء كنت بحاجة لتعديل ملابسك اليومية، أو تصليح التمزقات والسحابات، أو تعديلات خاصة – ملابسك معنا في أيدٍ أمينة ومحترفة. يثق بنا عملاؤنا بفضل دقة العمل، الالتزام بالمواعيد، والأسعار المناسبة.",
                services_title: "خدماتنا",
                service_1_title: "تعديل الملابس",
                service_1_desc: "تقصير، تقضيب، وتوسيع البناطيل، الجينز، القمصان، والجاكيتات والسترات.",
                service_2_title: "تصليح وتغيير السحابات",
                service_2_desc: "استبدال السحابات التالفة بسرعة، تصليح التمزقات، وتجديد البطانة الداخلية للملابس.",
                service_3_title: "تعديلات خاصة وستائر",
                service_3_desc: "تعديل البدلات الرسمية، فساتين السهرة، والستائر وفقاً لمقاساتك الخاصة تماماً.",
                contact_title: "التواصل والوصول",
                contact_subtitle: "تفضل بزيارتنا في المحل مباشرة أو اتصل بنا هاتفياً.",
                contact_rating: "تقييم جوجل: 5.0 ★★★★★",
                footer_rights: "© 2026 خياط الياسين سارلويس. جميع الحقوق محفوظة.",
                btn_lang: "Deutsch"
            }
        };

        let currentLang = 'de'; // اللغة الافتراضية هي الألمانية

        function setLanguage(lang) {
            currentLang = lang;
            const htmlTag = document.documentElement;
            
            // تغيير اتجاه الصفحة واللغة
            htmlTag.setAttribute('lang', lang);
            htmlTag.setAttribute('dir', lang === 'ar' ? 'rtl' : 'ltr');

            // تحديث جميع النصوص
            document.querySelectorAll('[data-i18n]').forEach(element => {
                const key = element.getAttribute('data-i18n');
                if (translations[lang][key]) {
                    element.innerHTML = translations[lang][key];
                }
            });

            // تحديث نص زر اللغة
            document.getElementById('langBtnText').textContent = translations[lang]['btn_lang'];
        }

        function toggleLanguage() {
            setLanguage(currentLang === 'de' ? 'ar' : 'de');
        }

        // تشغيل اللغة الألمانية تلقائياً فور فتح الصفحة
        window.addEventListener('DOMContentLoaded', () => {
            setLanguage('de');
        });
    </script>
</body>
</html>
