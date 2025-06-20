# Video Conferencing for Computer Department

This is a simple web-based video conferencing application built using the **Agora Web SDK**. It is designed to support real-time communication for departmental or academic collaboration.

## 📁 Project Structure

| File/Folder               | Description |
|---------------------------|-------------|
| `index.html`              | Main HTML page for the video conferencing UI. |
| `index.css`               | Stylesheet for UI layout and design. |
| `index.js`                | JavaScript logic for handling user media, channel operations, and Agora integration. |
| `AgoraRTC_N-4.19.1.js`    | Agora Web SDK library file (version 4.19.1). |
| `vendor/`                 | Directory for additional third-party resources (if any). |

## 🛠️ Setup Instructions

1. **Clone or download** this project folder.

2. **Open `index.html`** in a browser (Chrome is recommended).

3. **Ensure internet connectivity** for Agora SDK or host the files via a local server.

4. **Agora Setup:**
   - Get a free [Agora App ID](https://www.agora.io/en/).
   - Replace the placeholder in the JavaScript file (likely in `index.js`) with your App ID.

```js
const client = AgoraRTC.createClient({ mode: "rtc", codec: "vp8" });
client.init("YOUR_APP_ID_HERE");
```

5. **Run the app:**
   - Use `Live Server` extension in VS Code or run a local HTTP server:
   ```bash
   npx serve .
   ```

## ✨ Features

- Real-time video and audio communication
- Join and leave channel functionality
- Scalable with Agora's cloud infrastructure
- Modular file organization for easy enhancement

## ✅ Requirements

- A modern web browser
- Agora App ID
- Internet connection

## 🔒 Notes

- Make sure to secure your App ID and use token authentication for production use.
- This implementation is intended for educational or prototype purposes.

## 📄 License

This project is open-source and intended for educational and academic use.
