# State Transition Testing

## Purpose

Bu doküman, rezervasyon akışı üzerinde temel bir State Transition Testing yaklaşımını göstermek amacıyla hazırlanmıştır.

---

# States

| State | Description |
|---|---|
| Available | Oda rezervasyona uygundur. |
| Reserved | Oda için aktif rezervasyon oluşturulmuştur. |


---

# Valid Transitions

| Current State | Action | Next State |
|---|---|---|
| Available | Create Reservation | Reserved |


---

# Invalid Transitions

| Current State | Invalid Action | Expected Result |
|---|---|---|
| Reserved | Create Another Reservation (same dates) | Sistem çakışan rezervasyonu engellemelidir. |
| Available | Create Reservation with past date | Sistem geçmiş tarih rezervasyonunu reddetmelidir. |

---

# State Transition Notes

- Bir oda aynı anda yalnızca bir aktif rezervasyona sahip olmalıdır.
- Geçersiz state geçişlerinde sistem uygun hata yönetimi sağlamalıdır.
- Rezervasyon durumu değişiklikleri business rule’lara uygun şekilde yönetilmelidir.
- Cancelled state bu platformda desteklenmemektedir. State transition çalışması yalnızca uygulamada test edilebilen geçişler üzerinden hazırlanmıştır.