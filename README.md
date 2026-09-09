<div align="center">

<img src="banner.jpg" alt="DybooAm" width="736">

# DybooAm

**Alight Motion tool — CLI only**

</div>

## Fitur

- Magic link login — cukup email, tanpa password
- Verifikasi link dari inbox
- Refresh token dari sesi tersimpan
- Satu sumber logika (`lib/auth.js`), CLI tipis di atasnya

## Persyaratan

- Node.js 18+
- Koneksi internet

## Cara pakai

```bash
npm install
node index.js
```

| Menu | Fungsi |
|------|--------|
| `1` | kirim magic link ke email |
| `2` | verifikasi link dari email |
| `3` | refresh token dari sesi tersimpan |
| `4` | lihat daftar sesi |

Sesi tersimpan di `sessions.json` (lokal, jangan dibagikan).

## Termux

```bash
pkg install nodejs -y
git clone https://github.com/ZhuxinScript/beriberipatapim
cd beriberipatapim
npm install
node index.js
```

## Test

```bash
npm test
```

## Struktur

```
index.js      CLI
lib/auth.js   logika inti (link, verify, refresh, extractCode)
test.js       self-check extractCode
```

## Disclaimer

Proyek riset independen, tidak berafiliasi dengan Alight Creative / Google.
Gunakan atas risiko sendiri.
