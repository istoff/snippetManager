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
- **⌨️ Keyboard Navigation**: Full keyboard control with intuitive shortcuts
- **📱 Mobile Responsive**: Works seamlessly on desktop, tablet, and mobile
- **🎨 Font Scaling**: Adjustable font size for better readability
- **🎯 Visual Selection**: Clear highlighting for selected snippets
- **🌐 Cross-Platform**: Runs in any modern web browser

## 🚀 Quick Start

### Installation
1. Download or save the HTML file to your computer
2. Double-click to open in your default browser
3. Your snippets automatically save to browser storage as you work

### First Use
1. **Auto-loading**: Previously saved snippets load automatically when you open the app
2. **Import existing collection**: Click "Import" to load a `snippets-backup.json` file
3. **Create new snippet**: Click "New" or press `Insert` key
4. **Search and filter**: Use the search bar and language filter
5. **Export for backup**: Click "Export" to save your collection to a file

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
| `+` or `🔤+` button | Increase font size |
| `-` or `🔤-` button | Decrease font size |
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
1. **Morning**: Open snippet manager (auto-loads your previous work)
2. **During work**: Add snippets (auto-saves as you type)
3. **End of day**: Export backup to cloud storage for cross-device sync

### Cross-Device Sync
1. **Device A**: Create/modify snippets → Export to cloud storage
2. **Device B**: Import from cloud storage → Continue working (auto-saves locally)
3. **Repeat**: Keep collections synchronized by periodically exporting/importing

### Team Sharing
1. **Individual**: Curate personal collection (auto-saves locally)
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

### Auto-Save
Your snippets automatically save to browser storage as you work:
- ✅ **Continuous saving**: Every create, edit, or delete action auto-saves
- ✅ **Auto-loading**: Snippets reload automatically when you reopen the app
- ✅ **Browser persistence**: Data persists across browser sessions
- ⚠️ **Single browser**: Storage is specific to each browser/device

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
- Use `🔤+` and `🔤-` buttons in the header

### Search Tips
- Search works across all text fields (title, code, documentation)
- Use language filter to narrow results
- Combine search terms with filters for precise results
- Sort results by date, name, or language

## 🔧 Troubleshooting

### Common Issues

**Snippets not loading**
- Solution: Check if you have existing data in browser storage
- Alternative: Import a `snippets-backup.json` file to get started
- Note: Each browser stores data separately

**Lost snippets after browser update**
- Solution: Regular exports provide backup protection
- Prevention: Export your collection periodically to files
- Browser storage can be cleared by browser updates or cleanup tools

**Snippets not syncing between devices**
- Expected: Browser storage is device/browser-specific
- Solution: Use Export → Import workflow for cross-device sync
- Alternative: Enable Auto-Export for regular file backups

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
- **Local Storage**: Required for automatic snippet saving and persistence

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

**Version**: 1.0.1  
**Last Updated**: June 2025  
**Compatibility**: Modern browsers supporting ES6+