# Tugas 6 - VPS Provisioning

## Tujuan
Melakukan inisialisasi VPS agar siap digunakan dengan:
- Update & upgrade sistem
- Setup swap memory 2GB
- Verifikasi hasil setup

---

## Langkah-langkah

### 1. Login ke VPS
Melakukan SSH ke server VPS.

![SSH Login](1-ssh-login.png)

---

### 2. Update Sistem
Menjalankan update package list.

![APT Update](2-apt-update.png)

---

### 3. Upgrade Sistem
Melakukan upgrade package.

![APT Upgrade](3-apt-upgrade.png)

---

### 4. Setup Swap Memory 2GB
Melakukan:
- fallocate
- chmod
- mkswap
- swapon

![Swap Setup](4-swap-setup.png)

---

### 5. Konfigurasi Permanent Swap
Menambahkan swap ke file `/etc/fstab`.

![FSTAB](5-fstab.png)

---

### 6. Verifikasi
Memastikan swap aktif menggunakan `free -h`.

![Verifikasi](6-verifikasi-free.png)

---

## Kesimpulan
Swap memory sebesar 2GB berhasil dibuat dan aktif, serta akan tetap berjalan setelah reboot.