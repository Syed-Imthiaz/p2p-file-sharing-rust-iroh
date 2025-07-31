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

- **iroh** – P2P networking
- **iroh-blobs** – Blob storage & file transfer  
- **tokio** – Async runtime  
- **anyhow** – Error handling

### ➕ Add to your `Cargo.toml`


[dependencies]


anyhow = "1"


tokio = { version = "1", features = ["full"] }


iroh = "0.10.0"


iroh-blobs = "0.10.0"



---
## 🔗 Resources

- 🌐 [iroh.computer](https://iroh.computer)
- 📘 [Awesome IROH GitHub Collection](https://github.com/n0-computer/awesome-iroh)
- 🚀 [Sendme Tool](https://github.com/n0-computer/sendme)
- 🎥 [Sendme Demo – YouTube](https://www.youtube.com/watch?v=Po3WRuD_Ic4)
- 🎥 [P2P File Sharing Overview – YouTube](https://www.youtube.com/watch?v=_nC2EqkFq8g)

---

## 👨‍💻 Author

**Syed Imthiaz I**  
B.E. Computer Science and Engineering  
KCG College of Technology  
🔗 [LinkedIn](https://www.linkedin.com/in/syedimthiaz/)  
🔗 [LinkedIn Post](https://www.linkedin.com/feed/update/urn:li:activity:7355251106823700480/)

---

## 🚫 License & Disclaimer

© 2025 Syed Imthiaz I — All rights reserved.
Unauthorized copying, modification, distribution, or use of this code or any part of it is strictly prohibited without the express written permission of the author.

📩 For permission requests, contact: syedimthiaz2006@gmail.com

---

