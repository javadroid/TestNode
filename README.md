<!-- 
import axios from "axios";
import express from "express";
import dotenv from "dotenv";
import { createEmailCpanel } from "create-emails";

dotenv.config();
const cpanelHost = process.env.cpanelHost;
const cpanelUsername = process.env.cpanelUsername;
const cpanelPassword = process.env.cpanelPassword;

const app = express();
app.use(express.json());

//get return hello word
app.get("/", (req, res) => {
  res.send("Hello World!");
});
  

// app.post("/create-email-cpanel", async (req, res) => {
//   const { domain, email, password, cpanelUser, cpanelPass } = req.body;

//   const authPanel = {
//     cpanelHost,
//     username: cpanelUser || cpanelUsername,
//     password: cpanelPass || cpanelPassword,
//   };
//   if (!domain || !email || !password) {
//     return res.status(400).json({ error: "Missing required fields" });
//   }

//   const data = {
//     domain,
//     email,
//     password,
//     quota: 100,
//   };

//   try {
//     console.log(data,authPanel)
//     const response = await createEmailCpanel(data, authPanel);
//     console.log(response)
//     if (response?.status == 1) {
//       return res.json(response);
//     }
//     return res.status(405).json(response);
//   } catch (error) {
//     res.status(500).json({ error: error.message });
//   }
// });

const PORT = process.env.PORT || 3006;
app.listen(PORT, () => {
  console.log(`Server is running on port ${PORT}`);
});
 -->

write  a readme 
# Email Cpanel API

This is a simple API that allows you to create email accounts on a cPanel server.

## Installation

1.  Clone the repository:

    ```bash
    git clone <repository-url>
    ```

2.  Install dependencies:

    ```bash
    npm install
    ```

## Usage

1.  Start the server:

    ```bash
    npm start
    ```

2.  The server will be running on port 3006 (or the port you specified in the `.env` file).

## Endpoints

### `GET /`

-   Returns a "Hello World!" message.

