# Edge Case Testing

## Purpose

Bu doküman, rezervasyon sistemi üzerinde test edilen önemli edge case senaryolarını içermektedir.

---

# Edge Case Scenarios

| Edge Case | Description | Expected Behavior |
|---|---|---|
| Leap Year Date | Rezervasyon tarihi olarak artık yıl tarihi girilmesi | Sistem geçerli tarihi kabul etmelidir. |
| Same Day Booking | Check-in ve check-out tarihlerinin aynı olması | Sistem business rule’a göre işlem yapmalıdır. |
| Past Date Reservation | Geçmiş tarih ile rezervasyon oluşturulması | Sistem rezervasyonu reddetmelidir. |
| Extremely Far Future Date | Çok ileri tarihli rezervasyon oluşturulması | Sistem business rule’a göre işlem yapmalıdır. |
| Whitespace Input | Sadece boşluk karakteri içeren giriş yapılması | Sistem girdiyi boş giriş olarak değerlendirmelidir. |
| Duplicate Room Number | Aynı oda numarasının tekrar oluşturulması | Sistem duplicate kayıt oluşumunu engellemelidir. |
| Negative Room Number | Negatif oda numarası girilmesi | Sistem negatif değerleri reddetmelidir. |
| Decimal Room Number | Ondalıklı oda numarası girilmesi | Sistem yalnızca tam sayı kabul etmelidir. |
| Invalid Calendar Date | Geçersiz tarih girilmesi (31 February) | Sistem geçersiz tarihi reddetmelidir. |
| Extremely Long Phone Number | Maksimum sınırı aşan telefon numarası girilmesi | Sistem girdiyi reddetmelidir. |

---

# Notes

- Edge case testleri, standart kullanıcı davranışlarının dışındaki senaryoları doğrulamak amacıyla hazırlanmıştır.
- Bu testler sistemin beklenmeyen girdilere karşı dayanıklılığını değerlendirmeye yardımcı olur.
- Edge case senaryoları exploratory testing sırasında tespit edilen gerçek bug’larla ilişkilendirilmiştir.