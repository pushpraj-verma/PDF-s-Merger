
# 🧾 PDF Merger Web Application

This is a simple Node.js web application that allows users to upload two PDF files and merges them into a single downloadable file. The merged PDF is automatically sent as a download and deleted after download, along with the uploaded files.

## 🔗 GitHub Repository

Ensure your GitHub repository is always accessible during evaluation.

## 📂 Features

- Upload two PDFs from the browser
- Merge them on the server using `pdf-merger-js`
- Auto-download the result
- Automatically deletes uploaded and merged PDFs after download

---

## 🚀 Getting Started

### 📦 Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/) (v14 or later)
- [npm](https://www.npmjs.com/)

---

## 🛠 Setup Instructions

1. **Clone the repository:**

   ```bash
   git clone https://github.com/your-username/pdf-merger-app.git
   cd pdf-merger-app
   ```

2. **Install dependencies:**

   ```bash
   npm install
   ```

3. **Start the server:**

   ```bash
   node index.js
   ```

4. **Visit in your browser:**

   ```
   http://localhost:3000
   ```

---

## 🧩 Project Structure

```
pdf-merger-app/
│
├── index.js               # Main server file
├── merge.js               # Logic for merging PDFs
├── public/                # Temporarily stores merged PDFs
├── uploads/               # Temporarily stores uploaded PDFs
├── templates/
│   └── index.html         # Frontend form
└── package.json
```

---

## 📦 Dependencies

- [express](https://www.npmjs.com/package/express) - Web framework
- [multer](https://www.npmjs.com/package/multer) - Middleware for handling `multipart/form-data` (file uploads)
- [pdf-merger-js](https://www.npmjs.com/package/pdf-merger-js) - PDF merging utility
- [path](https://nodejs.org/api/path.html) - Node.js path module (built-in)
- [fs](https://nodejs.org/api/fs.html) - Node.js file system module (built-in)

---

## ⚙️ Configurations

No special configuration is required. Uploaded and merged files are temporarily stored in `uploads/` and `public/` folders, respectively, and automatically deleted after processing.

---

## 📸 Demo Screenshot

![PDF Merger Form](screenshots/demo.png)

*(Create a `screenshots/` folder and add `demo.png` to include this)*

---

## ❗ Notes

- All uploaded and merged files are deleted immediately after download to maintain server cleanliness.
- This project does **not use a database**.
- If you add database or API integration later, make sure to update this README accordingly.

---

## 📬 Contact

If you encounter any issues, feel free to open an issue or reach out via GitHub.

---

## 📄 License

MIT License — free to use and modify.
