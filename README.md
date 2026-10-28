# ছোট্ট সোনা – বেবি শপ 🍼

বেবি প্রোডাক্টের বাংলা ও ইংরেজি অনলাইন শপ (ডেমো)।

🔗 **লাইভ ডেমো:** https://আপনার-username.github.io/chotto-shona/

## ফিচার
- বাংলা / English ভাষা বাটন
- ক্যাটাগরি, সার্চ, পণ্যের ডিটেইল, উইশলিস্ট
- কার্ট ও কুপন
- চেকআউট: COD, bKash, Nagad
- ঢাকার ভিতরে ও বাইরে আলাদা ডেলিভারি চার্জ
- ইউজার রেজিস্টার ও লগইন, অর্ডার হিস্ট্রি
- অ্যাডমিন প্যানেল: অর্ডার, পণ্য ও কুপন ম্যানেজ
- রিটার্ন পলিসি (৭ দিন)

## প্রযুক্তি
শুধু HTML, CSS ও JavaScript। একটাই ফাইল (`index.html`), কোনো ইনস্টলেশন লাগে না।

## নোট
এটা ডেমো ভার্সন। অর্ডার, অ্যাকাউন্ট ও পণ্য শুধু ব্রাউজারের localStorage-এ থাকে। আসল ব্যবহারের জন্য ব্যাকএন্ড (Firebase/Supabase) যোগ করা হবে।

## যোগাযোগ
📞 01719961987

## Firebase সেটআপ (অর্ডার অ্যাডমিনে আনতে)
1. https://console.firebase.google.com এ নতুন প্রজেক্ট খুলুন।
2. Build → Authentication → Sign-in method → **Email/Password** চালু করুন।
3. Authentication → Users → Add user: আপনার অ্যাডমিন ইমেইল ও পাসওয়ার্ড দিন।
4. Build → Firestore Database → Create database (production mode)।
5. Firestore → Rules এ `firestore.rules` ফাইলের লেখা পেস্ট করুন। `admin@example.com` এর জায়গায় আপনার অ্যাডমিন ইমেইল বসান, তারপর Publish।
6. Project settings → Your apps → Web app (`</>`) যোগ করে `firebaseConfig` কপি করুন।
7. `index.html` এ `const FB_CFG=null,ADMIN_EMAIL='admin@example.com';` লাইনটা খুঁজে `null` এর জায়গায় কনফিগ বসান এবং `ADMIN_EMAIL` এ আপনার অ্যাডমিন ইমেইল দিন।
8. Authentication → Settings → Authorized domains এ `আপনার-username.github.io` যোগ করুন।
9. সাইটে অ্যাডমিন ইমেইল ও পাসওয়ার্ড দিয়ে লগইন করুন (লগইন ঘরে মোবাইলের জায়গায় ইমেইল লিখবেন), অ্যাডমিন প্যানেলে "ডিফল্ট পণ্য ডাটাবেসে আপলোড" চাপুন।
