# 📝 Code Snippet Manager

A lightweight, portable code snippet manager built as a single HTML file. Store, organize, search, and manage your code snippets with a clean, modern interface that works across all your devices.

## ✨ Features

### Core Functionality
- **📁 Snippet Management**: Create, edit, delete, and organize code snippets
- **🔍 Advanced Search**: Search across titles, code content, documentation, and languages
- **🏷️ Language Support**: 20+ programming languages with syntax highlighting
- **📖 Documentation**: Optional detailed documentation field for each snippet
- **🎯 Smart Filtering**: Filter by language and sort by various criteria

### Import/Export
- **💾 Native File Dialogs**: Choose custom filenames and paths for exports
- **🔄 Smart Import**: Merge, replace, or append options to handle duplicates
- **📤 Auto-Export**: Optional auto-save functionality
- **🚀 Portable**: Single HTML file + JSON backup = complete solution

### User Experience
- **🎨 Modern Design**: Glassmorphism design with gradient backgrounds
- **⌨️ Keyboard Navigation**: Full keyboard control with intuitive shortcuts
- **📱 Mobile Responsive**: Works seamlessly on desktop, tablet, and mobile
- **🔍 Font Scaling**: Adjustable font size for better readability
- **🎯 Visual Selection**: Clear highlighting for selected snippets
- **🌐 Cross-Platform**: Runs in any modern web browser

## 🚀 Quick Start

### Installation
1. Download or save the HTML file to your computer
2. Double-click to open in your default browser
3. Start adding snippets or import an existing collection

### First Use
1. **Import existing snippets**: Click "Import" to load a `snippets-backup.json` file
2. **Create new snippet**: Click "New" or press `Insert` key
3. **Search and filter**: Use the search bar and language filter
4. **Export for backup**: Click "Export" to save your collection

## 📋 Keyboard Shortcuts

### Browse View
| Key | Action |
|-----|--------|
| `Insert` | Create new snippet |
| `↑/↓` | Navigate through snippets |
| `Enter` | Edit selected snippet |
| `Delete` | Delete selected snippet |
| `Ctrl+F` | Focus search bar |

### File Operations
| Key | Action |
|-----|--------|
| `Ctrl+E` | Export snippets |
| `Ctrl+I` | Import snippets |
| `Ctrl+V` | Read from clipboard |

### Add/Edit Modal
| Key | Action |
|-----|--------|
| `Ctrl+S` | Save snippet |
| `Escape` | Close modal without saving |

### Display Controls
| Key | Action |
|-----|--------|
| `+` | Increase font size |
| `-` | Decrease font size |
| `0` | Reset font size to default |

### Mouse Actions
- **Single-click**: Select snippet
- **Double-click**: Edit snippet
- **Action buttons**: Copy, edit, or delete individual snippets

## 🏷️ Supported Languages

- **Web**: JavaScript, TypeScript, HTML, CSS
- **Backend**: Python, Java, C++, C#, Go, Rust, PHP, Ruby, R, Scala
- **Data**: SQL, JSON, XML, YAML, Excel
- **Analytics**: PowerBI M-Code, PowerBI DAX, Kusto (KQL), PySpark
- **Scripts**: Bash, PowerShell, Windows Batch
- **Documentation**: Markdown
- **Other**: Custom language support

## 💾 File Format

Snippets are stored in JSON format with the following structure:

```json
[
  {
    "id": "unique-identifier",
    "language": "javascript",
    "description": "Snippet title/description",
    "documentation": "Optional detailed explanation",
    "code": "function example() {\n  return 'Hello World';\n}",
    "created": "2024-01-01T12:00:00.000Z",
    "modified": "2024-01-01T12:30:00.000Z"
  }
]
```

### Required Fields
- `id`: Unique identifier
- `language`: Programming language
- `description`: Brief title/description
- `code`: The actual code content
- `created`: Creation timestamp

### Optional Fields
- `documentation`: Detailed explanation or usage notes
- `modified`: Last modification timestamp

## 🔄 Workflow Examples

### Daily Development
1. **Morning**: Open snippet manager, import latest backup
2. **During work**: Copy useful code snippets, add documentation
3. **End of day**: Export updated collection to shared location

### Cross-Device Sync
1. **Device A**: Create/modify snippets → Export to cloud storage
2. **Device B**: Import from cloud storage → Continue working
3. **Repeat**: Keep collections synchronized across all devices

### Team Sharing
1. **Individual**: Curate personal snippet collection
2. **Export**: Generate team-specific snippet collections
3. **Share**: Distribute JSON files via email, Git, or shared drives
4. **Import**: Team members import and merge with their collections

## 📱 Platform Compatibility

### Desktop Browsers
- ✅ Chrome/Chromium (recommended)
- ✅ Firefox
- ✅ Safari
- ✅ Microsoft Edge

### Mobile Browsers
- ✅ Chrome Mobile
- ✅ Safari iOS
- ✅ Firefox Mobile
- ✅ Samsung Internet

### Operating Systems
- ✅ Windows (all versions)
- ✅ macOS
- ✅ Linux (all distributions)
- ✅ Steam Deck (Desktop mode)
- ✅ iOS/iPadOS
- ✅ Android

## 🛠️ Advanced Features

### Auto-Export
Enable auto-export to automatically save your collection after each change:
1. Click "Auto" button
2. Confirm the prompt
3. Choose save location for each auto-save

### Import Options
When importing, choose how to handle existing snippets:
- **Merge**: Add new snippets, skip duplicates (recommended)
- **Replace**: Replace entire collection with imported snippets
- **Append**: Add all snippets (may create duplicates)

### Font Scaling
Adjust font size for better readability:
- Press `+` to increase font size (70% - 200% range)
- Press `-` to decrease font size
- Press `0` to reset to default size

### Search Tips
- Search works across all text fields (title, code, documentation)
- Use language filter to narrow results
- Combine search terms with filters for precise results
- Sort results by date, name, or language

## 🔧 Troubleshooting

### Common Issues

**Snippets not loading on startup**
- Solution: Use the Import button to load your `snippets-backup.json` file
- Note: Auto-loading from file system is blocked by browser security

**Export not working**
- Modern browsers: Native save dialog should appear
- Older browsers: File downloads to default Downloads folder
- Check browser permissions for file access

**Keyboard shortcuts not working**
- Ensure no input fields are focused
- Some shortcuts only work in specific contexts (browse vs. modal)
- Check if browser extensions are intercepting key combinations

**Mobile layout issues**
- Try refreshing the page
- Clear browser cache if layout appears broken
- Ensure browser zoom is at 100%

**Import/Export errors**
- Verify JSON file format is correct
- Check file permissions
- Try smaller file sizes if importing large collections

### Browser Permissions

For optimal functionality, allow these permissions:
- **File System Access**: For native save dialogs (Chrome/Edge)
- **Clipboard Access**: For paste functionality
- **Local Storage**: For temporary data handling

## 📄 License

This project is released under the MIT License. Feel free to modify and distribute as needed.

## 🤝 Contributing

This is a single-file application designed for simplicity and portability. To contribute:

1. Test changes thoroughly across different browsers
2. Maintain compatibility with mobile devices
3. Keep the single-file architecture
4. Document any new features or changes

## 📞 Support

For issues or questions:
1. Check the troubleshooting section above
2. Verify browser compatibility
3. Test with a fresh browser session
4. Check browser console for error messages

---

**Version**: 1.0.0  
**Last Updated**: December 2024  
**Compatibility**: Modern browsers supporting ES6+
