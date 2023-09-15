# GitHub Actions self hosted runner

https://zenn.dev/kesin11/scraps/6a5eed6e2d5cba
を参考にカスタマイズしたもの。

## run

```
docker compose -p github-actions-self-hosted-runner up -d
```

## 変更点

- repo単位で動くように
- cypressが動くように
  + 参考：https://docs.cypress.io/guides/getting-started/installing-cypress#UbuntuDebian
  + ```
    apt-get update
    apt-get -y install libgtk2.0-0 libgtk-3-0 libgbm-dev libnotify-dev libgconf-2-4 libnss3 libxss1 libasound2 libxtst6 xauth xvfb
    ```
- `nanasess/setup-php`
  + `bc`が動くように
    * apt-get -y install bc
  + `apt-fast`が動くように
    * 参考：https://c-a-p-engineer.github.io/tech/2022/09/25/linux-apt-fast/
    * ```
      add-apt-repository ppa:apt-fast/stable
      apt-get update
      apt-get -y install apt-fast
      ```
