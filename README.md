# TPA — Skript Edition

A lightweight **/tpa** system for Minecraft servers running the **Skript** plugin.  
Players can request to teleport **to** another player or invite a player to teleport **here**, with built-in request expiry, movement-cancel protection, and simple slash commands for accepting, denying, or cancelling a request.

---

## ✨ Features

| Feature                | Description                                                    |
|------------------------|----------------------------------------------------------------|
| **/tpa \<player\>**    | Request to teleport **to** another player                      |
| **/tpahere \<player\>**| Ask another player to teleport **to you**                      |
| **/tpaaccept**         | Accept the oldest pending request                              |
| **/tpadeny**           | Deny the oldest pending request                                |
| **/tpacancel**         | Cancel a request you sent                                      |
| **Request expiry**     | Requests expire after **60 seconds**                           |
| **Movement cancel**    | Moving during the 5-second warm-up aborts the teleport         |
| **Clickable chat UI**  | Players click **[Accept] / [Deny]** buttons in chat            |
| **Custom prefix**      | One-line option lets you brand all messages to your server     |

---

## 📂 Installation

1. **Install Skript** (≥ 2.7) on your Spigot/Paper server.  
2. Drop `tpa.sk` into `plugins/Skript/scripts/`.  
3. Run `/skript reload TPA` from console or in-game.

_No addons required — everything uses native Skript JSON._

---

## ⚙️ Configuration

```skript
options:
    pr: &b&lTPA &7┃   # Prefix shown in every message
