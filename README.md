#### Hello!, I'm <a href="https://www.techdro.id/">Adek</a>.<img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="25px">


<a href="https://t.me/adekys">
  <img align="right" alt="Adek's Telegram" width="20px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/telegram.svg" />
</a>
<a href="https://www.instagram.com/adek.maulana/">
  <img align="right" alt="Adek's Instagram" width="20px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/instagram.svg" />
</a>
<a href="https://www.facebook.com/profile.php?id=100003779094856">
  <img align="right" alt="Adek's Facebook" width="20px" src="https://cdn.jsdelivr.net/npm/simple-icons@v3/icons/facebook.svg" />
</a>  
<details>	
  <summary><b>Github Stats</b></summary>

<img alt="" src="https://github-readme-stats.vercel.app/api?username=adekmaulana&show_icons=true&hide_border=true" />
</details>


<img src="https://camo.githubusercontent.com/992babdffd8c74a1502de375fbdf7e4d54773242/68747470733a2f2f6d656469612e67697068792e636f6d2f6d656469612f53576f536b4e36447854737a71494b4571762f67697068792e676966" width="495px">

```python3

from dataclasses import dataclass
from typing import Tuple


class Meta(type):
    def __new__(cls, name, bases, attrs):
        for attr in attrs:
            if not attr.startswith("_"):
                __annotations__[attr] = Tuple[str, ...]
        attrs["__annotations__"] = __annotations__
        new_cls = super().__new__(cls, name, bases, attrs)
        new_cls = dataclass(new_cls)
        return new_cls


class Stack(metaclass=Meta):
    languages   = ("Python", "Bash")
    ongoing     = ("C")


print("A little more about me")

adek = {
    'pronouns': 'he' or 'him' or 'his',
    'fullname': 'Muhammad Yusril Syahruddin',
    'othername': ['Sinyo', 'Iyus'],
    'nationality': ['Indonesia', 'ID'],
    'location': 'Surabaya, ID',
    'contact': {
        'email': 'yusrilsyahruddin@gmail.com',
    },
    'about': [
        'A student',
        'A fan of python',
        'I\'m considering myself as a runner. (even tho rarely do it) xd',
        'Love gaming',
        'Human.',
        'Still don\'t know how to feel about Last of Us 2 ending'
    ],
    'game': ['Granado Espada', 'Blade & Soul Revolution']
}
```
