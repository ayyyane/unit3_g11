# quiz040

## prompt
<img width="786" alt="Screenshot 2024-01-26 at 17 57 08" src="https://github.com/ayyyane/unit3_g11/assets/142702159/aceb8fc3-f5f6-4053-ae2f-c3cd574ec544">


## solution

```.py

# quiz040.py

from kivymd.app import MDApp

class quiz041(MDApp):
    def build(self):
        return

    def pressed_button(self):
        button_color = self.root.ids.text
        button_color.md_bg_color = "black"
        button_color.color = "white"






test = quiz041()
test.run()

# quiz040.kv
Screen:
    size: 600,400

    MDBoxLayout:
        pos_hint : {"center_x":0.5, "center_y":0.5}
        size_hint : 1, 1 # width, height, h:relative

        MDLabel:
            id: text
            text: "Your Name"
            pos_hint: {"x_center":.5, "y_center":.5}
            font_size: "45pt"
            halign: "center"



        MDRaisedButton:
            id: button
            md_bg_color: "blue"
            size_hint: .1, .1
            font_size: "10pt"
            text: "Dark moad"
            on_press:
                app.pressed_button()


```

## evidence
<img width="811" alt="Screenshot 2024-01-26 at 17 55 28" src="https://github.com/ayyyane/unit3_g11/assets/142702159/b5760c56-6ff3-402d-b2b7-4b6397d082a3">
<img width="802" alt="Screenshot 2024-01-26 at 17 55 37" src="https://github.com/ayyyane/unit3_g11/assets/142702159/a3107eb2-b289-4f41-824e-bf741ff59717">

