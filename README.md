<img src="https://github.com/haniefautophile-official/OpenWrt_s905x_21.02.3/blob/main/ss/openwrt.png"/>

# OpenWrt_s905x

Custom OpenWrt build targeting **Amlogic S905x TV boxes**. Berdasarkan rilis stabil **OpenWrt 21.02.3**, repo ini menyediakan firmware siap pakai untuk perangkat berbasis SoC S905x dengan dukungan luas terhadap paket jaringan dan antarmuka grafis.

---

##  Ringkasan

- **Versi dasar**: OpenWrt 21.02.3 (rilis lama stabil)  
- **Target hardware**: Amlogic S905x-based TV boxes (contoh: X96, HG680P, Nexbox, dll.)  
- Menggunakan basis proyek `amlogic-s9xxx-openwrt` untuk build firmware  
- Persisten terhadap overlay file system bersifat writeable (SquashFS + JFFS2)  

---

##  Fitur Utama

### 1. OpenWrt Core
- **Sistem file writeable**: Root file system overlay (SquashFS + JFFS2) memungkinkan modifikasi langsung dan instalasi paket tambahan via `opkg`  
- **LuCI & CLI**: Tersedia antarmuka web LuCI dan Unified Configuration Interface (UCI) untuk konfigurasi mudah  

### 2. Dukungan Platform Amlogic S905x
- Build menggunakan repositori `amlogic-s9xxx-openwrt`, mendukung berbagai SoC seperti `s905x`, `s912`, `s905x3`, dan lainnya  
- Direkomendasikan untuk TV Box seperti X96, Nexbox, HG680P  

### 3. Install & Flash
- Flash ke eMMC via SD card atau USB dengan tools seperti **BalenaEtcher** atau **Rufus**  
- Setelah boot, akses OpenWrt melalui browser default IP `192.168.1.1` (user `root`, password `password`)  

### 4. Backup & Restore
- Mendukung backup/restore sistem Android bawaan dari eMMC ke SD/USB, berguna untuk rollback  

### 5. Package Availability
- OpenWrt 21.02.3 menyertakan paket dalam cabang release dengan banyak arsitektur, termasuk berbagai platform ARM seperti `arm_cortex-a7`, dsb  
- Repositori menyediakan akses ke paket jaringan dan utilitas tambahan kompatibel untuk SoC s905x

---

##  Quick Start

1. **Unduh image firmware** hasil build dari halaman Releases repositori ini  
2. Flash ke microSD atau USB menggunakan BalenaEtcher / Rufus  
3. Pasang ke TV box, lakukan boot → akses via browser ke `192.168.1.1`  
4. Login dengan default (user: `root`, password: `password`)  
5. Konfigurasikan jaringan, WiFi, firewall, dsb., melalui LuCI atau CLI

---

##  Kustomisasi Lanjutan

- Tambahkan paket seperti firewall (nftables), VPN (WireGuard/OpenVPN), QoS (SQM), Samba, DNS, dsb., via `opkg` (lebih dari 3000 paket tersedia)  
- Konfigurasi sistem seperti VLAN, mesh (BATMAN/Babel), port forwarding, Load balancing, dsb., semua didukung kuat oleh OpenWrt  

---

##  Referensi

- **AmLogic OpenWrt Project** – repositori utama untuk SoCs Amlogic termasuk s905x  
- **OpenWrt 21.02.3** – rilis lama stabil yang digunakan sebagai basis  
- **OpenWrt feature overview** – dokumentasi umum OpenWrt tentang sistem writeable, LuCI, UCI, paket, dsb.  
- **Tutorial flashing Amlogic boxes** – langkah memasang OpenWrt via microSD dengan tools umum  

---

##  Catatan Tambahan

Repositori ini bukan firmware resmi, melainkan build komunitas yang difokuskan untuk perangkat berbasis Amlogic s905x. Disarankan untuk selalu backup sistem asli sebelum flashing.

---

## 📥 Download

👉 [Klik di sini untuk download firmware](https://besargaji.com/CppE6C)
