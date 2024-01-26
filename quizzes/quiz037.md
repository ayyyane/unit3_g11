# quiz037

## prompt
![Screenshot 2024-01-26 at 16 43 35](https://github.com/ayyyane/unit3_g11/assets/142702159/21678413-bdac-402a-9692-63b4ac63f903)
![Class](https://github.com/ayyyane/unit3_g11/assets/142702159/a4590494-52b5-4b2b-b776-465c4a81be80)

## sulution

```.py
class CompoundInterest:
    def __init__(self):
        self.principal = None
        self.rate = None
        self.years = None

class AccountingProgram(CompoundInterest):
    def __init__(self,principal, rate, years):
        super().__init__()
        self.years=years

    def set_principal(self,principal):
        self.principal = principal
        print(principal)
        return self.principal


    def set_rate(self, rate):
        self.rate = rate
        return self.rate

    def set_years(self, years):
        self.principal = years
        return self.years

    def calculate_interest(self):
        return self.principal*(1+self.rate)**self.years


test = AccountingProgram(principal=100, rate=0.1, years=20)
print(test.calculate_interest())

```

## evidnece
<img width="1336" alt="Screenshot 2024-01-26 at 16 44 43" src="https://github.com/ayyyane/unit3_g11/assets/142702159/ed6cf464-b3a9-42bd-a7da-74c7c24a7911">
