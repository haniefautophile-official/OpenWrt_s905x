<img src="https://github.com/haniefautophile-official/OpenWrt_s905x_21.02.3/blob/main/ss/openwrt.png"/>
# penWrt_s905x_21.02.3

Custom OpenWrt build targeting **Amlogic S905x TV boxes**. Berdasarkan rilis stabil **OpenWrt 21.02.3**, repo ini menyediakan firmware siap pakai untuk perangkat berbasis SoC S905x dengan dukungan luas terhadap paket jaringan dan antarmuka grafis.

---

##  Ringkasan

- **Versi dasar**: OpenWrt 21.02.3 (rilis lama stabil) :contentReference[oaicite:0]{index=0}  
- **Target hardware**: Amlogic S905x-based TV boxes (contoh: X96, HG680P, Nexbox, dll.)  
- Menggunakan basis proyek `amlogic-s9xxx-openwrt` untuk build firmware :contentReference[oaicite:1]{index=1}  
- Persisten terhadap overlay file system bersifat writeable (SquashFS + JFFS2) :contentReference[oaicite:2]{index=2}  

---

##  Fitur Utama

### 1. OpenWrt Core
- **Sistem file writeable**: Root file system overlay (SquashFS + JFFS2) memungkinkan modifikasi langsung dan instalasi paket tambahan via `opkg` :contentReference[oaicite:3]{index=3}  
- **LuCI & CLI**: Tersedia antarmuka web LuCI dan Unified Configuration Interface (UCI) untuk konfigurasi mudah :contentReference[oaicite:4]{index=4}

### 2. Dukungan Platform Amlogic S905x
- Build menggunakan repositori `amlogic-s9xxx-openwrt`, mendukung berbagai SoC seperti `s905x`, `s912`, `s905x3`, dan lainnya :contentReference[oaicite:5]{index=5}  
- Direkomendasikan untuk TV Box seperti X96, Nexbox, HG680P :contentReference[oaicite:6]{index=6}  

### 3. Install & Flash
- Flash ke eMMC via SD card atau USB dengan tools seperti **BalenaEtcher** atau **Rufus** :contentReference[oaicite:7]{index=7}  
- Setelah boot, akses OpenWrt melalui browser default IP `192.168.1.1` (user `root`, password `password`) :contentReference[oaicite:8]{index=8}  

### 4. Backup & Restore
- Mendukung backup/restore sistem Android bawaan dari eMMC ke SD/USB, berguna untuk rollback :contentReference[oaicite:9]{index=9}  

### 5. Package Availability
- OpenWrt 21.02.3 menyertakan paket dalam cabang release dengan banyak arsitektur, termasuk berbagai platform ARM seperti `arm_cortex-a7`, dsb :contentReference[oaicite:10]{index=10}  
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

- Tambahkan paket seperti firewall (nftables), VPN (WireGuard/OpenVPN), QoS (SQM), Samba, DNS, dsb., via `opkg` (lebih dari 3000 paket tersedia) :contentReference[oaicite:11]{index=11}  
- Konfigurasi sistem seperti VLAN, mesh (BATMAN/Babel), port forwarding, Load balancing, dsb., semua didukung kuat oleh OpenWrt :contentReference[oaicite:12]{index=12}

---

##  Referensi

- **AmLogic OpenWrt Project** – repositori utama untuk SoCs Amlogic termasuk s905x :contentReference[oaicite:13]{index=13}  
- **OpenWrt 21.02.3** – rilis lama stabil yang digunakan sebagai basis :contentReference[oaicite:14]{index=14}  
- **OpenWrt feature overview** – dokumentasi umum OpenWrt tentang sistem writeable, LuCI, UCI, paket, dsb. :contentReference[oaicite:15]{index=15}  
- **Tutorial flashing Amlogic boxes** – langkah memasang OpenWrt via microSD dengan tools umum :contentReference[oaicite:16]{index=16}  

---

##  Catatan Tambahan

Repositori ini bukan firmware resmi, melainkan build komunitas yang difokuskan untuk perangkat berbasis Amlogic s905x. Disarankan untuk selalu backup sistem asli sebelum flashing.

---

Semoga README ini membantu kamu dalam menerangkan fitur `penWrt_s905x_21.02.3`. Kalau ada hal spesifik yang ingin ditambahkan—misalnya fitur WiFi, VPN, atau auto-update—silakan beri tahu saya dan bisa kita tambahkan!
::contentReference[oaicite:17]{index=17}
