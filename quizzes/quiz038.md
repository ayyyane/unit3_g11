# quiz038

## propmt
<img width="1276" alt="Screenshot 2024-01-26 at 16 45 38" src="https://github.com/ayyyane/unit3_g11/assets/142702159/0803810f-4792-41b0-8ddb-143034ec56e4">

![IMG_6AC62064957B-1](https://github.com/ayyyane/unit3_g11/assets/142702159/64ecf1af-a25b-43f1-a1ff-8484887ef045)


## solution

```.py
import matplotlib.pyplot as plt
import random

class SelemanMap:
    def __init__(self):
        self.x = []
        self.y = []
        self.names = []

    def set_names(self,ust_name:list):
        self.names = ust_name
        for i in range(len(ust_name)):
            x_value = random.randint(0,101)
            y_value = random.randint(0,101)
            self.x.append(x_value)
            self.y.append(y_value)
        return self.names, self.x, self.y

    def get_map(self):
        for item, x, y in zip(self.names, self.x, self.y):
            plt.text(x, y, item)
        plt.scatter(self.x, self.y)
        plt.xlabel("Distance (km)")
        plt.ylabel("Distance (km)")
        plt.show()

test = SelemanMap()
test.set_names(["Tokyo","Kyoto","Osaka","Karuizawa"])
test.get_map()


```

## evidence
<img width="615" alt="Screenshot 2024-01-26 at 17 27 38" src="https://github.com/ayyyane/unit3_g11/assets/142702159/0183d53c-a500-4167-b034-76afd9cc4bae">

