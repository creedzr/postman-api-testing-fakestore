🛒 FakeStore API Testing – Postman
Manual API test suite untuk FakeStore API menggunakan Postman.

✅ Endpoint yang Diuji
MethodEndpointSkenarioGET/productsGet all products, single product (valid & invalid id)GET/usersGet single user by idPOST/productsAdd product (valid, empty body)POST/auth/loginLogin valid & invalid credentialPUT/products/{id}Update full product (valid id, invalid id, empty body)PATCH/products/{id}Update sebagian field (title, price, category, invalid id)DELETE/products/{id}Delete product (valid & invalid id)DELETE/users/{id}Delete userDELETE/carts/{id}Delete cart
Total: 20 test case

📋 Dokumentasi Test Case
Dokumentasi lengkap test case (scenario, test data, expected result, actual result, status) tersedia di spreadsheet berikut:
🔗 API Manual Testcase – Google Sheets

🚀 Cara Import Collection ke Postman

Clone atau download repo ini
Buka Postman
Klik Import (pojok kiri atas)
Pilih file Fakestore_Api_Testing_postman_collection.json
Collection siap digunakan


📁 Struktur Folder
postman-api-testing-fakestore/
├── Fakestore_Api_Testing_postman_collection.json   # Postman collection
└── README.md

🛠️ Tools

Postman
FakeStore API (https://fakestoreapi.com/)
Google Sheets (https://docs.google.com/spreadsheets/d/1sbA2lhFqs_Zop7BG_-snsm6_4MQjbKzzNWQ9idXXFAg/edit?gid=920238044#gid=920238044)


📝 Catatan

TC-GET-003 (/products/999) berstatus FAIL — API mengembalikan response 200 OK dengan body kosong, bukan 404 Not Found sesuai ekspektasi. Ini merupakan bug pada FakeStore API.
Project ini merupakan manual API testing, bukan automation.
