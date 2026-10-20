# Литературные иллюстрации для QR-кодов

Пять статических страниц с иллюстрациями к литературным произведениям. Каждая страница имеет отдельный адрес для ссылки из QR-кода.

| № | Произведение | Страница | Исходник |
|---|---|---|---|
| 1 | Хамелеон | [Открыть](https://xondell.github.io/qr-images/1/) | [HTML](docs/1/index.html) |
| 2 | Дети подземелья | [Открыть](https://xondell.github.io/qr-images/2/) | [HTML](docs/2/index.html) |
| 3 | Васюткино озеро | [Открыть](https://xondell.github.io/qr-images/3/) | [HTML](docs/3/index.html) |
| 4 | Капитанская дочка | [Открыть](https://xondell.github.io/qr-images/4/) | [HTML](docs/4/index.html) |
| 5 | Тарас Бульба | [Открыть](https://xondell.github.io/qr-images/5/) | [HTML](docs/5/index.html) |

## Локальный просмотр

Нужны Git, Python 3 и браузер. Сборка и npm не требуются.

```bash
git clone https://github.com/xondell/qr-images.git
cd qr-images
python3 -m http.server 8000 --directory docs
```

Откройте [http://localhost:8000](http://localhost:8000). Страницы произведений доступны по путям `/1/`–`/5/`.

## Структура и обновление

Опубликованные файлы находятся в [docs](docs). В каждой нумерованной папке лежат `index.html` и `poster.png`; [docs/index.html](docs/index.html) служит общей точкой входа.

Чтобы заменить иллюстрацию, обновите соответствующий `poster.png`, сохранив папку и имя файла: существующий QR-код продолжит вести на тот же адрес. Проверьте страницу на телефоне после публикации.

Для GitHub Pages используется содержимое папки `/docs`; [.nojekyll](docs/.nojekyll) отключает обработку Jekyll. Ссылки выше рассчитаны на адрес `https://xondell.github.io/qr-images/`.
