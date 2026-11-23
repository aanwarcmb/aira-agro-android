AIRA AGRO — মোবাইল থেকে APK বানানোর প্রজেক্ট

গুরুত্বপূর্ণ:
এই ZIP-এ আপনার লাইব্রেরিতে পাওয়া Aira_Agro_Fram_V2 starter source ব্যবহার করা হয়েছে এবং বিক্রির ওজনের ঘর কেজি/গ্রাম পাশাপাশি করা হয়েছে। এটি আগের Netlify + Google Drive OAuth ফাইনাল HTML নয়; সেই সর্বশেষ ফাইলটি এই মুহূর্তে উপলভ্য ছিল না। তাই Google Drive Auto Backup এই APK-তে যুক্ত আছে বলে ধরে নেবেন না।

মোবাইল দিয়ে APK বানানোর ধাপ:
1) ZIP ফাইলটি Extract করুন।
2) Chrome-এ https://github.com খুলে সাইন ইন করুন।
3) New repository তৈরি করুন; নাম দিন aira-agro-android এবং Public বা Private যেকোনোটি বেছে নিন।
4) Add file > Upload files দিয়ে ZIP Extract করা ফোল্ডারের ভেতরের সব ফাইল/ফোল্ডার আপলোড করুন। .github ফোল্ডারটিও অবশ্যই আপলোড হবে।
5) Commit changes চাপুন।
6) Repository-র Actions ট্যাবে যান। "Build Aira Agro APK" workflow নির্বাচন করে Run workflow চাপুন (push হলে স্বয়ংক্রিয়ভাবেও চলবে)।
7) Build শেষ হলে workflow run খুলুন। নিচে Artifacts অংশে Aira-Agro-debug-APK চাপলে APK ZIP ডাউনলোড হবে।
8) ডাউনলোড করা artifact ZIP Extract করে app-debug.apk খুলে Install দিন। Android চাইলে Chrome/Files-এর জন্য "Install unknown apps" অনুমতি দিন।

নোট:
- GitHub account প্রয়োজন।
- প্রথমবার build হতে কয়েক মিনিট লাগতে পারে।
- এটি debug APK; Play Store release signing নয়।
- ডাটা এই অ্যাপের WebView local storage-এ থাকে। অ্যাপ uninstall/clear data করলে ডাটা মুছে যেতে পারে; নিয়মিত backup রাখুন।
- Google Drive backup / OAuth-এর জন্য আলাদা কনফিগারেশন ও পরীক্ষা প্রয়োজন।
