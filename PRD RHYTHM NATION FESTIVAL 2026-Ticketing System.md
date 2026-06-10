PRODUCT REQUIREMENTS DOCUMENT (PRD)
RHYTHM NATION FESTIVAL 2026 Ticketing System

Project Overview
RHYTHM NATION FESTIVAL 2026 Ticketing System merupakan platform penjualan tiket online yang dirancang untuk mendukung proses pembelian tiket festival secara aman, cepat, dan stabil. Sistem ini mampu menangani lonjakan pengunjung saat ticket war melalui mekanisme antrean digital, pengelolaan stok tiket otomatis, serta validasi e-ticket berbasis QR Code unik.
Objectives
Menjaga stabilitas sistem saat ticket war.
Mengurangi risiko tiket palsu dan duplikasi tiket.
Mengoptimalkan pengelolaan stok tiket melalui booking lock.
Memberikan pengalaman pembelian tiket yang mudah dan aman.

Key Users
Customer: Pengguna yang membeli tiket festival, melakukan pembayaran, dan mengakses e-ticket.
Admin/Event Organizer: Pihak yang mengelola stok tiket, memantau transaksi, serta melakukan validasi tiket saat acara berlangsung.

Core Features
1. Queue Management System
Waiting room saat traffic tinggi.
Nomor antrean dan estimasi waktu tunggu.
2. Booking Lock System
Reservasi tiket selama 10 menit.
Tiket otomatis kembali ke stok jika pembayaran tidak selesai.
3. Ticket Purchase & Payment
Pemilihan kategori tiket dan jumlah pembelian.
Pembayaran melalui QRIS atau Virtual Account.
Pembaruan status pembayaran otomatis.
4. E-Ticket System
QR Code unik untuk setiap tiket.
Validasi satu kali scan (single-use ticket).
5. User Account & Dashboard
Registrasi dan login pengguna.
Riwayat transaksi dan daftar tiket aktif.
6. Refund Management
Pengajuan refund.
Monitoring status refund.
7. Admin Dashboard
Manajemen pengguna.
Monitoring stok tiket.
Monitoring transaksi dan validasi tiket.

Technology Stack
Backend: Laravel 12
Frontend: Vue 3
Database: MySQL

Data Models
User: Menyimpan data akun pengguna.
TicketCategory: Menyimpan kategori tiket, harga, dan stok.
Booking: Menyimpan informasi transaksi dan status pembayaran.
Ticket: Menyimpan data tiket, nomor seri, QR Code, dan status penggunaan.
Relationship
User → Booking (1)
Booking → Ticket (1)
TicketCategory → Ticket (1)

Main User Flow
Pembelian Tiket:
User → Waiting Room → Pilih Tiket → Checkout → Pembayaran → Booking Success → E-Ticket Terbit
Validasi Tiket:
User Menunjukkan QR Code → Petugas Scan → Sistem Verifikasi → Status Tiket Menjadi Used

Out of Scope
Marketplace jual-beli tiket resmi.
Pemilihan nomor kursi.
Penjualan merchandise.
Survei atau kuesioner peserta.

