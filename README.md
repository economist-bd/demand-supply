<!DOCTYPE html>
<html lang="bn">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>প্রজেক্ট ডকুমেন্টেশন: চাহিদা-যোগান</title>
    
    <!-- Google Fonts (Hind Siliguri) -->
    <link href="https://fonts.googleapis.com/css2?family=Hind+Siliguri:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    
    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>

    <style>
        body {
            font-family: 'Hind Siliguri', sans-serif;
            background-color: #f8fafc;
            color: #1e293b;
            line-height: 1.6;
        }
        h1, h2, h3, h4 {
            color: #0f172a;
        }
        code {
            font-family: Consolas, Monaco, 'Andale Mono', 'Ubuntu Mono', monospace;
            background-color: #f1f5f9;
            padding: 0.2rem 0.4rem;
            border-radius: 0.25rem;
            color: #ef4444;
            font-size: 0.9em;
        }
        .section-card {
            background: white;
            border-radius: 0.75rem;
            box-shadow: 0 1px 3px 0 rgb(0 0 0 / 0.1), 0 1px 2px -1px rgb(0 0 0 / 0.1);
            padding: 2rem;
            margin-bottom: 2rem;
            border: 1px solid #e2e8f0;
        }
        ul {
            list-style-type: disc;
            padding-left: 1.5rem;
        }
        li {
            margin-bottom: 0.5rem;
        }
    </style>
</head>
<body class="p-4 md:p-8 max-w-5xl mx-auto">

    <!-- Header -->
    <header class="text-center mb-10">
        <h1 class="text-3xl md:text-4xl font-bold mb-4 text-blue-700">প্রজেক্ট ডকুমেন্টেশন: চাহিদা-যোগান (ই-কমার্স)</h1>
        <p class="text-lg text-gray-600 max-w-3xl mx-auto">
            এই প্রজেক্টটি একটি <strong>Single Page Application (SPA)</strong> যা HTML, Tailwind CSS এবং Firebase ব্যবহার করে তৈরি করা হয়েছে। এটিতে ডায়নামিক প্রোডাক্ট লোডিং, কার্ট সিস্টেম, ইউজার অথেন্টিকেশন এবং একটি ফিচার-সমৃদ্ধ অ্যাডমিন প্যানেল রয়েছে।
        </p>
    </header>

    <!-- Tech Stack -->
    <section class="section-card">
        <h2 class="text-2xl font-bold mb-4 border-b pb-2 border-gray-200">১. প্রযুক্তি এবং সেটআপ (Tech Stack)</h2>
        <ul class="text-gray-700 space-y-2">
            <li><strong>ফ্রন্টএন্ড:</strong> HTML5, JavaScript (ES6 Modules)</li>
            <li><strong>ডিজাইন ফ্রেমওয়ার্ক:</strong> Tailwind CSS (CDN)</li>
            <li><strong>আইকন:</strong> FontAwesome (CDN)</li>
            <li><strong>ফন্ট:</strong> Google Fonts (Hind Siliguri)</li>
            <li><strong>ব্যাকএন্ড ও ডাটাবেস:</strong> Firebase Authentication & Firestore Database (v11.6.1)</li>
            <li><strong>ইমেইল সার্ভিস:</strong> Formspree (ফুটারের কন্টাক্ট ফর্মের জন্য)</li>
        </ul>
    </section>

    <!-- UI & Features -->
    <section class="section-card">
        <h2 class="text-2xl font-bold mb-6 border-b pb-2 border-gray-200">২. ইউজার ইন্টারফেস (UI) ও ফিচারসমূহ</h2>

        <div class="grid md:grid-cols-2 gap-6">
            <div>
                <h3 class="text-xl font-semibold mb-3 text-blue-600">হিরো সেকশন (Hero Section)</h3>
                <ul class="text-gray-700 mb-4">
                    <li><strong>ডায়নামিক স্লাইডার:</strong> অ্যাডমিন প্যানেল থেকে নিয়ন্ত্রিত অটোমেটিক স্লাইডার।</li>
                    <li><strong>কন্টেন্ট:</strong> প্রতিটি স্লাইডে টাইটেল, সাব-টাইটেল এবং "অর্ডার করুন" বাটন।</li>
                    <li><strong>ফলব্যাক:</strong> ডাটাবেসে ব্যানার না থাকলে ডিফল্ট ৫টি ব্যানার দেখাবে।</li>
                </ul>
            </div>

            <div>
                <h3 class="text-xl font-semibold mb-3 text-blue-600">নেভিগেশন (Navigation)</h3>
                <ul class="text-gray-700 mb-4">
                    <li><strong>ডেস্কটপ:</strong> টপ বারে ক্যাটাগরি মেনু।</li>
                    <li><strong>মোবাইল:</strong> হ্যামবার্গার মেনু সহ সাইড ড্রয়ার (Side Drawer)।</li>
                    <li><strong>স্টিকি হেডার:</strong> স্ক্রল করলেও মেনু উপরে ফিক্সড থাকবে।</li>
                </ul>
            </div>
        </div>

        <div class="mt-4">
            <h3 class="text-xl font-semibold mb-3 text-blue-600">প্রোডাক্ট ডিসপ্লে ও ফ্রি বই ফিচার</h3>
            <ul class="text-gray-700 mb-4">
                <li><strong>ক্যাটাগরি ভিত্তিক:</strong> প্রতিটি ক্যাটাগরি আলাদা সেকশনে দেখাবে।</li>
                <li><strong>ফ্রি বই লজিক:</strong> বইয়ের দাম ০ টাকা হলে:
                    <ul class="ml-4 mt-2 list-[circle]">
                        <li>কভারে লাল রঙের <strong>"ফ্রি"</strong> স্টিকার দেখাবে।</li>
                        <li>"কার্টে নিন" বাটনের পরিবর্তে <strong>"ডাউনলোড করুন"</strong> বাটন আসবে।</li>
                        <li><strong>লগইন ছাড়াই</strong> সরাসরি পিডিএফ ডাউনলোড করা যাবে।</li>
                    </ul>
                </li>
                <li><strong>পেইড বই:</strong> সাধারণ বইয়ের ক্ষেত্রে "কার্টে নিন" বাটন এবং দাম দেখাবে।</li>
                <li><strong>মডেল ভিউ:</strong> পণ্যের বিস্তারিত, লেখকের নাম এবং বড় ছবি দেখার জন্য পপ-আপ মডেল।</li>
            </ul>
        </div>

        <div class="grid md:grid-cols-2 gap-6 mt-4">
            <div>
                <h3 class="text-xl font-semibold mb-3 text-blue-600">শপিং কার্ট ও চেকআউট</h3>
                <ul class="text-gray-700">
                    <li><strong>সাইডবার কার্ট:</strong> ডান পাশ থেকে স্লাইড হয়ে আসা কার্ট।</li>
                    <li><strong>শিপিং চার্জ:</strong> ঢাকার ভেতরে (২০ টাকা) এবং বাহিরে (৬০ টাকা) রেডিও বাটন সিলেকশন।</li>
                    <li><strong>পেমেন্ট মেথড:</strong>
                        <ul class="ml-4 mt-1 list-[circle]">
                            <li>ক্যাশ অন ডেলিভারি (COD)।</li>
                            <li>বিকাশ (সিলেক্ট করলে পার্সোনাল নাম্বার এবং TrxID ইনপুট ফিল্ড দেখাবে)।</li>
                        </ul>
                    </li>
                </ul>
            </div>
            <div>
                <h3 class="text-xl font-semibold mb-3 text-blue-600">ইউজার ড্যাশবোর্ড</h3>
                <ul class="text-gray-700">
                    <li>লগইন থাকা অবস্থায় ইউজার নিজের সব অর্ডার দেখতে পারবে।</li>
                    <li>অর্ডারের স্ট্যাটাস (Pending, Delivered, Cancelled) কালার কোড সহ দেখা যাবে।</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Admin Panel -->
    <section class="section-card">
        <h2 class="text-2xl font-bold mb-6 border-b pb-2 border-gray-200">৩. অ্যাডমিন প্যানেল (Admin Panel)</h2>
        <div class="bg-blue-50 p-4 rounded-lg mb-4 border border-blue-100">
            <strong>অ্যাক্সেস:</strong> শুধুমাত্র নির্দিষ্ট ইমেইল (<code>eco452@gmail.com</code>) দিয়ে লগইন করলে "Admin" বাটন দৃশ্যমান হবে।<br>
            <strong>ট্যাব সিস্টেম:</strong> ৩টি প্রধান ট্যাব - অর্ডার, পণ্য, ব্যানার।
        </div>

        <div class="space-y-4">
            <div>
                <h4 class="font-bold text-lg">ক. অর্ডার ম্যানেজমেন্ট</h4>
                <p>সকল কাস্টমারের অর্ডার লিস্ট (তারিখ অনুযায়ী সর্ট করা)। অর্ডার স্ট্যাটাস পরিবর্তন করার ড্রপডাউন (Pending -> Processing -> Delivered -> Cancelled)।</p>
            </div>
            <div>
                <h4 class="font-bold text-lg">খ. পণ্য ম্যানেজমেন্ট (Product CRUD)</h4>
                <ul class="text-gray-700">
                    <li><strong>নতুন পণ্য যোগ:</strong> নাম, <strong>লেখক (ঐচ্ছিক)</strong>, ক্যাটাগরি, দাম, বিবরণ।
                        <ul class="ml-4 list-[circle]">
                            <li><strong>ছবি আপলোড:</strong> লোকাল ফাইল সিলেক্ট করলে অটোমেটিক রিসাইজ (Max Width 400px) হয়ে Base64 ফরম্যাটে সেভ হয়। অথবা সরাসরি ইমেজ লিংক দেওয়া যায়।</li>
                            <li><strong>PDF আপলোড:</strong> দাম ০ দিলে PDF লিংক বা ফাইল আপলোডের অপশন দৃশ্যমান হয় (ফ্রি বইয়ের জন্য)।</li>
                        </ul>
                    </li>
                    <li><strong>এডিট ও ডিলিট:</strong> যেকোনো পণ্য এডিট বা ডিলিট করার সুবিধা।</li>
                </ul>
            </div>
            <div>
                <h4 class="font-bold text-lg">গ. ব্যানার ম্যানেজমেন্ট</h4>
                <p>হিরো সেকশনের জন্য নতুন ব্যানার ছবি ও টাইটেল যোগ করা এবং পুরানো ব্যানার ডিলিট করা।</p>
            </div>
        </div>
    </section>

    <!-- Database Structure -->
    <section class="section-card">
        <h2 class="text-2xl font-bold mb-6 border-b pb-2 border-gray-200">৪. ডাটাবেস স্ট্রাকচার (Firestore Collections)</h2>
        <p class="mb-4">এই প্রজেক্টটি চালানোর জন্য Firestore-এ ৩টি কালেকশন ব্যবহার করা হয়েছে (এগুলো অটোমেটিক তৈরি হয়):</p>

        <div class="grid md:grid-cols-3 gap-4">
            <div class="bg-gray-50 p-4 rounded border border-gray-200">
                <h3 class="font-bold text-blue-700 mb-2">1. products</h3>
                <ul class="text-sm space-y-1">
                    <li><code>title</code> (string)</li>
                    <li><code>author</code> (string) - লেখকের নাম</li>
                    <li><code>category</code> (string)</li>
                    <li><code>price</code> (number)</li>
                    <li><code>description</code> (string)</li>
                    <li><code>img</code> (string - Base64/URL)</li>
                    <li><code>pdf</code> (string - Base64/URL) [ফ্রি বই]</li>
                    <li><code>createdAt</code> (timestamp)</li>
                </ul>
            </div>

            <div class="bg-gray-50 p-4 rounded border border-gray-200">
                <h3 class="font-bold text-blue-700 mb-2">2. orders</h3>
                <ul class="text-sm space-y-1">
                    <li><code>userId</code> (string)</li>
                    <li><code>userEmail</code> (string)</li>
                    <li><code>customer</code> (map: name, phone, address)</li>
                    <li><code>items</code> (array: cart items)</li>
                    <li><code>total</code> (number)</li>
                    <li><code>payment</code> (map: method, trxId)</li>
                    <li><code>status</code> (string)</li>
                    <li><code>createdAt</code> (timestamp)</li>
                </ul>
            </div>

            <div class="bg-gray-50 p-4 rounded border border-gray-200">
                <h3 class="font-bold text-blue-700 mb-2">3. banners</h3>
                <ul class="text-sm space-y-1">
                    <li><code>title</code> (string)</li>
                    <li><code>sub</code> (string)</li>
                    <li><code>img</code> (string - Base64/URL)</li>
                    <li><code>createdAt</code> (timestamp)</li>
                </ul>
            </div>
        </div>
    </section>

    <!-- Logic Notes -->
    <section class="section-card">
        <h2 class="text-2xl font-bold mb-4 border-b pb-2 border-gray-200">৫. গুরুত্বপূর্ণ লজিক নোট</h2>
        <ul class="text-gray-700 space-y-2">
            <li><strong>ইমেজ কমপ্রেশন:</strong> ব্রাউজার ভারী হওয়া রোধ করতে আপলোডের সময় জাভাস্ক্রিপ্ট ক্যানভাস ব্যবহার করে ছবি ছোট করে ডাটাবেসে সেভ করা হয়।</li>
            <li><strong>অথেন্টিকেশন:</strong> Firebase Auth ব্যবহার করা হয়েছে, যা সেশন মনে রাখে (রিফ্রেশ দিলেও লগইন থাকে)।</li>
            <li><strong>টোস্ট মেসেজ:</strong> সুন্দর ইউজার অভিজ্ঞতার জন্য কাস্টম টোস্ট নোটিফিকেশন ব্যবহার করা হয়েছে।</li>
        </ul>
    </section>

    <footer class="text-center text-gray-500 text-sm mt-8 pb-8">
        &copy; 2025 চাহিদা-যোগান প্রজেক্ট ডকুমেন্টেশন
    </footer>

</body>
</html>
