# State Transition Testing

## Purpose

Bu doküman, rezervasyon akışı üzerinde temel bir State Transition Testing yaklaşımını göstermek amacıyla hazırlanmıştır.

---

# States

| State | Description |
|---|---|
| Available | Oda rezervasyona uygundur. |
| Reserved | Oda için aktif rezervasyon bulunmaktadır. |
| Cancelled | Rezervasyon iptal edilmiştir. |

---

# Valid Transitions

| Current State | Action | Next State |
|---|---|---|
| Available | Create Reservation | Reserved |
| Reserved | Cancel Reservation | Cancelled |
| Cancelled | Rebook Room | Reserved |

---

# Invalid Transitions

| Current State | Invalid Action | Expected Result |
|---|---|---|
| Reserved | Create Another Reservation | Sistem aynı oda için tekrar rezervasyon oluşturulmasını engellemelidir. |
| Cancelled | Cancel Reservation Again | Sistem hata mesajı göstermelidir. |
| Available | Cancel Reservation | Sistem geçersiz işlem yapılmasını engellemelidir. |

---

# State Transition Notes

- Bir oda aynı anda yalnızca bir aktif rezervasyona sahip olmalıdır.
- İptal edilmiş rezervasyon tekrar aktif hale getirilebilmelidir.
- Geçersiz state geçişlerinde sistem uygun hata yönetimi sağlamalıdır.
- Rezervasyon durumu değişiklikleri business rule’lara uygun şekilde yönetilmelidir.