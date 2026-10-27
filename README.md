# OriginChain

> **Web3 Supply Chain Traceability Platform for Specialty Commodities**  
> Melacak asal-usul, integritas, dan perjalanan komoditas fisik bernilai tinggi berbasis batch, QR code publik, dan bukti kriptografis.

---

## 📌 Ringkasan Proyek

OriginChain menghubungkan produsen komoditas (seperti petani, koperasi, dan roastery kopi) dengan pembeli B2B dan konsumen akhir melalui sistem penelusuran (*traceability*) yang transparan dan tahan manipulasi.

- **Fokus Awal**: Kopi Spesialti & Kakao Indonesia.
- **Prinsip Utama**: *Pragmatic Web3* — operasional cepat dan terjangkau secara off-chain, dengan pengikatan bukti kriptografis (*Merkle Tree anchoring*) di blockchain L2 (Base / Polygon) tanpa mewajibkan pengguna memiliki crypto wallet atau membayar gas fee.

---

## 📚 Dokumentasi

- 💡 **[Master Project Prompt / Brainstorm](brainstrom.md)**: Dokumen visi produk, panduan perancangan, standar teknis, dan tahapan kerja.
- 🔄 **[End-to-End Business Process](docs/BUSINESS_PROCESS.md)**: Alur kerja lengkap stakeholder, siklus hidup batch (state machine), mitigasi risiko lapangan, dan model monetisasi SaaS.
- ⚙️ **[Project Rules & Memory](.agents/rules/project-context.md)**: Konfigurasi memori konteks proyek untuk agen AI Antigravity.

---

## 🛠️ Rencana Teknologi

- **Frontend & Backend**: Next.js (App Router, TypeScript).
- **Database**: PostgreSQL (Prisma / Drizzle ORM).
- **Storage**: S3-compatible Object Storage (Cloudflare R2 / Supabase Storage).
- **Verifikasi Kriptografis**: SHA-256 Document Hashing + Merkle Tree Root Anchoring on EVM Layer-2.
- **Identifikasi Fisik**: Dynamic QR Code Generator resolusi tinggi (SVG/PNG/PDF).

---

## 🗺️ Status & Roadmap

- [x] **Phase A — Discovery & Business Process Definition**
- [ ] **Phase B — Domain Modeling & UI Wireframing**
- [ ] **Phase C — Core Platform Engine (Batch, QR & Hashing)**
- [ ] **Phase D — Public Traceability & Verification Page**
- [ ] **Phase E — Cryptographic L2 Anchoring Engine**
- [ ] **Phase F — Pilot Launch with Business Partners**
