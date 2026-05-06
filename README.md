````markdown
# IS370 Secure Chat Application

A Python client-server chat application developed for the IS370 course project.  
The system supports secure messaging, user authentication, group chats, broadcast messages, image sharing, and chat history.

## Features

- User registration and login
- Private, group, and broadcast messaging
- Encrypted communication using Fernet
- Password hashing with SHA-256
- Multi-client support using sockets and threading
- Image sharing
- Chat history logging
- SQLite database for users and groups
- GUI built with CustomTkinter

## Technologies Used

- Python
- Socket Programming
- SQLite
- CustomTkinter
- Cryptography / Fernet
- Pillow

## Project Structure

```text
├── GUI.py
├── server.py
├── register_and_groups.py
├── requirements.txt
└── utility/
    ├── database.py
    └── encryption.py
````

## Installation

```bash
git clone https://github.com/riyanfa/IS370-Project.git
cd IS370-Project
pip install -r requirements.txt
```

## Usage

Start the server:

```bash
python server.py
```

Register users or manage groups:

```bash
python register_and_groups.py
```

Run the client GUI:

```bash
python GUI.py
```

To test multiple users, run `GUI.py` in more than one terminal.

## Messaging Options

* `All` — broadcast message to all online users
* `@username` — private message
* `#groupname` — group message

## Notes

* The application runs on `127.0.0.1:5051` by default.
* Chat logs are stored locally in a `logs/` folder.
* The SQLite database is created automatically as `user.db`.
