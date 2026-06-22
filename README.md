# PeerChat

A decentralized peer-to-peer video chat application built with WebRTC and Agora RTM for signaling. PeerChat enables users to join a shared room and establish direct video and audio connections with other participants in real time. :contentReference[oaicite:0]{index=0}

## Features

- Real-time peer-to-peer video communication
- WebRTC-powered audio and video streaming
- Room-based chat lobby
- Lightweight frontend built with vanilla JavaScript
- Responsive user interface
- Direct browser-to-browser media connections

## Tech Stack

- HTML5
- CSS3
- JavaScript (ES6)
- WebRTC
- Agora RTM SDK

## Project Structure

```
Peerchat/
├── index.html
├── lobby.html
├── main.js
├── main.css
├── lobby.css
├── agora-rtm-sdk-1.5.1.js
├── icons/
└── README.md
```

## How It Works

1. Users enter a room through the lobby.
2. Agora RTM is used to exchange signaling messages between participants.
3. WebRTC establishes a direct peer-to-peer connection.
4. Audio and video streams are shared directly between browsers.
5. Participants can communicate with low latency and without routing media through a central media server.

## Getting Started

### Prerequisites

- Modern web browser (Chrome, Firefox, Edge)
- Agora RTM App ID

### Installation

Clone the repository:

```bash
git clone https://github.com/pcortezj/Peerchat.git
cd Peerchat
```

### Configuration

Update the Agora App ID in the JavaScript configuration before running the application.

Example:

```javascript
const APP_ID = "YOUR_AGORA_APP_ID";
```

### Run Locally

Because WebRTC requires a secure context, serve the application through a local web server.

Using Python:

```bash
python -m http.server 8000
```

Then visit:

```
http://localhost:8000
```

## Future Improvements

- Screen sharing
- Text chat
- Group video rooms
- User authentication
- End-to-end encryption enhancements
- Mobile-first UI improvements
- Recording and playback

## Learning Objectives

This project explores:

- WebRTC peer connection lifecycle
- ICE candidate negotiation
- Session Description Protocol (SDP)
- Real-time signaling architecture
- Browser media APIs
- Real-time communication patterns

## Author

**Pa'tron Johnson**

Software Engineer focused on building scalable web applications, real-time systems, and developer tools.

GitHub: https://github.com/pcortezj

## License

This project is available under the MIT License.
