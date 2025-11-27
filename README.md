# Private Diary 📖

A PWA (Progressive Web App), privacy-focused digital diary application that runs entirely in your browser. Your thoughts stay local, secure, and private unless explicitly shared. Track your life daily, then recall your memories with ease, it's fun.

## 📸 Screenshot

![Private Diary App](screenshot.png)
- *The clean, intuitive interface of Private Diary showing the calendar view and entry form*

## 🚀 Progressive Web App Benefits

- **Works completely offline**: After your first visit, the app works without internet connection thanks to Service Worker technology
- **Works offline forever**: Once cached, the app works offline permanently - no internet required
- **Auto-updates when new version pushed**: When new versions are released, they automatically update on your next visit
- **Works on phone without installing anything**: Just add to home screen for native app experience
- **Native app experience**: Runs in fullscreen mode without browser UI when installed
- **Cross-platform**: Works identically on Android, iOS, Windows, Mac, and Linux

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

### 🌐 Online Access
1. **Visit the app**: Go to https://kaydansky.github.io/private-diary-pwa
2. **Start immediately**: No registration, downloads, or setup required
3. **Your data stays local**: Even though the app is hosted online, all your diary entries are stored only on your device

### 📱 Add to Home Screen
**Android (Chrome/Edge):**
1. Visit the app URL in your browser
2. Tap the menu (⋮) → "Add to Home Screen" or "Install App"
3. Confirm installation
4. Launch from your home screen like any native app

**iOS (Safari):**
1. Visit the app URL in Safari
2. Tap the Share button (□↗) → "Add to Home Screen"
3. Confirm installation
4. Launch from your home screen

**Desktop (Chrome/Edge):**
1. Visit the app URL
2. Click the install icon (⊕) in the address bar
3. Or go to Settings → "Install Private Diary"

### 🔒 Privacy Note
Even though the app is accessed via a public URL, **all your diary entries remain 100% private and local to your device**. The online hosting only delivers the app code - your personal data never leaves your device.

### ✍️ Using the App
1. **Start writing**: Click on today's date and hit "Add Entry"
2. **Navigate**: Use the calendar to browse different dates
3. **Search**: Use the search box to find specific entries
4. **Share**: Click 3 dots next to an entry → "Share", "Edit" and "Delete" options
4. **Customize**: Toggle between light and dark themes

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

## 💻 Local Development

If you want to run the app locally:
1. Download `index.html` from the repository
2. Open it in any modern web browser
3. The app works identically to the online version

## 🛠️ Development

The app is built with:
- **HTML5**: Semantic markup and modern web standards
- **CSS3**: Custom properties, Grid, Flexbox, and responsive design
- **Vanilla JavaScript**: ES6+ features with async/await
- **Web APIs**: IndexedDB, Web Share API, Service Worker

## 📄 License

This project is released under the MIT License.

## 🤝 Contributing

This is a single-file application designed for simplicity and portability. Feel free to fork and customize for your needs.

---

*Keep your thoughts private, secure, and always accessible.* ✨