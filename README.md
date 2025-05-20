# 🌍 Country Info App

Aplikasi ini menampilkan informasi negara-negara di dunia menggunakan API dari [REST Countries](https://restcountries.com/). Dibangun dengan Laravel (Backend) dan React Native (Frontend).

---

## ✅ Langkah Install Project

### 🔧 Backend (Laravel)

1. Clone repository:

   ```bash
   git clone https://github.com/username/backend-countryinfo.git
   cd backend-countryinfo
   ```

2. Install dependencies:

   ```bash
   composer install
   ```

3. Copy file `.env`:

   ```bash
   cp .env.example .env
   ```

4. Generate app key:

   ```bash
   php artisan key:generate
   ```

5. Jalankan server:

   ```bash
   php artisan serve
   ```

---

### 📱 Frontend (React Native)

1. Masuk ke folder frontend:

   ```bash
   cd frontend-countryinfo
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Jalankan Metro bundler:

   ```bash
   npx react-native start
   ```

4. Jalankan app (Android):

   ```bash
   npx react-native run-android
   ```

> ⚠️ Jika menggunakan emulator Android, pastikan API Laravel diakses dengan `http://10.0.2.2:{port}`
> Jika menggunakan device fisik, gunakan `ngrok` atau IP lokal sesuai jaringan.

---

## 🚀 Menjalankan Backend dan Frontend

| Komponen     | Perintah                                                     |
| ------------ | ------------------------------------------------------------ |
| Laravel      | `php artisan serve`                                          |
| React Native | `npx react-native start` lalu `npx react-native run-android` |

---

## 🔗 Penjelasan Singkat Endpoint API

| Endpoint                | Method | Deskripsi                                             |
| ----------------------- | ------ | ----------------------------------------------------- |
| `/api/countries`        | `GET`  | Mengambil seluruh data negara dari REST Countries API |
| `/api/countries/{name}` | `GET`  | Mengambil data negara berdasarkan nama tertentu       |

Contoh respons:

```json
[
  {
    "name": "Indonesia",
    "capital": "Jakarta",
    "region": "Asia",
    "flag": "https://flagcdn.com/id.svg"
  }
]
```

---

## 🧪 Screenshot Hasil Testing

### 📬 Postman

![Postman Test](/screenshots/postman-test.png)

### 📲 App

![App Test](/screenshots/app-test.png)

---

## 📌 Catatan

* API publik diambil dari: [https://restcountries.com/v3.1/all](https://restcountries.com/v3.1/all)
* Tidak perlu API key
* Respons berbentuk JSON

---

Jika kamu ingin, saya juga bisa bantu buatkan file `README.md` lengkap dalam format siap commit ke GitHub. Mau sekalian saya bantu buatkan?
