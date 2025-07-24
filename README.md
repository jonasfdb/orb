# The foundations of Orb

Orb is a fully-featured, actively maintained multi-purpose Discord bot with an emphasis on utility, community, and fun. For more information on the bot itself and for the invite link, visit [the support server on Discord](https://discord.gg/kUPz8dS7PM). For questions, feedback and suggestions, feel free to open an issue or submit a discussion!

## 📦 About This Repository

This is the official codebase of the Orb bot. You are welcome to explore the code, contribute improvements, and suggest new features. Everything is welcome! But heads up, this is meant for people interested in contributing or experimenting. While Orb can be hosted on a local machine under the terms of the license, but this is not officially supported at this point in time, and this repository will not provide help for issues on self-hosted instances for now. This repository also does not provide end-user support. For questions or support related to the hosted version of Orb, visit the homepage or the official Discord server.

## 🤝 Contribute to Orb

### Got an idea?

If you have an idea, a suggestion or a feature request, you can make your voice heard in two ways. Either you get in contact with me through [the support server on Discord](https://discord.gg/kUPz8dS7PM), or, preferably, you create an Issue or a Discussion on here. Both works fine!

### Contributing code

If you want to submit code directly, please fork the repo, create a new branch (`feature/your-change`), and submit a pull request with a clear commit message. I'd love to be able to ask you to adhere to the coding style, but in all fairness, my codebase is still mostly a mess and I am actively working on improving it.

## ⚙️ Requirements & Setup

### Prerequisites

You should have a Discord bot token available through your [Discord Developer Portal](https://discord.com/developers), and have [Node.js](https://nodejs.org) >20 and [PostgreSQL](https://www.postgresql.org/) >17.5 installed. This version of Orb was built and is running on Node.js 20.18.0 and PostgreSQL 17.5, using discord.js 14.20.0.

### Installation and Setup

Clone the repository into a new folder and run `npm install` to install the necessary packages. Then, create a `.env` file based on the structure in `.env.example` at `/config`, where `.env.example` is. Populate it with the necessary values.
Orb provides a development and a production version of each `.env` variable in case you want to run two instances at once. The `config` file determines which to supply to the bot on startup based on the environment flag at the bottom of `.env`, which you have to change accordingly.

### Run

Orb provides the following scripts through `package.json`:

```bash
npm start               # run compiled build using tsx
npm run build           # compile /src to JavaScript
npm run deployToBot     # deploy /src/commands to bot instance
npm run deployToServer  # deploy /src/commands to specific guild specified in .env
```

## ⚖️ License

This project is licensed under the **GNU Affero General Public License v3.0 (AGPL-3.0)**. See [`LICENSE`](./LICENSE) for the full text of the license and it's conditions. For a general overview, visit [this summary](https://choosealicense.com/licenses/agpl-3.0/).

Third-party packages used in this project and their respective licenses can be found in [`LICENSE`](./NOTICE.md).

## 💭 Contact

Orb is developed and maintained with love and care by me, jonasfdb. I can be found on Discord under the same username, feel free to talk to me (preferably through the Discord server though).
