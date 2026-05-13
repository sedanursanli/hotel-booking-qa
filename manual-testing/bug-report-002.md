# Bug Report

---

## Bug ID
BUG-002

---

## Bug Title
Sistem aynı oda numarası ile duplicate oda oluşturulmasına izin veriyor.

---

## Module
Admin

---

## Environment
- Browser: Google Chrome
- OS: Windows 11
- Environment: Test Environment

---

## Severity
Medium

---

## Priority
Medium

---

## Preconditions
Admin kullanıcı sisteme giriş yapmış olmalıdır.

---

## Steps to Reproduce
1. Admin paneline giriş yap.
2. Rooms alanına git.
3. Sistemde mevcut olan bir oda ile aynı bilgileri gir.
4. "Create" butonuna tıkla.

---

## Test Data
- Room #: 101
- Type: Single
- Accessible: true
- Price: 100
- Room Details: TV, WiFi, Safe

---

## Expected Result
Sistem aynı oda numarası ile yeni oda oluşturulmasına izin vermemelidir.

---

## Actual Result
Sistem aynı oda numarası ile yeni oda oluşturulmasına izin verdi.

---

## Attachment / Screenshot

![Duplicate Room Bug](screenshots/duplicate-room-bug.png)

---

## Reported By
Seda Nur Sanlı

---

## Report Date
12.05.2026

---

## Status
Open