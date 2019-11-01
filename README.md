# KV4Jetbrains

## Syntax highlighting and auto-completion for Kivy/KivyMD `.kv` files in PyCharm/Intellij IDEA
![kv_code](https://raw.githubusercontent.com/noembryo/KV4Jetbrains/master/img/kv.screen.2b.png)

This settings file is based on the one that is located at the
["Setting Up Kivy with various popular IDE's"](https://github.com/kivy/kivy/wiki/Setting-Up-Kivy-with-various-popular-IDE's) page of [Kivy@GitHub](https://github.com/kivy/kivy).  
It's **updated** and has also support for the **KivyMD** modules and properties.
___
There are 4 categories of keywords:
* **Modules** (e.g. `FloatLayout`, `Button`, `Image` ..)
* **Properties** (e.g. `text`, `source`, `size_hint_x` ..)
* **Actions** (e.g. `on_release`, `on_text`, `on_parent` ..)
* **Special** (The `app`, `cls`, `root`, `self`, `False`, `None`, `True` keywords)

The colors of these categories can be changed in
`Settings`>`Editor`>`Color Scheme`>`Custom`.

<p align="center">
  <a href="https://raw.githubusercontent.com/noembryo/KV4Jetbrains/master/img/kv.colors.png">
    <img src="https://raw.githubusercontent.com/noembryo/KV4Jetbrains/master/img/kv.colors.png" height="350"></a>
</p>

You can Add/Remove keywords by going to the
`Settings`>`Editor`>`File Types` and double click (edit) the `Kv Language` entry.

<p align="center">
  <a href="https://raw.githubusercontent.com/noembryo/KV4Jetbrains/master/img/kv.edit.png">
    <img src="https://raw.githubusercontent.com/noembryo/KV4Jetbrains/master/img/kv.edit.png" height="300"></a>
  <a href="https://raw.githubusercontent.com/noembryo/KV4Jetbrains/master/img/kv.keywords.png">
    <img src="https://raw.githubusercontent.com/noembryo/KV4Jetbrains/master/img/kv.keywords.png" height="300"></a>
</p>

_Also, feel free to inform me about missing keywords so that I can update the settings file._

___
## Installation instructions for PyCharm/Intellij IDEA:

* Click `File`>`Export Settings` and save a backup of your current settings
(in case something goes wrong)
* Download the `JetBrains.kvMD.completion.v0.x.jar` from the [releases](https://github.com/noembryo/KV4Jetbrains/releases)
* Click `File`>`Import Settings`
* Select the `.jar` file and a dialog will open.
* Click OK and restart PyCharm ;o)
___
## Semi-Language Injection to String Literals
_Added in v0.3_

PyCharm, IDEA (and all the JetBrains IDE's) support "Language Injection", a way to have
syntax highlighting inside the Python's string literals.  
Unfortunately, only the supported languages are supported (!)

There is a workaround (better than nothing, but not by much), to have something like this:

![kv_code](https://user-images.githubusercontent.com/24675403/67905219-4f350480-fb79-11e9-970d-09a5fb91074a.png)

You can read about it [here](https://github.com/noembryo/KV4Jetbrains/issues/2#issuecomment-548008947).

To use it, just select _all_ the `kv` code in the string, press `Ctrl+Alt+T` ("Surround
With...") and select the `KV. Surround for kv injection` entry.
