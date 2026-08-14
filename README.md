# Smart-Chess-Board
To bring it up to modern standards, I developed a complete Python-based server setup for the Raspberry Pi. It includes:      Stockfish Integration with move quality evaluation.      OLED Chess Clock display support (I2C).      Web TV Visualizer (shows live board state &amp; move evaluation on any TV/browser).      CYD Touchscreen UI support.
# ♟️ DIY Smart Chessboard Server (Raspberry Pi, ESP32 CYD, OLED & TV-Visualizer)


A feature-rich, standalone Python server for custom-built DIY smart chessboards (e.g., 3D-printed magnetic or LED boards). 

This project breathes new life into custom chessboards by acting as a central hub running on a Raspberry Pi. It coordinates physical LED indicators, a dedicated I2C OLED chess clock, a local Web/TV visualizer with Stockfish engine analysis, and an ESP32 Cheap Yellow Display (CYD) touchscreen interface.

### ✨ Key Features
* **Stockfish Engine Integration:** Real-time position evaluation and blunder detection ("Blunder").
* **Dedicated I2C OLED Chess Clock:** Displays active player timers, move indicators, last played UCI move, and game status (Checkmate, Stalemate, Turn).
* **Web TV Visualizer:** Live interactive web dashboard for spectators on port `8080` (board representation, evaluation bar, move quality commentary).
* **ESP32 CYD Touchscreen Support:** Socket-based communication (`port 5000`) for menu navigation, mode selection (PvP, vs Bot, Auto-Play), and move sync.
* **Arduino/Hardware LED Support:** Communicates via Serial (`/dev/ttyAMA0`) to light up squares on physical boards.
