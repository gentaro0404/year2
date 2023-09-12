# quiz072
## Prompt
Create the code for the MAC address machine

## Code Structure
### Python Flie
```.py
import random
class MacMaker():
    def __init__(self, n):
        self.number = n

    def generate_hex_pair(self):
        char = "0123456789ABCDEF"
        return f"{char[random.randint(0,15)]}{char[random.randint(0,15)]}"

    def generate_one(self):
        return ":".join(self.generate_hex_pair() for i in range(6))

    def final(self):
        out = set()
        while len(out) < self.number:
            out.add(self.generate_one())
        return out

boi = MacMaker(10)
print(boi.final())
```

## Paper Programming
## Evidence

