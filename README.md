# 🛒 FakeStore API Testing – Postman

Manual API test suite untuk **[FakeStore API](https://fakestoreapi.com/)** menggunakan Postman.

---

## ✅ Endpoint yang Diuji

| Method | Endpoint | Skenario |
|---|---|---|
| GET | /products | Get all products, single product (valid & invalid id) |
| GET | /users | Get single user by id |
| POST | /products | Add product (valid, empty body) |
| POST | /auth/login | Login valid & invalid credential |
| PUT | /products/{id} | Update full product (valid id, invalid id, empty body) |
| PATCH | /products/{id} | Update sebagian field (title, price, category, invalid id) |
| DELETE | /products/{id} | Delete product (valid & invalid id) |
| DELETE | /users/{id} | Delete user |
| DELETE | /carts/{id} | Delete cart |

**Total: 20 test case**

---

## 📋 Dokumentasi Test Case

Dokumentasi lengkap test case (scenario, test data, expected result, actual result, status) tersedia di spreadsheet berikut:

🔗 [API Manual Testcase – Google Sheets](https://docs.google.com/spreadsheets/d/1sbA2lhFqs_Zop7BG_-snsm6_4MQjbKzzNWQ9idXXFAg/edit?gid=0#gid=0)

---

## 🚀 Cara Import Collection ke Postman

1. Clone atau download repo ini
2. Buka **Postman**
3. Klik **Import** (pojok kiri atas)
4. Pilih file `Fakestore_Api_Testing_postman_collection.json`
5. Collection siap digunakan

---

## 📁 Struktur Folder

```
postman-api-testing-fakestore/
├── Fakestore_Api_Testing_postman_collection.json   # Postman collection
└── README.md
```

---

## 🛠️ Tools

- **Postman**
- **FakeStore API** (https://fakestoreapi.com/)
- **Google Sheets** (dokumentasi test case)

---

## 📝 Catatan

- TC-GET-003 (`/products/999`) berstatus **FAIL** — API mengembalikan response 200 OK dengan body kosong, bukan 404 Not Found sesuai ekspektasi. Ini merupakan bug pada FakeStore API.
- Project ini merupakan manual API testing, bukan automation.
