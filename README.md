# axewell UI

<img src="public/logo.png" alt="axewell UI Logo" width="180">

Project focused on creating a completely new VUE-based frontend that integrates with the existing Bitaxe firmware as altertative to AxeOS.

Download latest release: [www.bin](https://github.com/ruchus/axewell-UI/releases)

Just upload the file above to your Bitaxe. Don't worry about updating axewell UI, if you don't like it you can go back to AxeOS from the settings page by re-uploading the AxeOS www .bin

Discuss about the project on [Discord](https://discord.gg/6XYuqTXR)

# Some screenshots

<img width="1480" height="880" alt="1" src="https://github.com/user-attachments/assets/395bc541-79f2-4ac3-8f9b-12df8aed6b62" />

<img width="1481" height="881" alt="2" src="https://github.com/user-attachments/assets/264a9f80-dd48-4897-881a-da5522b5c6e8" />

<img width="1498" height="882" alt="3" src="https://github.com/user-attachments/assets/b58e9c73-9ade-4b91-9bb9-c1f426a36d5c" />

<img width="1484" height="879" alt="4" src="https://github.com/user-attachments/assets/8b74af4b-34f6-489a-9506-6cdd496f61a7" />

## Features

A modern, high-performance web interface for **Bitaxe** ASIC miners. axewell UI provides a comprehensive dashboard to monitor, manage, and optimize your mining hardware with a focus on aesthetics, responsiveness, and user experience.

- **Real-time Dashboard**: Monitor hashrate (Gh/s), power consumption (W), and efficiency (J/Th) in real-time.
- **Swarm Management**: Monitor multiple devices on your network from a single interface.
- **Detailed Metrics**: View accepted/rejected shares, error percentages, and performance graphs.
- **Electricity Cost Calculator**: Estimation of daily, monthly, and yearly costs with multi-currency support.
- **Custom parameters**: Tune frequency, voltage, and pool settings directly from the UI.
- **Network Control**: Manage Wi-Fi connections and hostname settings.
- **Multi-language Support**: Available in multiple languages (English, Spanish, and more).
- **Dark Mode**: Optimized for both light and dark environments.
- **Fully Responsive**: Designed to look great on desktops, tablets, and smartphones.

## Tech Stack

- **Framework**: [Vue 3](https://vuejs.org/) (Composition API)
- **UI System**: [Quasar Framework](https://quasar.dev/)
- **State Management**: [Pinia](https://pinia.vuejs.org/) (with local storage persistence)
- **Build Tool**: [Vite](https://vitejs.dev/)
- **Communication**: [Axios](https://axios-http.com/)
- **Internationalization**: [Vue I18n](https://vue-i18n.intlify.dev/)

## Installation & Development

### Prerequisites

- [Node.js](https://nodejs.org/) (v18 or higher recommended)
- [npm](https://www.npmjs.com/)

### Setup

```bash
# Clone the repository
git clone https://github.com/ruchus/axewell-UI.git

# Install dependencies
npm install
```

### Development Mode

Runs the app in development mode with hot-reloading.

```bash
npm run dev
```

> **Note**: For development, is configured by default an API prefix in a `.env.development` file to route requests to a specific test server in order to projects works.
> `VITE_AXIOS_BASE_URL_PREFIX=https://apidevices.axewell.tech/api/test/bitaxe`

### Build for Production

Builds the application for production to the `dist` folder.

```bash
npm run build
```

The build process also includes post-build compression steps using `compress.js` and `only-gzip.js` to ensure the application is as lightweight as possible for firmware integration.

## Project Structure

- `src/pages/`: Main views (Dashboard, Swarm, Pool, Settings, etc.).
- `src/components/`: Reusable Vue components (Cards, Charts, Nav).
- `src/stores/`: Pinia stores for state management (Axe, Auth, etc.).
- `src/layouts/`: Basic layout wrappers.
- `src/plugins/i18n/`: Translation files and configuration.

## Contributing

If you are a developer, you are welcome to collaborate with the project! Feel free to open issues or submit pull requests. If not, you can still help us by purchasing your [Bitaxe Completion Kit](https://axewell.tech/).

---

_Made with ❤️ by the Axewell Team._
