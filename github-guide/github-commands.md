# GitHub Guide — GitHub va remote komandalar

Ushbu qo‘llanma GitHub platformasi, repositorylar va lokal hamda masofaviy repository o‘rtasidagi ish tartibini tushuntiradi.

## 1. GitHub nima?

**Ta’rif:** GitHub — Git repositorylarini internetda saqlash, ulashish, ko‘rib chiqish va loyihalar ustida hamkorlik qilish platformasi.

**Vazifasi:** Loyihalarni masofaviy saqlash va boshqalar bilan hamkorlik qilish imkonini beradi.

**Qachon ishlatiladi:** Loyihani internetga joylashtirish yoki boshqalarga ko‘rsatishda.

**Misol:**
```bash
https://github.com/
```
## 2. Git va GitHub farqi

**Ta’rif:** Git — versiya nazorati tizimi; GitHub esa Git repositorylarini onlayn saqlash va boshqarish xizmatidir.

**Vazifasi:** Git o‘zgarish tarixini boshqaradi, GitHub esa repositoryni internetda ulashishga yordam beradi.

**Qachon ishlatiladi:** Lokal ish bilan onlayn repository vazifalarini farqlashda.

**Misol:**
```bash
git --version
```
## 3. GitHub account nima?

**Ta’rif:** GitHub account — foydalanuvchining GitHub platformasidagi shaxsiy hisobi.

**Vazifasi:** Repository yaratish, loyihalarni saqlash va platforma imkoniyatlaridan foydalanish uchun kerak.

**Qachon ishlatiladi:** GitHub’da loyiha ochish yoki o‘z loyihalaringizni boshqarishda.

**Misol:**
```bash
https://github.com/signup
```
## 4. Repository nima?

**Ta’rif:** GitHub repository — loyiha fayllari, commitlar, branchlar va boshqa loyiha ma’lumotlari saqlanadigan masofaviy ombor.

**Vazifasi:** Loyiha nusxasini onlayn saqlaydi va hamkorlikka imkon beradi.

**Qachon ishlatiladi:** Loyiha fayllarini internetda saqlash yoki ulashishda.

**Misol:**
```bash
git clone https://github.com/USERNAME/REPOSITORY.git
```
## 5. Public va Private repository farqi

**Ta’rif:** Public repository hammaga ko‘rinadi; private repository esa faqat egasi va ruxsat berilgan foydalanuvchilarga ko‘rinadi.

**Vazifasi:** Loyiha kimlarga ko‘rinishini boshqaradi.

**Qachon ishlatiladi:** Loyihani ochiq ko‘rsatish yoki faqat tanlangan odamlarga berish kerak bo‘lganda.

**Misol:**
```bash
GitHub’da repository yaratishda Public yoki Private ni tanlash.
```
## 6. Remote nima?

**Ta’rif:** Remote — lokal Git repository bilan bog‘langan masofaviy repository manzili.

**Vazifasi:** Kompyuterdagi repository va GitHub’dagi nusxa o‘rtasidagi aloqani belgilaydi.

**Qachon ishlatiladi:** Lokal loyihani GitHub bilan bog‘lashda.

**Misol:**
```bash
git remote -v
```
## 7. git remote add

**Ta’rif:** Mavjud lokal repositoryga remote manzil qo‘shadi.

**Vazifasi:** `origin` nomi bilan GitHub repository manzilini saqlaydi.

**Qachon ishlatiladi:** Lokal repositoryni GitHub’dagi yangi repositoryga ulashda.

**Misol:**
```bash
git remote add origin https://github.com/USERNAME/REPOSITORY.git
```
## 8. git remote -v

**Ta’rif:** Ulangan remote repositorylarning fetch va push manzillarini ko‘rsatadi.

**Vazifasi:** Remote to‘g‘ri ulanganini tekshiradi.

**Qachon ishlatiladi:** Push yoki pull qilishdan oldin manzilni tekshirishda.

**Misol:**
```bash
git remote -v
```
## 9. git push

**Ta’rif:** Lokal commitlarni remote repositoryga yuboradi.

**Vazifasi:** Kompyuterdagi o‘zgarishlarni GitHub’da ko‘rinadigan qiladi.

**Qachon ishlatiladi:** Commitlar tayyor bo‘lgach GitHub’ga yuborishda.

**Misol:**
```bash
git push -u origin main
```
## 10. git pull

**Ta’rif:** Remote repositorydagi yangilanishlarni olib keladi va joriy branchga birlashtiradi.

**Vazifasi:** Lokal repositoryni masofadagi yangilanishlar bilan moslaydi.

**Qachon ishlatiladi:** Boshqa joyda kiritilgan o‘zgarishlarni olishda.

**Misol:**
```bash
git pull origin main
```
## 11. git clone

**Ta’rif:** Masofaviy repository nusxasini kompyuterga yuklab, lokal Git repository yaratadi.

**Vazifasi:** Mavjud GitHub loyihasi bilan kompyuterda ishlashni boshlaydi.

**Qachon ishlatiladi:** Boshqa repositoryni o‘z kompyuteringizda ochmoqchi bo‘lsangiz.

**Misol:**
```bash
git clone https://github.com/USERNAME/REPOSITORY.git
```
## 12. GitHub’da branch nima?

**Ta’rif:** Branch — repository ichidagi alohida ish yo‘nalishi.

**Vazifasi:** Asosiy branchni darhol o‘zgartirmasdan alohida vazifada ishlashga yordam beradi.

**Qachon ishlatiladi:** Yangi funksiya yoki hujjatni alohida tayyorlashda.

**Misol:**
```bash
git switch -c new-feature
```
## 13. GitHub’da commit nima?

**Ta’rif:** Commit — repository tarixidagi saqlangan o‘zgarishlar to‘plami.

**Vazifasi:** O‘zgarishlarning qachon va qanday izoh bilan saqlanganini ko‘rsatadi.

**Qachon ishlatiladi:** Loyiha tarixini ko‘rish yoki o‘zgarish sababini aniqlashda.

**Misol:**
```bash
git log --oneline
```
## 14. GitHub’da faylni tahrirlash

**Ta’rif:** GitHub repository sahifasida faylni ochib, Edit orqali matnni o‘zgartirish va Commit changes orqali saqlash mumkin.

**Vazifasi:** Kichik o‘zgarishlarni brauzer orqali kiritishga yordam beradi.

**Qachon ishlatiladi:** Kompyuterda Git ishlatmasdan kichik matnli tuzatish kiritishda.

**Misol:**
```bash
Repository → fayl → Edit → matnni o‘zgartirish → Commit changes.
```
## 15. GitHub’da branchni o‘chirish

**Ta’rif:** Repository’ning Branches sahifasidan branchni o‘chirish mumkin; remote branch terminaldan ham o‘chiriladi.

**Vazifasi:** Ishi tugagan remote branchlarni tartibga keltiradi.

**Qachon ishlatiladi:** Branchdagi ish kerakli branchga birlashtirilgandan keyin.

**Misol:**
```bash
git push origin --delete branch-name
```
