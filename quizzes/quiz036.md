# quiz036

## prompt

## solution

```.py
class Account:
    def __init__(self):
        self.balance = 0
        self.holder_name = ""
        self.holder_email = ""
        self.number = ["000", "00000", "0"]

    def get_account_no(self)->str:
        output = f"{self.number[0]}-{self.number[1]}-{self.number[2]}"
        return output

    def set_holder_name(self, name:str)->str:
        self.holder_name = name
        return f"Holder's name set to {self.holder_name}"

    def set_holder_email(self, email:str)->str:
        self.holder_email = email
        return f"Holder's email set to {self.holder_email}"

    def get_balance(self)->int:
        return self.balance

    def deposit(self, amount:int)->str:
        output = ""
        if amount > self.balance:
            self.balance += amount
            output += f"New balance: {self.balance} USD"
        else:
            output += f"you don't have enough money"
        return output

#test quiz036

import pytest
from quiz036 import Account

def test_empty_account():
    bk = Account() # create object
    assert bk.balance == 0
    assert bk.holder_name == ""
    assert bk.holder_email == ""
    assert isinstance(bk.number, list) # checks datatype
    number = bk.get_account_no().split("-")
    assert len(number)==3 and len(number[0])==3 and len(number[1])==5 and len(number[2])==1

def test_create_accounty():
    bk = Account()
    assert bk.get_balance() == 0
    assert bk.set_holder_name(name="Ayane") == "Holder's name set to Ayane"
    assert bk.set_holder_email(email = "gmail") == "Holder's email set to gmail"
    assert bk.deposit(amount = 100) == "New balance: 100 USD"
```

## evidence
<img width="1460" alt="Screenshot 2024-01-16 at 10 55 27" src="https://github.com/ayyyane/unit3_g11/assets/142702159/d0555413-4413-408f-9225-1a2b0602ad6e">
