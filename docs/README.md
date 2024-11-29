# 📋 Clipboard Utils

Command line utilities for advanced clipboard management in X environments. Perfect for power users and developers who need quick clipboard access and monitoring.

## 🚀 Features

### show-clip
Real-time clipboard monitoring with history and visual display
- Persistent clipboard history up to 50 entries
- Visual transitions with color-coded display
- Smart content truncation for long entries
- Configurable update interval
- Emergency cleanup options

### clip-file
Streamlined command-line clipboard operations
- Copy file contents directly to clipboard
- Accept piped input from other commands
- Clean, simple interface with Unix philosophy
- Works with X selection system

## 🛠 Installation

### Dependencies
```bash
# For Debian/Ubuntu
sudo apt-get install xclip

# For Arch Linux
sudo pacman -S xclip
```

### Setup
```bash
git clone https://github.com/yourusername/clipboard-utils.git
cd clipboard-utils
chmod +x bin/*
sudo ln -s $(pwd)/bin/show-clip /usr/local/bin/show-clip
sudo ln -s $(pwd)/bin/clip-file /usr/local/bin/clip-file
```

## 💻 Usage

### show-clip
Monitor and manage clipboard history:
```bash
show-clip              # Start monitoring clipboard
show-clip -c          # Clear clipboard history
show-clip -h          # Show help
show-clip -v          # Show version
```

Controls:
- Ctrl+X: Exit program
- Ctrl+D: Clear history

### clip-file
Copy file contents or input to clipboard:
```bash
clip-file file.txt    # Copy file contents to clipboard
cat file | clip-file  # Pipe file contents to clipboard
echo "text" | clip-file # Pipe text to clipboard
```

## 🔄 Version Status

### show-clip
Current Version: 1.8.5-alpha
- Full multiline support
- Visual transitions
- Progress bar during updates
- File-based history system
- Smart content truncation
- Emergency history cleanup
- Configurable colors and timing

### clip-file
Current Version: 1.0
- Basic file to clipboard functionality
- Stdin support
- Planned features:
  - Clipboard clearing (-c)
  - Content printing (-p)
  - Selection control (-s)


## 📋 TODO

### System Improvements
- [ ] Create proper config file system (~/.config/clipboard-utils/)
- [ ] Add logging system for debugging
- [ ] Implement proper error handling for xclip dependency
- [ ] Add system tray integration option
- [ ] Create uninstall script

### show-clip Enhancements
- [ ] Add search functionality for clipboard history
- [ ] Implement persistent history across sessions
- [ ] Add export/import functionality for clipboard history
- [ ] Create clipboard content categories/tags
- [ ] Add keyboard shortcuts for history navigation
- [ ] Implement mouse support for selection
- [ ] Add clipboard content filtering options
- [ ] Create different view modes (compact/full)

### clip-file Features
- [ ] Add multiple clipboard selection support
- [ ] Implement clipboard stack functionality
- [ ] Add content transformation options (base64, URL encode/decode)
- [ ] Create clipboard rotation feature
- [ ] Add clipboard content validation
- [ ] Implement secure string handling

### Integration Ideas
- [ ] Create Vim/Neovim plugin
- [ ] Add tmux integration
- [ ] Implement REST API for remote access
- [ ] Create desktop notifications for important clips
- [ ] Add integration with password managers
- [ ] Implement synchronization between machines

### Documentation
- [ ] Create man pages for both utilities
- [ ] Add detailed configuration guide
- [ ] Create troubleshooting guide
- [ ] Add examples for common use cases
- [ ] Create contribution guidelines


## 🤝 Contributing

1. Fork it
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request


## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## 👥 Authors

- Meldrey - Project Lead
- Claude/Anthropic - Development Support


## 🔮 Roadmap


### Version 2.0 (Next Major Release)
Focus: Core Architecture & Integration
- Proper config file system implementation
- Logging and error handling system
- System tray integration
- Persistent history across sessions
- Multiple clipboard selection support
- REST API foundations
- Man pages and documentation

### Version 2.1
Focus: Enhanced User Experience
- Search functionality for clipboard history
- Mouse support and keyboard shortcuts
- Clipboard categories/tags
- Different view modes (compact/full)
- Desktop notifications
- Content filtering options

### Version 2.2
Focus: Advanced Features
- Export/import functionality
- Content transformation options
- Clipboard stack functionality
- Clipboard rotation feature
- Content validation
- Secure string handling

### Version 2.3
Focus: Integration & Ecosystem
- Vim/Neovim plugin
- Tmux integration
- Password manager integration
- Multi-machine synchronization
- Remote access improvements

### Version 3.0
Focus: Enterprise & Professional Features
- Multi-user support
- Network clipboard sharing
- Encrypted clipboard content
- Plugin system
- Full API maturity
- Enterprise deployment options

### Current Development
#### show-clip (v1.9)
- Complete multiline viewing implementation
- Add history browsing improvements
- Implement scrolling with cursor support
- Add vi-style shortcuts
- Finalize Ctrl-X exit and Ctrl-D clear

#### clip-file (v1.1)
- Add clear clipboard option (-c)
- Implement print clipboard contents (-p)
- Add X selection support (-s)
- Complete error handling
