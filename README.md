# Depined Auto Ping and Auto Reff

![banner](image.png)

## Features

- **Auto Ping Widget Connection**
- **Support multiple accounts**
- **Support Proxy usage**

## Prerequisites

- Node.js installed on your machine
- `tokens.txt` file containing token from depined platform follow instruction below to get:
- Open depined dashboard [https://app.depined.org/dashboard](https://app.depined.org/dashboard)
- Login With your email
- inspect or just F12, and find Application
- in local storage find `token` and copy all value.
    ![token](image-1.png)

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/Vantone/depinedBot.git
    cd depinedBot
    ```

2. Install the required dependencies:
    ```sh
    npm install
    ```
3. Input your tokens in `tokens.txt` file, one user per line;
    ```sh
    nano tokens.txt
    ```
4. optionally you can use proxy: 
- paste proxy in `proxy.txt` format `http://username:password@ip:port` 
    ```sh
    nano proxy.txt
    ```
5. 启动脚本方式一:
    ```sh
    npm run start
    ```

## Additional Feature Auto Registration / Auto Referral
-   ```bash
    npm run autoreg
    ```
- accounts information saved at `accounts.txt` and tokens auto saved to `tokens.txt`
## 启动脚本方式二:

 -  docker版本部
   ```
   cd  ~
   git clone https://github.com/Vantone/depinedBot.git
   cd depinedBot
   docker pull node:20-alpine
   docker run -itd --restart always   --name depined  -v /root/depinedBot:/root/depinedBot  -w /root/depinedBot  node:20-alpine1  sh -c 'npm install && npm run start '
```

## ![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)

This project is licensed under the [MIT License](LICENSE).

