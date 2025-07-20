# Vue Demo App - Simple Counter Application

A clean and simple Vue 3 demonstration application featuring a counter with increment/decrement functionality. Perfect for showcasing Vue.js basics and AWS Amplify deployment.

## ✨ Features

- 🎯 **Vue 3 Composition API** - Modern reactive programming
- ⚡ **Vite Build Tool** - Fast development and optimized builds
- 🎨 **Clean UI Design** - Simple and elegant interface
- 📱 **Responsive Layout** - Works on all device sizes
- 🚀 **AWS Amplify Ready** - Pre-configured for deployment

## 🎮 Live Demo

Interactive counter with:
- ➕ Increment button
- ➖ Decrement button
- Real-time value display
- Smooth hover animations

## 🚀 Quick Start

### Prerequisites

- Node.js 20 or higher
- npm or yarn package manager

### Local Development

1. **Navigate to the app directory**
   ```bash
   cd vue-amplify-app
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```

4. **Open your browser**
   Navigate to `http://localhost:5173`

### Build for Production

```bash
npm run build
```

The built files will be in the `dist/` directory.

## 🌐 AWS Amplify Deployment

This app is pre-configured for AWS Amplify deployment with an optimized `amplify.yml` file.

### Deploy to Amplify

1. **Connect to GitHub**
   - Log into the [AWS Amplify Console](https://console.aws.amazon.com/amplify/)
   - Click "New app" → "Host web app"
   - Connect your GitHub repository

2. **Configure Build Settings**
   - Select this repository
   - Set the root directory to `vue-amplify-app`
   - Amplify will automatically detect the `amplify.yml` file
   - The build configuration is optimized for Vue 3 + Vite

3. **Deploy**
   - Click "Save and deploy"
   - Your app will be available at a generated URL

### Manual Amplify CLI Deployment

```bash
# Install Amplify CLI
npm install -g @aws-amplify/cli

# Configure Amplify
amplify configure

# Initialize Amplify in your project
amplify init

# Add hosting
amplify add hosting

# Publish your app
amplify publish
```

## 📁 Project Structure

```
vue-amplify-app/
├── public/
│   ├── _redirects          # SPA routing configuration
│   └── vite.svg           # App icon
├── src/
│   ├── components/
│   │   └── HelloWorld.vue  # Demo component
│   ├── assets/
│   │   └── vue.svg        # Vue logo
│   ├── App.vue            # Main application component
│   ├── main.js            # Vue app initialization
│   └── style.css          # Global styles
├── amplify.yml            # Amplify build configuration
├── index.html             # HTML entry point
├── package.json           # Dependencies and scripts
├── vite.config.js         # Vite configuration
└── README.md              # This file
```

## 🛠️ Available Scripts

- `npm run dev` - Start development server with hot reload
- `npm run build` - Build for production with minification
- `npm run preview` - Preview production build locally

## 🔒 Security Features

The `amplify.yml` configuration includes:

- **Security Headers**: HSTS, CSP, X-Frame-Options, etc.
- **Content Security Policy**: Restricts resource loading for security
- **Optimized Caching**: Long-term caching for static assets
- **Production Optimizations**: Minification and compression

## 🎨 Customization

### Styling
- Modify `src/style.css` for global styles
- Update component styles in individual `.vue` files
- Colors use Vue.js brand colors (#42b883)

### Functionality
- Add new components in `src/components/`
- Extend the counter logic in `src/App.vue`
- Add routing with Vue Router if needed

## 📈 Performance

Built with performance in mind:
- ⚡ Vite for fast builds and HMR
- 🗜️ Automatic code splitting
- 📦 Optimized bundle size
- 💾 Efficient caching strategies

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License.

---

Built with ❤️ using Vue 3, Vite, and AWS Amplify
