# Git Guide — Git asoslari va komandalar

Ushbu qo‘llanma Git asoslarini o‘rganish uchun tayyorlandi. Har bir bo‘limda ta’rif, vazifa, ishlatilish holati va amaliy misol berilgan.

## 1. Git nima?

**Ta’rif:** Git — fayllardagi o‘zgarishlarni kuzatish va loyiha versiyalarini boshqarish uchun ishlatiladigan taqsimlangan versiya nazorati tizimi.

**Vazifasi:** Loyiha tarixini saqlash va oldingi holatlarga qaytish imkonini beradi.

**Qachon ishlatiladi:** Dastur yoki hujjatlar ustida ishlaganda o‘zgarishlarni nazorat qilish kerak bo‘lsa.

**Misol:**
```bash
git --version
```
## 2. Git nima uchun kerak?

**Ta’rif:** Git fayllar tarixini va ularga kiritilgan o‘zgarishlarni saqlaydi.

**Vazifasi:** Xatolarni aniqlash, oldingi holatni ko‘rish, branchlarda alohida ishlash va hamkorlik qilishga yordam beradi.

**Qachon ishlatiladi:** Loyiha rivojlanishini bosqichma-bosqich saqlashda.

**Misol:**
```bash
git status
```
## 3. Repository nima?

**Ta’rif:** Repository — loyiha fayllari va Git tarixini saqlaydigan ombor.

**Vazifasi:** Fayllar, commitlar va branchlarni bir joyda boshqaradi.

**Qachon ishlatiladi:** Git bilan kuzatiladigan yangi loyiha boshlaganda yoki mavjud loyihani ochganda.

**Misol:**
```bash
git init
```
## 4. Global va Local konfiguratsiya farqi

**Ta’rif:** Global konfiguratsiya foydalanuvchining barcha repositorylari uchun, local konfiguratsiya esa faqat joriy repository uchun amal qiladi.

**Vazifasi:** Commit muallifining ismi va emailini belgilaydi. Local qiymat shu repository ichida global qiymatdan ustun turadi.

**Qachon ishlatiladi:** Git’ni ilk sozlashda yoki alohida loyiha uchun boshqa muallif ma’lumotini ishlatishda.

**Misol:**
```bash
git config --global user.name "Ism Familiya"
git config --global user.email "email@example.com"
git config user.name
```
## 5. git init

**Ta’rif:** Joriy papkada yangi Git repository boshlaydi.

**Vazifasi:** Papkani Git tomonidan kuzatiladigan loyiha qiladi.

**Qachon ishlatiladi:** Yangi loyiha uchun versiyalar tarixini boshlashda.

**Misol:**
```bash
mkdir my-project
cd my-project
git init
```
## 6. git status

**Ta’rif:** Repository’ning joriy holatini ko‘rsatadi.

**Vazifasi:** Yangi, o‘zgargan, stagingga qo‘shilgan va commit qilinmagan fayllarni bildiradi.

**Qachon ishlatiladi:** Fayllarni add yoki commit qilishdan oldin holatni tekshirishda.

**Misol:**
```bash
git status
```
## 7. git add

**Ta’rif:** Tanlangan fayldagi o‘zgarishlarni staging area’ga qo‘shadi.

**Vazifasi:** Keyingi commitga qaysi o‘zgarishlar kiritilishini tanlaydi.

**Qachon ishlatiladi:** Yangi yoki o‘zgartirilgan faylni commitga tayyorlashda.

**Misol:**
```bash
git add README.md
git add .
```
## 8. git commit

**Ta’rif:** Staging area’dagi o‘zgarishlarni repository tarixida yangi commit sifatida saqlaydi.

**Vazifasi:** Loyihaning muayyan holatini va unga berilgan izohni tarixga yozadi.

**Qachon ishlatiladi:** Mantiqan tugallangan ish bosqichini saqlashda.

**Misol:**
```bash
git add README.md
git commit -m "Add project description"
```
## 9. git log

**Ta’rif:** Repository’dagi commitlar tarixini ko‘rsatadi.

**Vazifasi:** Commit muallifi, sanasi va izohlarini ko‘rishga yordam beradi.

**Qachon ishlatiladi:** Oldingi ishlar yoki commit izohlarini tekshirishda.

**Misol:**
```bash
git log --oneline
```
## 10. git branch

**Ta’rif:** Branch — asosiy ish tarixidan ajratilgan alohida ish yo‘nalishi. `git branch` branchlarni ko‘rsatadi yoki yangisini yaratadi.

**Vazifasi:** Asosiy branchni darhol o‘zgartirmasdan yangi vazifa ustida ishlashga yordam beradi.

**Qachon ishlatiladi:** Yangi funksiya yoki mavzuni alohida ishlab chiqishda.

**Misol:**
```bash
git branch
git branch new-feature
```
## 11. git switch

**Ta’rif:** Mavjud branchga o‘tadi; `-c` parametri yangi branch yaratib unga o‘tkazadi.

**Vazifasi:** Turli ish yo‘nalishlari o‘rtasida almashadi.

**Qachon ishlatiladi:** Boshqa branchda ishlashni boshlash yoki yangi branch yaratishda.

**Misol:**
```bash
git switch main
git switch -c new-feature
```
## 12. git merge

**Ta’rif:** Boshqa branchdagi o‘zgarishlarni joriy branchga birlashtiradi.

**Vazifasi:** Alohida ishlab chiqilgan ishlarni bitta branch tarixiga qo‘shadi.

**Qachon ishlatiladi:** Branchdagi ish tugab, uni asosiy branchga birlashtirish kerak bo‘lganda.

**Misol:**
```bash
git switch main
git merge new-feature
```
## 13. git branch -d

**Ta’rif:** Lokal branchni o‘chiradi. Git odatda birlashtirilmagan ish bo‘lsa ogohlantiradi.

**Vazifasi:** Ishi tugagan va birlashtirilgan branchlarni tartibga keltiradi.

**Qachon ishlatiladi:** Branchdagi ish kerakli branchga merge qilingandan keyin.

**Misol:**
```bash
git switch main
git branch -d new-feature
```
