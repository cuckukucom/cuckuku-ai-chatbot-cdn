# 💬 Chatbot Widget

A lightweight and customizable chatbot widget that can be easily integrated into any website or web application.

## ✨ Features

- 🚀 Easy integration with any framework
- 🎨 Customizable themes via JSON configuration
- 📱 Responsive design
- ⚡ Lightweight and fast
- 🔧 Simple configuration

## 📦 Installation

### 🌐 CDN Integration (HTML/ReactJs for index.html)

Add the following code to your HTML file:

```html
<!-- Add CSS -->
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/gh/cuckukucom/cuckuku-ai-chatbot-cdn@v1.0.0/chatbot.css"
/>

<!-- Add JavaScript -->
<script src="https://cdn.jsdelivr.net/gh/cuckukucom/cuckuku-ai-chatbot-cdn@v1.0.0/chat.bundle.iife.js"></script>

<!-- Initialize the chatbot -->
<script>
  ChatWidget.createChat({
    themeConfigUrl: "/themeConfig.json",
  });
</script>
```

### ⚡ Vue.js Integration

For Vue.js applications, add the widget in your component:

```vue
<template>
  <!-- Your component content -->
</template>

<script setup>
import { onMounted } from "vue";

onMounted(() => {
  // Add CSS
  const link = document.createElement("link");
  link.rel = "stylesheet";
  link.href =
    "https://cdn.jsdelivr.net/gh/cuckukucom/cuckuku-ai-chatbot-cdn@v1.0.0/chatbot.css";
  document.head.appendChild(link);

  // Load and initialize chatbot
  const script = document.createElement("script");
  script.src =
    "https://cdn.jsdelivr.net/gh/cuckukucom/cuckuku-ai-chatbot-cdn@v1.0.0/chat.bundle.iife.js";
  script.onload = () => {
    if (window.ChatWidget && window.ChatWidget.createChat) {
      window.ChatWidget.createChat({
        themeConfigUrl: "/themeConfig.json",
      });
    }
  };
  document.head.appendChild(script);
});
</script>
```

### 🔥 Nuxt.js Integration

For Nuxt.js applications, add the widget in your `app.vue` or component:

```vue
<template>
  <!-- Your app content -->
</template>

<script setup>
onMounted(async () => {
  if (process.client) {
    // Add CSS
    const link = document.createElement("link");
    link.rel = "stylesheet";
    link.href =
      "https://cdn.jsdelivr.net/gh/cuckukucom/cuckuku-ai-chatbot-cdn@v1.0.0/chatbot.css";
    document.head.appendChild(link);

    // Load and initialize chatbot
    const script = document.createElement("script");
    script.src =
      "https://cdn.jsdelivr.net/gh/cuckukucom/cuckuku-ai-chatbot-cdn@v1.0.0/chat.bundle.iife.js";
    script.onload = () => {
      if (window.ChatWidget && window.ChatWidget.createChat) {
        window.ChatWidget.createChat({
          themeConfigUrl: "/themeConfig.json",
        });
      }
    };
    document.head.appendChild(script);
  }
});
</script>
```

<!-- ## ⚙️ Configuration

### Theme Configuration

Create a `themeConfig.json` file in your public directory to customize the chatbot appearance:

```json
{
  "primaryColor": "#007bff",
  "backgroundColor": "#ffffff",
  "textColor": "#333333",
  "borderRadius": "8px",
  "position": "bottom-right"
}
```

### Available Options

| Option           | Type    | Default        | Description                               |
| ---------------- | ------- | -------------- | ----------------------------------------- |
| `themeConfigUrl` | string  | Required       | URL to your theme configuration JSON file |
| `position`       | string  | `bottom-right` | Widget position on screen                 |
| `autoOpen`       | boolean | `false`        | Automatically open chat on page load      |

## 🚀 Quick Start

1. **Copy the integration code** for your framework
2. **Create a `themeConfig.json`** file in your public directory
3. **Customize the theme** according to your brand
4. **Test the integration** on your website

## 📝 Examples

Check out the [examples directory](./examples) for complete implementation examples in various frameworks.

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License.

## 🆘 Support

If you encounter any issues or have questions, please [open an issue](https://github.com/cuckukucom/cuckuku-ai-chatbot-cdn/issues) on GitHub. -->

## Just git add, commit, push and you are done