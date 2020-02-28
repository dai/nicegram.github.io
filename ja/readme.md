# Nicegram 翻訳
Nicegram はすべてのユーザーが最高の体験を得られるよう最適な言語環境を提供したいと願っています。

Nicegram は翻訳、スペルチェック及び新規言語/翻訳の提案をしてくれる皆さまを歓迎します！

## Translate App

翻訳にあたって気づきがありましたら公式の翻訳プラットフォーム [official translations](https://translations.telegram.org/ja/ios/) をご参照ください。

翻訳に関する議論は

Nicegram翻訳: [https://translate.nicegram.app](https://translate.nicegram.app)

または

[@Kylmakalle](https://t.me/Kylmakalle) まで直接ご連絡ください。翻訳の完了報告もこちらでお伝えいただければアプリへの追加作業が早まります。

## Translate Articles

It's hard to control translations via [telegra.ph](https://telegra.ph) or other platforms. So now Nicegram using this website.

Steps to translate:


0) Fork/Download [this repo](https://github.com/nicegram/nicegram.github.io)

1) Create new `<lang>` folder with `readme.md`. Translation will be available at `https://nicegram.app/<lang>`

2) For each article create separated folder. Translation will be available at `https://nicegram.app/<lang>/<folder>`

3) For referencing other article, use `[Text](/<lang>/article)`

4) If you're translating images too, create folder `images` inside. If not, you can reference original (english) images with string like `../../faq/images/banner.png`

5) **Recommendation:** Try to use local `images` folder instead of images url, because some hostings can be blocked in your country.

6) Add article links to main page if you've done a new translation.

7) Submit a pull-request and ping [@Kylmakalle](https://t.me/Kylmakalle)

Please, do not translate `chats` section, just refer to `/chats`

You can use [this folder](https://github.com/nicegram/nicegram.github.io/tree/master/ru) with Russian translation as example.

[Example Pull Request](https://github.com/nicegram/nicegram.github.io/pull/1) for addding Turkish translation.


### Header Anchors (FAQs).

Small python script that will create a header which you can insert in table of contents. (not sure if works for chinese)

Online: [https://repl.it/repls/SpecificIndigoOperatingsystem](https://repl.it/repls/SpecificIndigoOperatingsystem) (hit Run)


Local:

```python
import string


def sanitize(s):
    return "#" + s.lower().translate(str.maketrans('', '', string.punctuation)).replace(' ', '-')


while True:
    st = input('Enter header: ')
    print('\n')
    print(sanitize(st))
    print('\n')
```


Thank you in advance!
