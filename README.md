### Alestro Handler


Author: Gabriel7zoo

📋 Description

Alestro Handler is a Discord bot template built for discord.js v14, designed to make it easy to create and manage your own Discord bot. This project includes a command and event handler, allowing users to quickly set up a robust, modular bot framework.

This handler allows you to:

Manage commands and events in separate files.

Easily extend and maintain your bot.

Keep your bot's codebase clean and organized.



---

## 🆕 What's New in Version 2.0.0

Updated for discord.js v14 compatibility.

Dependency versions upgraded to the latest for 2024.

Improved stability and bug fixes.

Custom Brisvi License added, allowing modification and public/private usage with credit.



---

### 🚀 Getting Started

Prerequisites

To run the Alestro Handler project, you need to have the following installed:

Node.js: >= v16.9.0
(Ensure you have Node.js installed here. Version 16.9.0 or higher is required for discord.js v14.)

npm: Comes with Node.js. You can check the version with:

npm -v

discord.js: ^14.13.0
(This will be installed automatically when you run npm install.)


## Installation

Follow these steps to install and set up the project:

1. Clone the repository:

git clone https://github.com/gabriel7zoo/Alestro_Base_Handler.git
cd Alestro_Base_Handler


2. Install all dependencies:

npm install


3. Create a .env file:

Set your Discord bot token and other configuration values in a .env file (e.g., TOKEN=your-bot-token).



## 4. Start the project:

node index.js




---

## 🛠️ How to Use

This project comes with a structured file organization that simplifies handling multiple commands and events. Here's how to work with it:

Adding Commands

1. Create a new command in the commands/ directory.


2. Each command file should export a data object and execute function. Example command:



const { SlashCommandBuilder } = require('discord.js');

module.exports = {
  data: new SlashCommandBuilder()
    .setName('ping')
    .setDescription('Replies with Pong!'),
  async execute(interaction) {
    await interaction.reply('Pong!');
  },
};

Adding Events

1. Create a new event in the events/ directory.


2. Example event for ready.js:



module.exports = {
  name: 'ready',
  once: true,
  execute(client) {
    console.log(`Logged in as ${client.user.tag}`);
  },
};


---

## 🧑‍💻 Contributing

Bug Fixes: Only open pull requests (PRs) for bug fixes. We aim to keep the code as clean and minimal as possible.

Custom Forks: Feel free to fork and modify the project for personal or public use, but be sure to follow the Brisvi License and credit Gabriel7zoo.



---

## ⚙️ Project Dependencies

This project relies on the following libraries:


---

## 📄 License

This project is licensed under the Brisvi License.
You can modify and run this project privately or publicly, but you must give credit to the original author, Gabriel7zoo. The author is not responsible for any damage caused by the use of this program. Users have permission to run, fork, and modify the project as long as they provide proper credit and do not misuse it. For full license terms, see the LICENSE file.


---

## 👨‍🏫 Support & Issues

If you encounter any issues or have questions, feel free to:

Open an issue on the GitHub repository.

Submit a bug fix via pull request.


Happy coding! 🎉
