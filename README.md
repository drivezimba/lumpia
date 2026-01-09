# Lumpia Library (GASLibv3) - Google Apps Script Telegram Bot

Repositori ini berisi struktur file untuk membangun library Telegram Bot di Google Apps Script menggunakan framework **lumpia (GASLibv3)**.

## 📁 Struktur File Library
Library ini terdiri dari **11 file** inti yang bekerja secara modular:

| No | Nama File | Fungsi Utama |
|---|---|---|
| 01 | `00 version.js` | Informasi rilis dan ID basis library. |
| 02 | `10 helper.js` | Fungsi utilitas (clearHTML, random, dll). |
| 03 | `15 markup.js` | Mengelola pembuatan Keyboard & Inline Keyboard. |
| 04 | `20 composer.js` | Middleware handler untuk menangkap command dan pesan. |
| 05 | `20 event.js` | Sistem event emitter untuk menangani alur library. |
| 06 | `30 context.js` | Menangani objek `ctx` (ctx.reply, ctx.answerCallbackQuery, dll). |
| 07 | `50 client.js` | Mesin pengirim data (JSON/Blob) ke API Telegram. |
| 08 | `60 telegram.js` | Koleksi lengkap metode API Telegram. |
| 09 | `70 fetch.js` | Fungsi dasar untuk HTTP request (UrlFetchApp). |
| 10 | `80 userdb.js` | Database sederhana berbasis PropertiesService. |
| 11 | `90 main.js` | Entry point utama: `new lumpia.init(token)`. |

---

## 🚀 Cara Penggunaan

### 1. Inisialisasi
Pastikan Anda sudah menambahkan Library ke proyek Anda dengan Identifier `lumpia`.

```javascript
const token = 'TOKEN_BOT_ANDA';
const bot = new lumpia.init(token);
