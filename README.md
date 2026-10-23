<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>قهوة أولاد البلد - طلبات، ألعاب، وماتشات</title>
    <!-- Tailwind CSS CDN -->
    <script src="https://cdn.jsdelivr.net/npm/@tailwindcss/browser@4"></script>
    <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@400;600;700;900&display=swap" rel="stylesheet">
    <style>
        body { font-family: 'Cairo', sans-serif; }
        /* إخفاء شريط التمرير للسلايدر مع الحفاظ على قابليته للسحب */
        .no-scrollbar::-webkit-scrollbar { display: none; }
        .no-scrollbar { -ms-overflow-style: none; scrollbar-width: none; }
    </style>
</head>
<body class="bg-amber-50 text-gray-800 min-h-screen pb-28">

    <!-- Header / الهيدر -->
    <header class="bg-amber-900 text-amber-100 p-4 shadow-md sticky top-0 z-50 text-center">
        <h1 class="text-2xl font-black">☕ قهوة أولاد البلد</h1>
        <p class="text-xs text-amber-200 mt-1">أصل القهوة البلدي.. اطلب، العب، وعيش جو الماتشات</p>
    </header>

    <!-- معلومات الطاولة والزبون -->
    <div class="max-w-md mx-auto p-4">
        <div class="bg-white p-3 rounded-xl shadow-sm border border-amber-200 flex justify-between items-center mb-4">
            <div>
                <span class="text-xs text-gray-500 block">الترابيزة الحالية:</span>
                <span class="font-bold text-amber-900 text-lg">ترابيزة رقم (5)</span>
            </div>
            <div>
                <input type="text" id="customerName" placeholder="اكتب اسمك هنا..." class="border border-gray-300 rounded-lg px-3 py-1.5 text-sm focus:outline-none focus:border-amber-700 w-36">
            </div>
        </div>

        <!-- ⚽ سلايدر المباريات والأخبار الحية -->
        <div class="mb-4">
            <div class="flex justify-between items-center mb-2 px-1">
                <h3 class="font-bold text-xs text-amber-900 flex items-center gap-1">⚽ شاشة ستاد أولاد البلد</h3>
                <span class="text-[10px] bg-red-600 text-white px-2 py-0.5 rounded-full animate-pulse font-bold">مباشر الآن</span>
            </div>
            <!-- السلايدر الأفقي -->
            <div class="flex gap-3 overflow-x-auto no-scrollbar pb-2 snap-x">
                <!-- كارت ماتش 1 (شغال) -->
                <div class="min-w-[240px] bg-gradient-to-l from-zinc-900 to-amber-950 text-white p-3 rounded-xl shadow-md border border-amber-600/50 snap-start flex-shrink-0">
                    <div class="flex justify-between items-center text-[10px] text-amber-400 mb-1 font-bold">
                        <span>دوري أبطال أوروبا</span>
                        <span class="bg-red-500/80 px-1.5 py-0.5 rounded text-white">الدقيقة 74'</span>
                    </div>
                    <div class="flex justify-between items-center my-2 text-xs font-bold">
                        <span>ريال مدريد</span>
                        <span class="bg-amber-500 text-amber-950 px-2 py-0.5 rounded-md font-black text-sm">2 - 1</span>
                        <span>مانشستر سيتي</span>
                    </div>
                    <p class="text-[10px] text-gray-300 text-center border-t border-gray-700 pt-1">🔥 اطلب الشاي وتابع الحلبة ع الشاشة!</p>
                </div>

                <!-- كارت ماتش 2 (قادم) -->
                <div class="min-w-[240px] bg-gradient-to-l from-zinc-900 to-amber-950 text-white p-3 rounded-xl shadow-md border border-amber-600/50 snap-start flex-shrink-0">
                    <div class="flex justify-between items-center text-[10px] text-amber-400 mb-1 font-bold">
                        <span>الدوري المصري الممتاز</span>
                        <span class="bg-amber-600/80 px-1.5 py-0.5 rounded text-white">الليلة 9:00 م</span>
                    </div>
                    <div class="flex justify-between items-center my-2 text-xs font-bold">
                        <span>الأهلي</span>
                        <span class="text-amber-300 font-black text-sm">VS</span>
                        <span>الزمالك</span>
                    </div>
                    <p class="text-[10px] text-gray-300 text-center border-t border-gray-700 pt-1">🥤 احجز ترابيزتك الماتش هيولع!</p>
                </div>

                <!-- كارت ماتش 3 (قادم) -->
                <div class="min-w-[240px] bg-gradient-to-l from-zinc-900 to-amber-950 text-white p-3 rounded-xl shadow-md border border-amber-600/50 snap-start flex-shrink-0">
                    <div class="flex justify-between items-center text-[10px] text-amber-400 mb-1 font-bold">
                        <span>دوري أبطال أفريقيا</span>
                        <span class="bg-amber-600/80 px-1.5 py-0.5 rounded text-white">غداً 8:00 م</span>
                    </div>
                    <div class="flex justify-between items-center my-2 text-xs font-bold">
                        <span>الترجي التونسي</span>
                        <span class="text-amber-300 font-black text-sm">VS</span>
                        <span>صن داونز</span>
                    </div>
                    <p class="text-[10px] text-gray-300 text-center border-t border-gray-700 pt-1">☕ قهوتك مظبوطة وسهرتك عندنا</p>
                </div>
            </div>
        </div>

        <!-- زر الطلب الصوتي الشات السريع -->
        <div class="bg-amber-800 text-white p-3 rounded-xl shadow-md mb-4 flex justify-between items-center">
            <div class="flex items-center gap-2">
                <span class="text-2xl">🎙️</span>
                <div>
                    <h3 class="font-bold text-sm">طلب فويس نوت للبار</h3>
                    <p class="text-xs text-amber-200">اضغط وتكلم مباشر مع الصنايعي</p>
                </div>
            </div>
            <button onclick="alert('جاري تفعيل التسجيل الصوتي...')" class="bg-amber-500 hover:bg-amber-600 text-white px-3 py-1.5 rounded-lg text-xs font-bold transition">اضغط وتكلم</button>
        </div>

        <!-- قسم التسلية والألعاب الرقمية 🎮 -->
        <div class="bg-gradient-to-r from-amber-700 to-amber-900 text-white p-4 rounded-2xl shadow-md mb-6">
            <div class="flex justify-between items-center mb-3">
                <h3 class="font-bold text-base flex items-center gap-1.5">🎲 تسلية أولاد البلد</h3>
                <span class="text-xs bg-amber-500/80 px-2 py-0.5 rounded-full">سهرة تروق الدم</span>
            </div>
            
            <div class="grid grid-cols-2 gap-2">
                <button onclick="openXOGame()" class="bg-amber-800 hover:bg-amber-900 border border-amber-600 p-2.5 rounded-xl text-center transition">
                    <span class="text-xl block mb-1">❌⭕</span>
                    <span class="text-xs font-bold block">لعبة الإكس أو</span>
                </button>
                <button onclick="spinLuckyCup()" class="bg-amber-800 hover:bg-amber-900 border border-amber-600 p-2.5 rounded-xl text-center transition">
                    <span class="text-xl block mb-1">🍀</span>
                    <span class="text-xs font-bold block">حظك على القهوة</span>
                </button>
            </div>
        </div>

        <!-- قسم المنيو / القائمة -->
        <h2 class="text-lg font-bold text-amber-900 mb-3 border-b border-amber-200 pb-1">📜 منيو المشاريب والمأكولات</h2>
        
        <div class="grid grid-cols-1 gap-3">
            <div class="bg-white p-3 rounded-xl shadow-sm border border-amber-100 flex justify-between items-center">
                <div>
                    <h3 class="font-bold text-gray-800">شاي مظبوط ع السريع</h3>
                    <p class="text-xs text-amber-700 font-semibold mt-0.5">5 جنيه</p>
                </div>
                <button onclick="addToCart('شاي مظبوط', 5)" class="bg-amber-900 text-white px-3 py-1.5 rounded-lg text-xs font-bold hover:bg-amber-800 transition">+ أضف</button>
            </div>

            <div class="bg-white p-3 rounded-xl shadow-sm border border-amber-100 flex justify-between items-center">
                <div>
                    <h3 class="font-bold text-gray-800">قهوة وسط (وش مضبوط)</h3>
                    <p class="text-xs text-amber-700 font-semibold mt-0.5">15 جنيه</p>
                </div>
                <button onclick="addToCart('قهوة وسط', 15)" class="bg-amber-900 text-white px-3 py-1.5 rounded-lg text-xs font-bold hover:bg-amber-800 transition">+ أضف</button>
            </div>

            <div class="bg-white p-3 rounded-xl shadow-sm border border-amber-100 flex justify-between items-center">
                <div>
                    <h3 class="font-bold text-gray-800">حلبة حصى بالمكسرات</h3>
                    <p class="text-xs text-amber-700 font-semibold mt-0.5">10 جنيه</p>
                </div>
                <button onclick="addToCart('حلبة حصى', 10)" class="bg-amber-900 text-white px-3 py-1.5 rounded-lg text-xs font-bold hover:bg-amber-800 transition">+ أضف</button>
            </div>
        </div>
    </div>

    <!-- نافذة منبثقة للألعاب (Modal) -->
    <div id="gameModal" class="fixed inset-0 bg-black/60 z-50 hidden flex items-center justify-center p-4">
        <div class="bg-white w-full max-w-sm rounded-2xl p-5 shadow-2xl relative text-center">
            <button onclick="closeGameModal()" class="absolute top-3 left-3 text-gray-400 hover:text-gray-700 font-bold text-lg">✕</button>
            <h3 id="gameTitle" class="font-bold text-lg text-amber-900 mb-3">🎮 تسلية القهوة</h3>
            <div id="gameContent" class="py-4"></div>
        </div>
    </div>

    <!-- شريط سلة الطلبات العائم أسفل الشاشة -->
    <div id="cartBar" class="fixed bottom-0 left-0 right-0 bg-white border-t border-amber-300 shadow-xl p-4 max-w-md mx-auto rounded-t-2xl hidden z-40">
        <div class="flex justify-between items-center mb-2">
            <span class="font-bold text-amber-900 text-sm">سلة طلباتك (<span id="cartCount">0</span>)</span>
            <span class="font-bold text-amber-800 text-sm" id="cartTotal">0 ج.م</span>
        </div>
        <div id="cartItemsList" class="text-xs text-gray-600 mb-3 max-h-20 overflow-y-auto"></div>
        <button onclick="checkout()" class="w-full bg-emerald-600 hover:bg-emerald-700 text-white font-bold py-2.5 rounded-xl text-sm transition shadow">تأكيد وإرسال للبار 🚀</button>
    </div>

    <script>
        let cart = [];

        function addToCart(name, price) {
            cart.push({ name, price });
            updateCartUI();
        }

        function updateCartUI() {
            const cartBar = document.getElementById('cartBar');
            const cartCount = document.getElementById('cartCount');
            const cartTotal = document.getElementById('cartTotal');
            const cartItemsList = document.getElementById('cartItemsList');

            if (cart.length > 0) {
                cartBar.classList.remove('hidden');
                cartCount.innerText = cart.length;
                
                let total = 0;
                let itemsHtml = '';
                cart.forEach((item) => {
                    total += item.price;
                    itemsHtml += `<div>- ${item.name} (${item.price} ج)</div>`;
                });
                cartTotal.innerText = total + ' ج.م';
                cartItemsList.innerHTML = itemsHtml;
            } else {
                cartBar.classList.add('hidden');
            }
        }

        function checkout() {
            const name = document.getElementById('customerName').value || 'ترابيزة 5';
            alert(`يا مرحب يا معلم ${name}! أوردرك وصل للبار وجاري التحضير ☕`);
            cart = [];
            updateCartUI();
        }

        function openGameModal(title, htmlContent) {
            document.getElementById('gameTitle').innerText = title;
            document.getElementById('gameContent').innerHTML = htmlContent;
            document.getElementById('gameModal').classList.remove('hidden');
        }

        function closeGameModal() {
            document.getElementById('gameModal').classList.add('hidden');
        }

        function spinLuckyCup() {
            const prizes = [
                "🎉 مبروك! كسبت كوباية شاي مجاناً من المعلم!",
                "☕ خسرت المرة دي.. اطلب قهوة وربنا يعوض عليك!",
                "🔥 ليلتك فل! خصم 20% على طلبك الجاي.",
                "⭐ حظك حلو.. البار هيبعتلك تسالي مع الأوردر!"
            ];
            const randomPrize = prizes[Math.floor(Math.random() * prizes.length)];
            openGameModal("🍀 حظك اليوم على القهوة", `<p class="text-base font-bold text-amber-800 p-4 bg-amber-50 rounded-xl">${randomPrize}</p>`);
        }

        function openXOGame() {
            let boardHtml = `
                <p class="text-xs text-gray-500 mb-3">العب مع صاحبك اللي معاك على الترابيزة وخلي الخسران يحاسب! 😉</p>
                <div class="grid grid-cols-3 gap-2 max-w-[200px] mx-auto">
                    <button onclick="this.innerText='X'" class="h-16 bg-amber-100 text-2xl font-black rounded-lg text-amber-900 border border-amber-300"></button>
                    <button onclick="this.innerText='X'" class="h-16 bg-amber-100 text-2xl font-black rounded-lg text-amber-900 border border-amber-300"></button>
                    <button onclick="this.innerText='X'" class="h-16 bg-amber-100 text-2xl font-black rounded-lg text-amber-900 border border-amber-300"></button>
                    <button onclick="this.innerText='X'" class="h-16 bg-amber-100 text-2xl font-black rounded-lg text-amber-900 border border-amber-300"></button>
                    <button onclick="this.innerText='X'" class="h-16 bg-amber-100 text-2xl font-black rounded-lg text-amber-900 border border-amber-300"></button>
                    <button onclick="this.innerText='X'" class="h-16 bg-amber-100 text-2xl font-black rounded-lg text-amber-900 border border-amber-300"></button>
                    <button onclick="this.innerText='X'" class="h-16 bg-amber-100 text-2xl font-black rounded-lg text-amber-900 border border-amber-300"></button>
                    <button onclick="this.innerText='X'" class="h-16 bg-amber-100 text-2xl font-black rounded-lg text-amber-900 border border-amber-300"></button>
                    <button onclick="this.innerText='X'" class="h-16 bg-amber-100 text-2xl font-black rounded-lg text-amber-900 border border-amber-300"></button>
                </div>
                <button onclick="openXOGame()" class="mt-4 bg-amber-900 text-white px-4 py-1.5 rounded-lg text-xs font-bold">إعادة اللعب</button>
            `;
            openGameModal("❌⭕ لعبة الإكس أو البلدي", boardHtml);
        }
    </script>
</body>
</html>
