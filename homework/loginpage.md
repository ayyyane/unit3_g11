# loginpage

## code
### loginpage.py

```.py

from kivymd.app import MDApp
from kivymd.uix.screen import MDScreen
from kivy.core.window import Window

class loginpage(MDApp):
    def build(self):
        return

class MainScreen(MDScreen):
    pass

class SecondScreen(MDScreen):
    pass

test = loginpage()
test.run()

```

### loginpage.kv
```.py
ScreenManager:
    id: main_scr
    MainScreen:
        name: "Login page"

    SecondScreen:
        name: "Signup page"

<MainScreen>:
    FitImage:
        size: 1,1
        source: "waterbottle.png"
    MDBoxLayout:
        size_hint: .8, .8
        md_bg_color: "white"
        orientation: "vertical"
        pos_hint:{"center_x": .5, "center_y": .5}

        MDLabel:
            pos_hint: {"center_x": .5, "center_y": .5}
            id: text
            font_size: "40pt"
            size: 1, 0.2
            halign: "center"
            text: "Login"

        MDTextField:
            id: username
            size: 1, 0.3
            text: "Enter username or email"
            font_size: "20pt"

        MDTextField:
            id: password
            size: 1, 0.3
            text: "Enter password"
            font_size: "20pt"

        MDBoxLayout:
            pos_hint: {"center_x": .5, "center_y": .7}
            size: 1, .2
            orientation: "horizontal"

            MDRaisedButton:
                id: Lg_button
                text: "Login"
                md_bg_color: "orange"
                size_hint_x: 0.45

            MDRaisedButton:
                id: Sg_button
                text: "Signup"
                md_bg_color: "red"
                size_hint_x: 0.45
                on_press:
                    root.parent.current = "Signup page"

<SecondScreen>:
    FitImage:
        size: 1,1
        source: "waterbottle.png"
    MDBoxLayout:
        size_hint: .8, .8
        orientation: "vertical"
        pos_hint:{"center_x": .5, "center_y": .5}
        md_bg_color: "white"

        MDLabel:
            halign: "center"
            id: text
            size: 1, .2
            font_size: "40pt"
            text: "Register"

        MDTextField:
            size: 1, .15
            id: username
            text: "Enter username or email"
            font_size: "15pt"

        MDTextField:
            size: 1, .15
            id: email
            text: "Enter email"
            font_size: "15pt"

        MDTextField:
            id: password
            size: 1, .15
            text: "Enter password"
            font_size: "15pt"

        MDTextField:
            id: confirm_password
            size: 1, .15
            text: "Enter password again"
            font_size: "15pt"

        MDBoxLayout:
            size: 1, .2
            orientation:"horizontal"
            padding: dp(10)

            MDRaisedButton:
                id: Sb_button
                #pos_hint: {"center_x":.2, "center_y":.5}
                text: "Submit"
                md_bg_color: "orange"
                size_hint_x: 0.45

            MDRaisedButton:
                id: Cn_button
                #pos_hint: {"center_x":.9, "center_y":.5}
                text: "Cancel"
                md_bg_color: "red"
                size_hint_x: 0.45
                on_press:
                    root.parent.current = "Login page"


```

## evidence

https://github.com/ayyyane/unit3_g11/assets/142702159/fd20b46d-5626-4ada-b482-147805c56285





https://github.com/ayyyane/unit3_g11/assets/142702159/54750d20-afae-4599-ae9b-69c67957c624




