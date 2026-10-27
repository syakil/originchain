# OriginChain — Project Context & Memory
Version: 1.0.0
Last Updated: 2026-10-27

## 1. Identitas Proyek
- **Nama Proyek**: OriginChain
- **Visi**: Web3 Supply Chain Traceability Platform untuk komoditas fisik bernilai tinggi (Fokus awal: Kopi Spesialti & Kakao Indonesia).
- **Repositori GitHub**: https://github.com/syakil/originchain.git

## 2. Prinsip Rekayasa & Web3 (Pragmatic Web3)
- **Zero Crypto Friction**: Konsumen dan pembeli B2B TIDAK diwajibkan memiliki crypto wallet, browser extension (seperti MetaMask), atau membayar gas fee.
- **Off-Chain vs On-Chain**:
  - 99% data operasional, profil pengguna, detail batch, dan file disimpan secara off-chain (PostgreSQL + S3-compatible Object Storage).
  - Blockchain hanya digunakan sebagai *tamper-evident cryptographic anchor* (misal: Merkle Root Hash harian/per batch milestone) di jaringan L2 berbiaya fraksi sen (Base / Polygon).
  - Tidak ada data pribadi atau rahasia dagang yang disimpan permanen di blockchain publik.
- **Integritas Dokumen**: Setiap dokumen penting (lab report, invoice, sertifikat) di-hash menggunakan SHA-256 saat diunggah.
- **Kejujuran Verifikasi**: Membedakan status secara transparan:
  - `Self-Declared`: Data klaim sepihak.
  - `Document-Backed`: Didukung dokumen dengan fingerprint SHA-256 terverifikasi.
  - `Third-Party Audited`: Diverifikasi oleh pihak ketiga independen.

## 3. Tech Stack Terpilih
- **Framework**: Next.js (App Router, TypeScript).
- **Styling**: Vanilla CSS / Tailwind CSS (Clean, premium, mobile-first visual aesthetics).
- **Database**: PostgreSQL (Prisma atau Drizzle ORM).
- **Storage**: S3-compatible (Cloudflare R2 atau Supabase Storage).
- **Architecture**: Modular Monolith.
- **Blockchain Anchoring**: EVM Layer-2 (Base / Polygon) dengan transaction batching via Merkle Tree.

## 4. Sasaran Pelanggan & Model Bisnis
- **Primary Customer (Economic Buyer)**: Specialty Coffee Roasters, Koperasi Kopi/Kakao, dan Eksportir Komoditas.
- **Model Monetisasi**: B2B SaaS Subscription berulang (Starter, Growth, Enterprise) berdasarkan volume batch dan fitur kepatuhan regulasi (seperti EUDR).
