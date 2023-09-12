# quiz 070

## Prompt
create the code for IPv4 machine

## Code Structure
```.py
def ipv4machine_gentaro():
    for a in range(0, 256):
        for b in range(0, 256):
            for c in range(0, 256):
                for d in range(0, 256):
                    yield f"{a}.{b}.{c}.{d}"

# 例として、最初の10個のIPアドレスを取得するには:
generator = ipv4machine_bernard()
for _ in range(10):
    print(next(generator))

```

## Paper Programming

## Evidence
