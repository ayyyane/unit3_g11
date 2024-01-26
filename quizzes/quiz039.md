# quiz039

## prompt
<img width="1162" alt="Screenshot 2024-01-26 at 17 08 27" src="https://github.com/ayyyane/unit3_g11/assets/142702159/5b8601a9-236f-4719-9e74-878388b76e55">

## solution

```.py
from kivymd.app import MDApp

class quiz039(MDApp):
    def build(self):
        self.count = 0
        return

    def button_pressed(self):
        the_label = self.root.ids.label
        self.count += 1
        the_label.text = f"Count{self.count}"


test = quiz039()
test.run()

```

## evidence
<img width="624" alt="Screenshot 2024-01-26 at 17 30 39" src="https://github.com/ayyyane/unit3_g11/assets/142702159/a789d1bf-84ed-4381-be38-622ce9888271">
<img width="627" alt="Screenshot 2024-01-26 at 17 30 55" src="https://github.com/ayyyane/unit3_g11/assets/142702159/384e5977-59de-4a50-b077-4925ebed41b7">

