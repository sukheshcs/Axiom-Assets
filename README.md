# Axiom Assets - Enterprise IT Asset Management

Axiom Assets is a robust, Electron-based desktop application designed for comprehensive IT asset management. It combines a modern React frontend with a secure Node.js/Express backend to provide a seamless experience for tracking hardware, software, and employee allocations.

## Key Features

- **Interactive Dashboard**: Real-time overview of asset distribution, stock status, and recent activities.
- **Asset Lifecycle Management**: distinct tracking for Hardware (Infra) and Software assets.
- **Employee Management**: Link assets to employees, track history, and manage details.
- **Reports & Analytics**: Generate detailed reports on employee assets, stock levels, and more.
- **Workflow Automation**: customize workflow templates and track request statuses.
- **Cross-Platform**: Built with Electron for reliable desktop performance on Windows.

## Technology Stack

### Core
- **Electron**: Desktop container
- **Node.js**: Runtime environment

### Frontend (Client)
- **React**: UI Library
- **Vite**: Build tool and dev server
- **Tailwind CSS**: Utility-first styling (inferred from standard practices, adjustable if custom CSS is used)
- **Framer Motion**: Animations
- **Chart.js**: Data visualization

### Backend (Server)
- **Express**: Web framework
- **SQLite / MS Access**: Database connectivity via `better-sqlite3` and `node-adodb`

## Prerequisites

- [Node.js](https://nodejs.org/) (Latest LTS recommended)
- [npm](https://www.npmjs.com/) (comes with Node.js)

## Installation

1.  **Clone the repository**
    ```bash
    git clone <repository-url>
    cd axiom-assets-desktop
    ```

2.  **Install Root Dependencies**
    ```bash
    npm install
    ```

3.  **Install Backend Dependencies**
    ```bash
    cd server
    npm install
    ```

4.  **Install Frontend Dependencies**
    ```bash
    cd ../client
    npm install
    ```

## Development

To run the application in development mode (with hot-reload for client/server):

1.  **Return to the root directory**
    ```bash
    cd ..
    ```

2.  **Start All Services**
    ```bash
    npm run dev
    ```
    This command concurrently starts the Express server, the Vite dev server, and the Electron window.

## Building for Production

To create a deployable Windows installer or portable executable:

```bash
npm run build:win
```
The output will be generated in the `dist` directory.

## License

This project is licensed under the ISC License.

## Author

Sukhesh Publisher
