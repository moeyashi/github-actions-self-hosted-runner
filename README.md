# GitHub Actions self hosted runner

https://zenn.dev/kesin11/scraps/6a5eed6e2d5cba
を参考にカスタマイズしたもの。

## 変更点

- cypressが動くように
  + 参考：https://docs.cypress.io/guides/getting-started/installing-cypress#UbuntuDebian
  + ```
    apt-get update
    apt-get -y install libgtk2.0-0 libgtk-3-0 libgbm-dev libnotify-dev libgconf-2-4 libnss3 libxss1 libasound2 libxtst6 xauth xvfb
    ```
