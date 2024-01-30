# quiz041

## prompt
<img width="734" alt="Screenshot 2024-01-26 at 17 58 03" src="https://github.com/ayyyane/unit3_g11/assets/142702159/2d4b018d-25d8-447d-9d88-9a6367e9a182">

![IMG_1326](https://github.com/ayyyane/unit3_g11/assets/142702159/142988bf-fd69-4b72-856f-42e897a62162)

## solution
```.py

# quiz041.py

from kivymd.app import MDApp

class quiz041(MDApp):
    def build(self):
        self.count = 0
        return

    def button_pressed(self, button):
        the_label = self.root.ids.text2
        if self.count%2 == 1:
            the_label.text = "It is O's turn"
            button.text = "o"
            button.md_bg_color = "yellow"
        else:
            the_label.text = "It is X's turn"
            button.text = "x"
            button.md_bg_color = "red"

        self.count += 1




test = quiz041()
test.run()

# quiz040.kv
Screen:
    size: 500,500

    MDLabel:
        id: text1
        pos_hint: {"center_x": .5, "center_y": .9}
        text: "Tic Tac Toe by student_name"
        halign: "center"
        font_size: "20pt"

    MDLabel:
        id: text2
        pos_hint: {"center_x": .5, "center_y": .8}
        text: "It is X's turn"
        halign: "center"
        font_size: "15pt"

    MDBoxLayout:
        orientation: "vertical"
        pos_hint:{"center_x": .5, "center_y": .4}
        size_hint: .6, .6




        MDBoxLayout:
            size_hint: 1, .2
            md_bg_color: "red"



            MDRaisedButton:
                id: button1
                size_hint: .2, 1
                md_bg_color: "green"
                on_press:
                    app.button_pressed(self)


            MDRaisedButton:
                id: button2
                size_hint: .2, 1
                md_bg_color: "green"
                on_press:
                    app.button_pressed(self)

            MDRaisedButton:
                id: button3
                size_hint: .2, 1
                md_bg_color: "green"
                on_press:
                    app.button_pressed(self)


        MDBoxLayout:
            size_hint: 1, .2
            md_bg_color: "green"

            MDRaisedButton:
                id: button4
                size_hint: .2, 1
                md_bg_color: "green"
                on_press:
                    app.button_pressed(self)

            MDRaisedButton:
                id: button5
                size_hint: .2, 1
                md_bg_color: "green"
                on_press:
                    app.button_pressed(self)

            MDRaisedButton:
                id: button6
                size_hint: .2, 1
                md_bg_color: "green"
                on_press:
                    app.button_pressed(self)

        MDBoxLayout:
            size_hint: 1, .2
            md_bg_color: "green"

            MDRaisedButton:
                id: button6
                size_hint: .2, 1
                md_bg_color: "green"

                on_press:
                    app.button_pressed(self)

            MDRaisedButton:
                id: button7
                size_hint: .2, 1
                md_bg_color: "green"
                on_press:
                    app.button_pressed(self)

            MDRaisedButton:
                id: button8
                size_hint: .2, 1
                md_bg_color: "green"
                on_press:
                    app.button_pressed(self)

```

## evidence


https://github.com/ayyyane/unit3_g11/assets/142702159/d312d09a-1237-4a59-a849-6d4de4acd75f





