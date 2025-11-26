# Private Diary 📖

A modern, privacy-focused digital diary application that runs entirely in your browser. Your thoughts stay local, secure, and private.

## ✨ Features

### 🗄️ IndexedDB Storage
- **Local-first approach**: All data is stored locally in your browser using IndexedDB
- **No server dependency**: Works completely offline without any external servers
- **Privacy guaranteed**: Your entries never leave your device
- **Persistent storage**: Data survives browser restarts and system reboots
- **Performance benefits**: Fast read/write operations with efficient data retrieval

### 🎨 Theme Toggle
- **Smart theme detection**: Automatically respects your system's dark/light mode preference
- **Manual override**: Toggle between dark and light themes with a single click
- **Persistent preference**: Theme choice is saved in localStorage and remembered across sessions
- **Smooth transitions**: CSS variables ensure seamless theme switching

### 📤 Share Functionality
- **Native sharing**: Uses the Web Share API for seamless sharing on supported devices
- **Cross-platform compatibility**: Integrates with your device's native share menu
- **Fallback support**: Graceful degradation for older browsers and WebView environments
- **Context-aware**: Shares entries with date context for better organization

### 💾 Auto-Save
- **Real-time saving**: Automatically saves your entries as you type (500ms delay)
- **No data loss**: Prevents accidental loss of content during editing
- **Smart detection**: Only saves when there's actual content to preserve
- **Background operation**: Saves silently without interrupting your writing flow

### ↩️ Undo Functionality
- **Revert changes**: Undo button restores original text before editing
- **Smart restoration**: Handles both new entries and edited existing entries
- **Storage cleanup**: Automatically removes auto-saved entries when undoing
- **State management**: Maintains proper entry state throughout the undo process

### 🔍 Advanced Search
- **Powered by MiniSearch**: Uses the MiniSearch library for fast, fuzzy text search
- **Intelligent matching**: Supports partial matches, typos, and prefix searching
- **Date prioritization**: Search results prioritize date matches for better relevance
- **Live results**: Real-time search results as you type
- **Quick navigation**: Click any search result to jump directly to that date
- **Preview snippets**: Shows text previews in search results for context

### 📱 Mobile-First Design
- **Responsive layout**: Optimized for all screen sizes from mobile to desktop
- **Touch-friendly**: Large tap targets and intuitive gesture support
- **WebView ready**: Perfect for embedding in mobile applications
- **Progressive Web App**: Includes manifest for "Add to Home Screen" functionality
- **Offline capable**: Service worker enables full offline functionality
- **Mobile instructions**: Automatic detection and guidance for mobile users

### 📅 Interactive Calendar
- **Visual overview**: Month view with clear indicators for days with entries
- **Smart navigation**: Previous/Next month buttons and "Today" quick access
- **Entry indicators**: Visual dots show which days have diary entries
- **Date selection**: Click any past date to view or add entries
- **Future protection**: Prevents creating entries for future dates
- **Today highlighting**: Current date is clearly marked and emphasized

### ⌨️ Keyboard Shortcuts
- **Ctrl + Enter**: Quick save and close entry form
- **Intuitive editing**: Standard text editing shortcuts work as expected
- **Accessibility**: Full keyboard navigation support

### 🎯 User Experience
- **Clean interface**: Minimalist design focuses on your content
- **Smooth animations**: Subtle transitions enhance the user experience
- **Visual feedback**: Hover effects and state changes provide clear interaction cues
- **Error prevention**: Confirmation dialogs for destructive actions
- **Loading states**: Proper handling of asynchronous operations

## 🚀 Getting Started

1. **Open the app**: Simply open `diary.html` in any modern web browser
2. **Start writing**: Click on today's date and hit "Add Entry"
3. **Navigate**: Use the calendar to browse different dates
4. **Search**: Use the search box to find specific entries
5. **Customize**: Toggle between light and dark themes

## 💻 Technical Details

### Browser Compatibility
- **Modern browsers**: Chrome, Firefox, Safari, Edge (latest versions)
- **Mobile browsers**: iOS Safari, Chrome Mobile, Samsung Internet
- **WebView support**: Android WebView, iOS WKWebView
- **Progressive enhancement**: Graceful degradation for older browsers

### Dependencies
- **MiniSearch**: Lightweight full-text search engine
- **Bootstrap Icons**: Icon font for UI elements
- **No frameworks**: Pure vanilla JavaScript for maximum compatibility

### Storage Specifications
- **Database**: IndexedDB with structured object stores
- **Capacity**: Virtually unlimited storage (subject to browser quotas)
- **Data format**: JSON-structured entries with timestamps
- **Backup**: Data can be exported through browser developer tools

### Performance Features
- **Lazy loading**: Calendar renders efficiently for any month/year
- **Debounced search**: Search queries are optimized to prevent excessive processing
- **Memory management**: Efficient DOM manipulation and event handling
- **Caching**: Smart caching of DOM elements and computed values

## 🔒 Privacy & Security

- **100% local**: No data transmission to external servers
- **No tracking**: No analytics, cookies, or user tracking
- **Secure storage**: IndexedDB provides secure, sandboxed storage
- **XSS protection**: All user input is properly escaped and sanitized
- **Offline-first**: Works without internet connection

## 📱 Mobile Installation

### Android
1. Open Chrome browser
2. Navigate to the diary app
3. Tap menu (⋮) → "Add to Home Screen"
4. Confirm installation

### iOS
1. Open Safari browser
2. Navigate to the diary app
3. Tap Share button → "Add to Home Screen"
4. Confirm installation

## 🛠️ Development

The app is built with:
- **HTML5**: Semantic markup and modern web standards
- **CSS3**: Custom properties, Grid, Flexbox, and responsive design
- **Vanilla JavaScript**: ES6+ features with async/await
- **Web APIs**: IndexedDB, Web Share API, Service Worker

## 📄 License

MIT License
Created by Alexander Kaydansky (kaydansky@gmail.com) - 2025

## 🤝 Contributing

This is a single-file application designed for simplicity and portability. Feel free to fork and customize for your needs.

---

*Keep your thoughts private, secure, and always accessible.* ✨