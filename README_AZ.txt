QALA KURSU — YENILENMIS KOD PAKETI

Fayllar:
- index.html — saytın HTML hissəsi
- style.css — görünüş və dizayn
- script.js — giriş, dərs mərhələləri, brauzer sessiyası və API çağırışları
- google_apps_script.gs — Google Sheets ilə işləyən server kodu

VACİB: Bu ZIP kodları hazır vəziyyətdə paketləyir, amma GitHub-a və ya Google Apps Script-ə özü yükləmir.

1) GOOGLE APPS SCRIPT-I YENİLƏMƏK
- Google Sheet-i açın və Extensions / Genişləndirmələr > Apps Script bölməsinə keçin.
- Mövcud server kodunun ehtiyat nüsxəsini saxlayın.
- google_apps_script.gs faylının bütün məzmununu Apps Script redaktoruna köçürün və yadda saxlayın.
- Deploy > Manage deployments > mövcud Web App deployment-in Edit (karandaş) düyməsi > New version > Deploy seçin.
- Mövcud deployment URL-sini qoruyun. Yeni URL yaranarsa, script.js faylındakı SCRIPT_URL sətrini də dəyişmək lazımdır.
- Web App icazələrinin sizin istifadə ssenarinizə uyğun olduğuna əmin olun.

2) GITHUB SAYTINI YENİLƏMƏK
- index.html, script.js və style.css fayllarını GitHub repozitoriyasındakı uyğun fayllarla əvəz edin.
- Commit edin və saytın yenilənməsini gözləyin.
- Sonra brauzerdə sərt yeniləmə edin (Ctrl+F5).

DƏYİŞİKLİKLƏR
- Davamiyyət və statistika yazılışında təkrar sətirlərin qarşısını almaq üçün tarix + fənn + şagird açarı tətbiq edilir.
- Serverdə paralel/ardıcıl yazılışlar üçün LockService istifadə olunur.
- Valideyn məlumatlarının oxunmasında sütun yoxlamaları və daha dəqiq ad uyğunluğu əlavə olunub.
- Tamamla düyməsində təkrar kliklər bloklanır; uğursuz yazılışda mərhələ irəli keçmir.
- Dərs mərhələləri arasında geri düymələri əlavə olunub.
- Müəllim/valideyn sessiyası və dərs formalarının daxil edilmiş dəyərləri localStorage-da saxlanır; Çıxış düyməsi sessiyanı silir.

QEYD
- Kod sintaksisi yoxlanılıb, lakin real Google Sheet və canlı Apps Script deployment-ə qoşulub tam inteqrasiya sınağı aparılmayıb.
- Google Sheet-də əvvəldən yaranmış təkrar sətirlər avtomatik silinmir; yeni yazılışlar üçün təkrarın qarşısı alınır.
- Sessiya giriş parolunu saxlamır, lakin müəllim/valideyn profilini və formadakı daxil edilmiş məlumatları həmin brauzerin localStorage yaddaşında saxlayır. Ortaq kompüterdə istifadə etdikdən sonra Çıxış düyməsini basın.
