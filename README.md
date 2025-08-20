<img src="https://github.com/haniefautophile-official/OpenWrt_s905x/blob/main/ss/wrt.png"/>

# OpenWrt_s905x

Custom OpenWrt build targeting **Amlogic S905x TV boxes**. Repo ini menyediakan firmware siap pakai untuk perangkat berbasis SoC S905x dengan dukungan luas terhadap paket jaringan dan antarmuka grafis.

---

## Ringkasan

- **Target hardware**: STB B860H v1 & v2  
- Menggunakan basis proyek `amlogic-s9xxx-openwrt` untuk build firmware  
- Persisten terhadap overlay file system bersifat writeable (SquashFS + JFFS2)  

---

## Fitur Utama

### 1. OpenWrt Core
- **Sistem file writeable**: Root file system overlay memungkinkan modifikasi langsung dan instalasi paket tambahan via `opkg`  
- **LuCI & CLI**: Tersedia antarmuka web LuCI dan Unified Configuration Interface (UCI) untuk konfigurasi mudah  

### 2. Dukungan Platform Amlogic S905x
- Build mendukung SoC `s905x` dan varian terkait  
- Direkomendasikan untuk STB B860H v1 & v2  

### 3. Install & Flash
- Flash ke eMMC via SD card atau USB dengan tools seperti **BalenaEtcher** atau **Rufus**  
- Setelah boot, akses OpenWrt melalui browser default IP `192.168.1.1`  
  - User: `root`  
  - Password: `password`  

### 4. Backup & Restore
- Mendukung backup/restore sistem asli dari eMMC ke SD/USB untuk rollback  

### 5. Package Availability
- Repositori menyediakan akses ke paket jaringan dan utilitas tambahan kompatibel untuk SoC s905x  

---

## Quick Start

1. **Unduh image firmware** hasil build dari halaman Releases repositori  
2. Flash ke microSD atau USB menggunakan BalenaEtcher / Rufus  
3. Pasang ke STB, lakukan boot → akses via browser ke `192.168.1.1`  
4. Login dengan default (user: `root`, password: `password`)  
5. Konfigurasikan jaringan, WiFi, firewall, dsb., melalui LuCI atau CLI  

---

## Kustomisasi Lanjutan

- Tambahkan paket seperti firewall (nftables), VPN (WireGuard/OpenVPN), QoS (SQM), Samba, DNS, dsb., via `opkg`  
- Konfigurasi sistem seperti VLAN, mesh, port forwarding, Load balancing, dsb., semua didukung kuat oleh OpenWrt  

---

## Catatan Tambahan

Repositori ini **hanya untuk STB B860H v1 atau v2**, bukan firmware resmi. Disarankan untuk selalu backup sistem asli sebelum flashing.

---

## 📥 Download

[Klik di sini untuk download firmware](https://besargaji.com/CppE6C)
