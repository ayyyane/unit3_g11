# quiz042

## prompt
<img width="788" alt="Screenshot 2024-01-26 at 17 58 09" src="https://github.com/ayyyane/unit3_g11/assets/142702159/6882380b-ced2-4bef-87b9-39b0e2b51550">

## solution

```.py
# quiz041.py

from kivymd.app import MDApp
from kivymd.uix.screen import MDScreen

class mystery(MDApp):
    def build(self):
        return

class SecondScreen(MDScreen):
    pass

class MainScreen(MDScreen):
    def change_to_page2(self):
        print("changing to page 2")
        self.parent.current = "MysteryPageB"


test = mystery()
test.run()

# mystery.kv
ScreenManager:
    id: main_scr

    MainScreen:
        name: "MysteryPageA"

    SecondScreen:
        name: "MysteryPageB"


<MainScreen>:
    MDLabel:
        id: text1
        text: "This is mystery page A you pressed the button"



    MDRaisedButton:
        on_press:
            root.change_to_page2()


<SecondScreen>:
    MDLabel:
        id: text2
        text: "This is mystery page B you pressed the button"

    MDRaisedButton:
        on_press:
            root.parent.current = "MysteryPageA"


```

## evidence
<img width="499" alt="Screenshot 2024-01-26 at 19 15 35" src="https://github.com/ayyyane/unit3_g11/assets/142702159/b9a07726-71d7-4949-b5e8-110b8fc076ea">

<img width="603" alt="Screenshot 2024-01-26 at 19 15 41" src="https://github.com/ayyyane/unit3_g11/assets/142702159/bc33cdcd-89cb-4e2e-a467-9a88af530bed">


https://github.com/ayyyane/unit3_g11/assets/142702159/cce754bc-5fba-4495-b779-9a8a0e6dd844

