# Terminal Guide — Terminal komandalar

Ushbu qo‘llanmada terminal bilan ishlash va asosiy komandalar keltirilgan. Misollar Git Bash uchun yozilgan.

## 1. Terminal nima?

**Ta’rif:** Terminal — kompyuter bilan matnli buyruqlar orqali muloqot qilish imkonini beradigan dastur yoki interfeys.

**Vazifasi:** Buyruqlar yordamida fayl va papkalarni boshqarish hamda dasturlarni ishga tushirish imkonini beradi.

**Qachon ishlatiladi:** Grafik oynalar o‘rniga buyruq kiritib ishlash kerak bo‘lganda.

**Misol:**
```bash
pwd
```
## 2. Terminal nima uchun kerak?

**Ta’rif:** Terminal operatsion tizimga buyruqlar yuborish uchun ishlatiladi.

**Vazifasi:** Fayl va papkalarni boshqarish, dasturlarni ishga tushirish va Git buyruqlarini bajarishga yordam beradi.

**Qachon ishlatiladi:** Tez-tez takrorlanadigan ishlarni buyruqlar orqali bajarishda.

**Misol:**
```bash
git status
```
## 3. pwd — joriy joylashuvni ko‘rish

**Ta’rif:** `pwd` terminal hozir qaysi papkada turganini to‘liq manzili bilan ko‘rsatadi.

**Vazifasi:** Joriy ish papkasini aniqlaydi.

**Qachon ishlatiladi:** Buyruqni qaysi papkada bajarishingizni tekshirishda.

**Misol:**
```bash
pwd
```
## 4. ls — fayllarni ko‘rish

**Ta’rif:** `ls` joriy papkadagi fayl va papkalar ro‘yxatini ko‘rsatadi.

**Vazifasi:** Papka ichidagi mavjud elementlarni ko‘rishga yordam beradi.

**Qachon ishlatiladi:** Kerakli fayl yoki papka borligini tekshirishda.

**Misol:**
```bash
ls
```
## 5. cd — papkaga kirish

**Ta’rif:** `cd` ko‘rsatilgan papkaga o‘tadi.

**Vazifasi:** Terminalning joriy joylashuvini o‘zgartiradi.

**Qachon ishlatiladi:** Boshqa papkadagi fayllar bilan ishlashdan oldin.

**Misol:**
```bash
cd documents
```
## 6. cd .. — yuqori papkaga chiqish

**Ta’rif:** `cd ..` joriy papkaning bitta yuqori darajasiga qaytaradi.

**Vazifasi:** Papka ichidan ota papkaga chiqishga yordam beradi.

**Qachon ishlatiladi:** Bir daraja yuqoridagi papkaga qaytish kerak bo‘lganda.

**Misol:**
```bash
cd ..
```
## 7. mkdir — papka yaratish

**Ta’rif:** `mkdir` yangi papka yaratadi.

**Vazifasi:** Fayllarni tartibli saqlash uchun papka hosil qiladi.

**Qachon ishlatiladi:** Loyiha yoki mavzu uchun yangi papka ochishda.

**Misol:**
```bash
mkdir my-folder
```
## 8. touch — fayl yaratish

**Ta’rif:** `touch` Git Bash, macOS va Linux’da yangi bo‘sh fayl yaratadi.

**Vazifasi:** Yangi matnli faylni tez yaratadi.

**Qachon ishlatiladi:** Markdown yoki boshqa bo‘sh faylni terminaldan yaratishda.

**Misol:**
```bash
touch notes.txt
```
## 9. cat — fayl mazmunini ko‘rish

**Ta’rif:** `cat` matnli fayl ichidagi yozuvlarni terminalda chiqaradi.

**Vazifasi:** Faylni tahrirlamasdan uning mazmunini o‘qishga yordam beradi.

**Qachon ishlatiladi:** Matnli fayl ichidagi ma’lumotni tez tekshirishda.

**Misol:**
```bash
cat notes.txt
```
## 10. clear — terminalni tozalash

**Ta’rif:** `clear` terminal oynasidagi avvalgi matnlarni ekrandan tozalaydi; fayllarni o‘chirmaydi.

**Vazifasi:** Terminal oynasini tartibli ko‘rsatadi.

**Qachon ishlatiladi:** Buyruqlar natijasi ko‘payib, oynani tozalash kerak bo‘lganda.

**Misol:**
```bash
clear
```
## 11. cp — nusxa olish

**Ta’rif:** `cp` fayl yoki papkadan nusxa yaratadi.

**Vazifasi:** Asl faylni saqlagan holda uning nusxasini hosil qiladi.

**Qachon ishlatiladi:** Faylning zaxira yoki ikkinchi nusxasi kerak bo‘lganda.

**Misol:**
```bash
cp notes.txt notes-copy.txt
```
## 12. mv — ko‘chirish yoki nomini o‘zgartirish

**Ta’rif:** `mv` fayl yoki papkani boshqa joyga ko‘chiradi yoki nomini o‘zgartiradi.

**Vazifasi:** Fayllar joylashuvini va nomini boshqaradi.

**Qachon ishlatiladi:** Faylni boshqa papkaga o‘tkazish yoki qayta nomlashda.

**Misol:**
```bash
mv old.txt new.txt
```
## 13. rm — fayl o‘chirish

**Ta’rif:** `rm` ko‘rsatilgan faylni o‘chiradi.

**Vazifasi:** Keraksiz faylni terminal orqali olib tashlaydi.

**Qachon ishlatiladi:** Faqat o‘chirish kerakligi aniq bo‘lgan sinov fayllarida.

**Misol:**
```bash
rm notes-copy.txt
```
## 14. git init — repository yaratish

**Ta’rif:** `git init` joriy papkada yangi Git repository boshlaydi.

**Vazifasi:** Loyiha fayllarini Git orqali kuzatishni yoqadi.

**Qachon ishlatiladi:** Yangi loyiha uchun versiyalar tarixini boshlashda.

**Misol:**
```bash
mkdir my-project
cd my-project
git init
```
## 15. git status — Git holatini tekshirish

**Ta’rif:** `git status` repositorydagi yangi, o‘zgargan va stagingga qo‘shilgan fayllarni ko‘rsatadi.

**Vazifasi:** Commit qilinmagan o‘zgarishlarni aniqlashga yordam beradi.

**Qachon ishlatiladi:** Git add yoki commitdan oldin va keyin holatni tekshirishda.

**Misol:**
```bash
git status
```
## Muhim eslatmalar

- Git Bash’da `touch notes.txt` ishlaydi. Windows PowerShell’da bo‘sh fayl yaratish uchun `New-Item notes.txt -ItemType File` buyrug‘idan foydalanish mumkin.
- PowerShell’da `ls` fayllar ro‘yxatini ko‘rsatadigan alias sifatida ishlaydi.
- `rm` faylni o‘chiradi. Mashq paytida faqat o‘zingiz yaratgan va kerak emasligiga ishonch hosil qilgan sinov faylini o‘chiring.
- Ushbu topshiriqda `rm -rf` kabi qaytarish qiyin bo‘lgan buyruqlarni ishlatmang.

## Amaliy mashq

```bash
pwd
mkdir terminal-mashq
cd terminal-mashq
touch notes.txt
ls
cat notes.txt
git init
git status
```

**Xulosa:** Terminal matnli buyruqlar orqali kompyuter bilan ishlashga yordam beradi. Har bir buyruqni bajarishdan oldin qaysi papkada turganingizni `pwd` bilan tekshiring.
