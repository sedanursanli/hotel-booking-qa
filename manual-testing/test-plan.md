# Test Plan – Restful Booker Platform Demo

---

# 1. Test Objectives (Test Hedefleri)

Bu test sürecinin amacı, Restful Booker Platform Demo uygulamasının temel fonksiyonlarının doğru, stabil ve kullanıcı beklentilerine uygun şekilde çalıştığını doğrulamaktır.

Test süreci boyunca aşağıdaki hedeflere odaklanılacaktır:

- Rezervasyon işlemlerinin doğru çalıştığını doğrulamak
- Form validasyonlarını kontrol etmek
- Kullanıcı deneyimini etkileyebilecek hataları tespit etmek
- Farklı veri girişlerinde sistem davranışlarını gözlemlemek
- Kritik kullanıcı akışlarının stabil çalıştığını doğrulamak

---

# 2. Scope (Kapsam)

## 2.1 In-Scope (Kapsam Dahili)

Aşağıdaki modüller manuel olarak test edilecektir:

- Booking işlemleri
- Contact form işlemleri
- Admin panel room management işlemleri
- Tarih seçim kontrolleri
- Form validation kontrolleri
- Total Price hesaplama kontrolleri
- UI/UX kontrolleri
- Smoke test senaryoları

---

## 2.2 Out-of-Scope (Kapsam Dışı)

Aşağıdaki test türleri bu çalışma kapsamında yer almamaktadır:

- API Testing
- Automation Testing
- Performance Testing
- Security Testing
- Database Testing

---

# 3. Test Approach (Test Yaklaşımı)

Test sürecinde aşağıdaki test türleri uygulanacaktır:

| Test Type | Açıklama |
|---|---|
| Functional Testing | Sistem fonksiyonlarının beklenen şekilde çalıştığının kontrol edilmesi |
| Smoke Testing | Temel sistem akışlarının hızlı doğrulama testi |
| Negative Testing | Geçersiz veri girişlerine karşı sistem davranışının kontrol edilmesi |
| Exploratory Testing | Sistemin manuel keşif yöntemiyle test edilmesi |
| UI Testing | Kullanıcı arayüzü davranışlarının kontrol edilmesi |

Testler manuel olarak gerçekleştirilecektir.

---

# 4. Test Environment (Test Ortamı)

| Alan | Detay |
|---|---|
| Application | Restful Booker Platform Demo |
| Test Type | Manual Testing |
| Browser | Google Chrome |
| Operating System | Windows 11 |
| Device | Desktop |

---

# 5. Entry Criteria (Giriş Kriterleri)

Test sürecinin başlatılabilmesi için aşağıdaki koşullar sağlanmalıdır:

- Test ortamı erişilebilir olmalıdır
- Uygulama stabil şekilde çalışmalıdır
- Test senaryoları hazırlanmış olmalıdır

---

# 6. Exit Criteria (Çıkış Kriterleri)

Test sürecinin tamamlanabilmesi için aşağıdaki koşullar sağlanmalıdır:

- Planlanan test senaryoları çalıştırılmış olmalıdır
- Kritik seviyedeki hatalar raporlanmış olmalıdır
- Smoke test senaryoları tamamlanmış olmalıdır

---

# 7. Risks (Riskler)

Test süreci boyunca karşılaşılabilecek olası riskler:

- Demo ortamının zaman zaman kararsız çalışması
- Tarih bazlı işlemlerde beklenmeyen sistem davranışları
- Aynı anda oluşabilecek rezervasyon çakışmaları
- Tarih veya oda değişimlerinde Total Price alanının yanlış hesaplanabilmesi
- UI tarafında tarayıcı kaynaklı farklılıklar oluşabilmesi

---

# 8. Test Deliverables (Test Çıktıları)

Test süreci sonunda aşağıdaki dokümanlar oluşturulacaktır:

- Test Plan
- Test Scenarios
- Test Cases
- Smoke Test Checklist
- Bug Report Documents
