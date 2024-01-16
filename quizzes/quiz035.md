## quiz035

## prompt

## solution
```.py
def iterate(list1:list, list2:list)->list:
    output = []
    for item in list1:
        for x in list2:
            if x == item:
                output.append(item)
    return output

print(iterate([2,5,7,8,9],[2,4,6,7,8]))

```

## evidence
<img width="1468" alt="Screenshot 2024-01-16 at 10 48 46" src="https://github.com/ayyyane/unit3_g11/assets/142702159/5564ba63-76e0-47d7-a264-c9cf82040570">
