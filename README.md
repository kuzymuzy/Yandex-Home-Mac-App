# Yandex-Home-Mac-App
***Yandex не имеет отношения к этому приложению, оно сделано мной на коленке***

Приложение "Дом с Алисой" для macOS, основано на Electron Framework.

Оригинальный app для ios использует просто вебсайт, зная ссылку я собрал полноценое app под macOS.

Работает этот app с macOS 10.13, про баги писать даже не стоит, все либо в yandex либо молчать в тряпочку)))

# Для тех кто дофига параноик
Рассказываю как собрать такое вручную на своем mac:
1. Качаем node.js с официального сайта, или ставим brew, точно так же с официального сайт.
2. Ставим nativefier
```bash
  npm install -g nativefier
```

Для Home Brew

```bash
  brew install nativefier
```
3. Билдем апликуха. (В моей есть красивая иконка, можете взять ее кинул в main и добавить ее через "-i '/путь/до/иконки.icns'")

```bash
nativefier "https://yandex.ru/iot" --name "Yandex Home" --platform=mac --width 407 --height 756 --disable-dev-tools -f --lang=ru --disable-context-menu --portable
```

# Если мне будет не лень я сделаю такое и для Windows)
