# quiz036

## prompt

## solution 

```.py
class converter:
    def __init__(self):
        self.roman_digits = {100:"C" ,90:"XC" ,50:"L", 40:"XL", 10:"Xl", 9:"IX", 5:"V", 4:"IV", 3:"Ⅲ", 2:"Ⅱ", 1:"Ⅰ"}

    def convert2roman(self,decimal:int)->str:
        if 0<decimal and decimal<101:
            output = ""
            for k,v in self.roman_digits.items():
                q = decimal//k
                output += v*q
                decimal = decimal%k
        else:
            output = f"Error. Please put another number"
        return output

converter1 = converter()
print(converter1.convert2roman(95))



```

## evidence
<img width="1470" alt="Screenshot 2024-01-16 at 10 49 08" src="https://github.com/ayyyane/unit3_g11/assets/142702159/070e884f-e913-4137-9496-0ab932db2b20">
