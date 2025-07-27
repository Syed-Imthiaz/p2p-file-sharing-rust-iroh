# 🔁 P2P File Sharing in Rust using IROH

A minimal peer-to-peer file sharing CLI tool built in **Rust** using [IROH](https://www.iroh.computer).  
This project enables fast, decentralized file transfers using an in-memory store with simple command-line usage.

---

## 📦 Features

- ⚙️ **Pure Rust**: Safe, fast, and portable
- 🌐 **Peer-to-Peer (P2P)**: No central server needed
- 📂 **Send & Receive**: Share files via blob tickets
- 🧠 **In-Memory Storage**: Lightweight and fast with `iroh-blobs::MemStore`

---

## 🚀 Usage

### 📨 Send a File

bash


cargo run -- send path/to/file.txt

## 📥 Receive a File

bash


cargo run -- receive [TICKET] path/to/save.txt

---

## 📁 Example

## ✅ Sender

bash


cargo run -- send notes.pdf

## 🧾 Output

arduino

Hashing file.
File hashed. Fetch this file by running:
cargo run -- receive [ticket] notes.pdf

## ✅ Receiver

bash


cargo run -- receive [ticket] notes.pdf

---

## 🔧 Dependencies

**iroh** – P2P networking  
**iroh-blobs** – Blob storage & file transfer  
**tokio** – Async runtime  
**anyhow** – Error handling


## ➕ Add to your Cargo.toml

toml


[dependencies]
anyhow = "1"
tokio = { version = "1", features = ["full"] }
iroh = "0.10.0"
iroh-blobs = "0.10.0"

---
## 🔗 Resources

- 🌐 [iroh.computer](https://www.iroh.computer)
- 📘 [Awesome IROH GitHub Collection](https://github.com/n0-computer/awesome-iroh)
- 🚀 [Sendme Tool](https://www.iroh.computer/sendme)
- 🎥 [Sendme Demo – YouTube](https://youtu.be/uj-7Y_7p4Dg?si=L0lLnxlkqhxs9AqX)
- 🎥 [P2P File Sharing Overview – YouTube](https://youtu.be/tlSwje2ru34?si=MU1UjEKoIliAZl86)

---

