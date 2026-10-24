# Klaviatura sarguzashti

Netlify’da ishlaydigan, o‘zbek tilidagi statik klaviatura mashqlari sayti. O‘quvchi natijalari brauzerda saqlanadi va Netlify Blobs orqali umumiy bazaga sinxronlanadi; o‘qituvchi paneli natijalarni barcha qurilmalardan ko‘rsatadi.

## Netlify sozlamalari

1. GitHub repozitoriyni Netlify’ga ulang. Build command talab qilinmaydi; publish directory `.`.
2. Netlify saytining **Environment variables** bo‘limida `TEACHER_LOGIN` va `TEACHER_PASSWORD` qiymatlarini o‘rnating. Parolni repozitoriyga yozmang.
3. Saytni qayta deploy qiling. Functions va Netlify Blobs deploy’dan keyin ishlaydi.

O‘quvchilarni o‘qituvchi panelida ko‘rish uchun o‘qituvchi ushbu sozlamalardagi login-parol bilan kiradi. Netlify Blobs doimiy umumiy saqlashni ta’minlaydi. HTML faylni kompyuterdan bevosita ochganda bulut sinxronizatsiyasi ishlamaydi; Netlify manzili orqali ochish kerak.

## Fayllar

- `index.html` — o‘yin, darslar, ro‘yxatdan o‘tish va panel.
- `netlify/functions/students.mjs` — o‘quvchi natijalarini saqlash va himoyalangan o‘qituvchi so‘rovlari.
- `netlify.toml` — Netlify build va routing sozlamalari.
