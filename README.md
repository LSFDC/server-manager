# Server Manager

**Server Manager** is an application designed to simplify the process of managing Lost Saga servers, services, or any custom server-related tools — both locally and remotely. This tool is intended for developers or administrators who want to efficiently control and monitor multiple server components from a single dashboard.

> This project is a part of the **Lost Saga Server** and aims to provide a clean and centralized way to manage multiple services.

---

## ✨ Features

- 🔧 **Start, Stop, Restart Servers** — Manage your services like `ls_mainsvr`, `ls_gamesvr`, and others.
- 📂 **Custom Configuration Support** — Load and store server configuration in editable formats.
- 📊 **Status Monitoring** — See the real-time status of each registered service.
- 🔒 **Safe Shutdown/Restart** — Handle processes safely to avoid crashes or data loss.
- 💬 **Log Output Viewer** — Display real-time log output from running services.
- 🖥️ **Cross-Platform Friendly** — Targeting Windows (primary), but planned for Linux support.

---

## 📦 Installation

Clone the repository and install dependencies:

```bash
git clone https://github.com/LSFDC/server-manager.git
cd server-manager
npm install
```

Start the development server:

```bash
npm run dev
```

Or build and start production:

```bash
npm run build
npm run start
```

---

## ⚙️ Configuration

Before running, make sure to configure your services. A sample structure might look like this:

```json
{
  "services": [
    {
      "name": "Game Server",
      "path": "C:/LostSaga/bin/ls_gamesvr.exe",
      "args": [],
      "autoStart": true
    },
    {
      "name": "Main Server",
      "path": "C:/LostSaga/bin/ls_mainsvr.exe",
      "args": [],
      "autoStart": true
    }
  ]
}
```

> Default config file: `./config/server-config.json`

---

## 🚀 Usage

Once running, open your browser:

```
http://localhost:3000
```

You can now:

- ✅ Add/edit/delete server entries
- ✅ Start/stop specific services
- ✅ View live logs per service
- ✅ Edit configuration files each server files easily

---

## 📁 Project Structure

```
server-manager/
├── public/
├── src/
│   ├── components/
│   ├── pages/
│   ├── utils/
│   └── config/
├── config/
│   └── server-config.json
├── .env
├── package.json
└── README.md
```

---

## 🧪 Environment Variables

You can set your own port and environment mode in `.env`:

```env
PORT=3000
NODE_ENV=development
```

---

## 📸 Screenshots

> SOON

---

## 🧑‍💻 Contributing

Want to help improve this project? Contributions are welcome!

1. Fork this repository
2. Create a new branch: `git checkout -b your-feature-name`
3. Commit your changes: `git commit -m "Add new feature"`
4. Push to your branch: `git push origin your-feature-name`
5. Submit a Pull Request 🚀

---

## 📜 License

This project is licensed under the **MIT License**. See the [Apache License 2.0](./LICENSE) file for details.

---

## 📬 Contact

Have questions, suggestions, or want to collaborate?

- GitHub Issues: [https://github.com/LSFDC/server-manager/issues](https://github.com/LSFDC/server-manager/issues)

---

> Made with ❤️ by [LSFDC](https://github.com/LSFDC)
