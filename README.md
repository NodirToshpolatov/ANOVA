ANOVA
Anova bu statistic tahlillardan biri bo'lib , u bir nechta guruhlar orasida sezilarli farq bor yoqligini tekshirish uchun ishlatilinadi. Anova guruhlar orasidagi dispersiyalarni tahlil qilib ular orasidagi farq tasodifiy yoki biror o'zgaruvchiga bog'liq ekanligini tekshiradi.
Anova ham null va alternative gipotezalarga asoslangan tahlildir. Javob sifatida chiqqan oxirgi p qiymat 0.05 dan katta bo'lsa null gippoteza aks holda alternative gipoteza o'z tasdig'ini topadi. Odatda null gipoteza guruhlar orasida farq yo'qligini alternative gipoteza esa guruhlar orasida farq borligini anglatadi. Gipotezadan guruhlar orasidagi farq qanchalik kuchli yoki kamliligini aytib bolmaydi. Anova faqat guruhlarning o'rtacha qiymatlarini orasida farq bor yoki yo'qligini ko'rsatib beradi holos. 
Anovani turlari
ONE-WAY anova
One-way anova faqat bitta o'zgaruvchi yoki faktor yuzasidan bir nechta guruhlarni bir-biri bilan taqqoslaydi.Misol uchun bizda 3 ta guruh bo'lsin. Ular o'qitish tizimi uchun 3 xil tizimni(An'anaviy,onlayn,aralash) qo'llashi bilan farqlansin. Bunda bizda null gipoteza guruhdagi bolalar qo'llayotgan tizim orasida hech qanday farq yo'qligini ilgari suradi. Alternativ esa buni aksini.
ONE-WAY anovani hisoblash
Bizda malumotlar tizimlar bo'yicha erishilgan ortacha test natijalarini
tashkil qilsin
Group A (An'anaviy): [85, 88, 90, 87, 86]
Group B (Onlayn): [78, 75, 80, 77, 79]
Group C (Aralash): [92, 94, 90, 91, 93]
1-QADAM. Ona-way anova ni hisoblashda eng birich qilinadigan ish bu umumiy o'rtacha qiymatni hisoblashdir.
Total Sum=85+88+90+87+86+78+75+80+77+79+92+94+90+91+93=1285
2-QADAM. Guruhlar o'rtacha qiymatlarini hisoblash.
Group A (An'anaviy):
X‾A​=85+88+90+87+86​=87.2
Group B (Onlayn):
X‾B​=78+75+80+77+79​=77.8
Group C (Aralash):
X‾C=92+94+90+91+93​=92
3-QADAM. Guruhlar o'rtasidagi variatsiya SSB (sum of squares between) hisoblanadi. Bunda har bir guruhning o'rtacha qiymatlari va umumiy o'rtacha qiymat orasidagi kvadrat farqlarni hisoblash kerak, va har bir guruhdagi kuzatuvlar soniga ko'paytiriladi.
Hisoblaymiz:
SSB = 5(87.2–85.67)² + 5(77.8–85.67)² + 5(92–85.67)² = 5(1.53)² + 5(-7.87)²+ 5(6.33)² = 5(2.34) + 5(61.93) + 5(40.07)= 11.7 + 309.65 + 200.35 = 521.7
4-QADAM. Guruh ichidagi variatsiya SSW (sum of squares within) har bir guruh ichidagi qiymatlar va guruhning o'rtacha qiymati orasidagi kvadrat farqlarni yig'ish orqali hisoblanadi.
Group A:
SSW_A = (85–87.2)² + (88–87.2)² + (90–87.2)² + (87–87.2)² + (86–87.2)²
SSW_A = 4.84 + 0.64 + 7.84 + 0.04 + 1.44 = 14.8
Group B:
SSW_B = (78–77.8)² + (75–77.8)² + (80–77.8)² + (77–77.8)² + (79–77.8)²
SSW_B = 0.04 + 7.84 + 4.84 + 0.64 + 1.44 = 14.8
Group C:
SSW_C = (92–92)² + (94–92)² + (90–92)² + (91–92)² + (93–92)²
SSW_C = 0 + 4 + 4 + 1 + 1 = 10
Umumiy SSW:
SSW = 14.8 + 14.8 + 10 = 39.6
5-QADAM. Erkinlik darajalarini (df) hisoblash
Erkinlik darajalari ANOVA tahlilining muhim qismi bo'lib, ular F-statistikani hisoblash uchun ishlatiladi.
Guruhlar o'rtasidagi erkinlik darajasi (df_between):
df_{between} = k - 1 = 3–1 = 2
Bu yerda (k) - guruhlar soni.
Guruh ichidagi erkinlik darajasi (df_within):
df_{within} = N - k = 15–3 = 12
Bu yerda (N) - barcha kuzatuvlar soni.
6-QADAM.F-statistikani hisoblash. F-statistik qiymatni hisoblash uchun guruhlar o'rtasidagi va guruh ichidagi dispersiyalarni taqqoslaymiz.
 SSB bo'yicha o'rtacha kvadrat (MSB):
MSB = \frac{SSB}{df_{between}} = \frac{521.7}{2} = 260.85
SSW bo'yicha o'rtacha kvadrat (MSW):
MSW = \frac{SSW}{df_{within}} = \frac{39.6}{12} = 3.3
F-statistika:
\[
F = \frac{MSB}{MSW} = \frac{260.85}{3.3} = 79.05
\]
Endi buni nusxalashingiz mumkin!
