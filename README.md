# Whisper Me

Simple home whisper dictation

The purpose of this project is to allow a compiled whisper C++ instance to
interact via a simple Python server over a wireguard VPN connection to a phone
that uses Tasker to send audio files and receive transcribed text back over port
443 using a self-signed certificate (this is redundant encryption, but for my
purpose it is a reasonable failsafe).

## Tools Used for this project

| Component    | Use             | Location                                                 |   |
+ ------------ + --------------- + -------------------------------------------------------- |
| Whsper.CPP   | Transcription   | [whisper.cpp](https://github.com/ggml-org/whisper.cpp)   |   |
| pywhispercpp | Python bindings | [pywhispercpp](https://github.com/absadiki/pywhispercpp) |   |
| Claude       | Code assistance | [claude.ai](https://claude.ai)                           |   |

## Project Components

Additional information is in the respective README.md files within the subfolders.

### Whisper-Me Python Server
Python server is named Whisper Me and is in the [whisper-me](/whisper-me)
directory.

It uses components from [ansadiki's](https://github.com/absadiki) [pywhispercpp](https://github.com/absadiki/pywhispercpp) project.


### Tasker
Tasker components are in the Tasker directory

## Disclaimer
This project comes with no offer of support or troubleshooting, I am
unfortunately very busy, this project has developed just for me in order to be
able to do rapid dictation.

Large portions of the code were written by Claude.

## License
[MIT License](LICENSE)
