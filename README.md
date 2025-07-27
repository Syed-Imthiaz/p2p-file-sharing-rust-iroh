# 🔁 P2P File Sharing in Rust using IROH

A minimal peer-to-peer file sharing CLI tool built in **Rust** using [IROH](https://www.iroh.computer) and `iroh-blobs`. This project enables fast, decentralized file transfers using an in-memory store with simple command-line usage.

---

## 📦 Features

- ⚙️ **Pure Rust**: Safe, fast, and portable.
- 🌐 **Peer-to-Peer (P2P)**: Direct connection between nodes, no central server.
- 📂 **Send & Receive**: Easily share files via generated blob tickets.
- 🧠 **In-Memory Storage**: Lightweight blob store using `iroh-blobs::MemStore`.

---

## 🚀 Usage

### 📨 Send a File

```bash
cargo run -- send path/to/file.txt

### 📥 Receive a File
bash
Copy
Edit
cargo run -- receive [TICKET] path/to/save.txt

---

## 📁 Example

## ✅ Sender

bash
Copy
Edit
cargo run -- send notes.pdf

## Output:

arduino
Copy
Edit
Hashing file.
File hashed. Fetch this file by running:
cargo run -- receive [ticket] notes.pdf

## ✅ Receiver
bash
Copy
Edit
cargo run -- receive [ticket] notes.pdf

---

## 🔧 Dependencies

iroh – Peer-to-peer networking

iroh-blobs – Blob storage & file transfer

tokio – Async runtime

anyhow – Error handling

## Add to your Cargo.toml:
toml
Copy
Edit
[dependencies]
anyhow = "1"
tokio = { version = "1", features = ["full"] }
iroh = "0.10.0"
iroh-blobs = "0.10.0"

---

🔗 Resources
🌐 iroh.computer

📘 Awesome IROH GitHub Collection

🚀 Sendme Tool

🎥 Sendme Demo – YouTube

🎥 P2P File Sharing Overview – YouTube

---





