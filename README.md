# subnet
[Subnet Calculator](https://www.calculator.net/ip-subnet-calculator.html)

[Sunet Mask: Hexidecimal to decimal](https://www.pawprint.net/designresources/netmask-converter.php)

```
echo "ffffff00" | perl -pe '$_ = join(".", map(hex, /.{2}/g))'
=> 255.255.255.0

echo "ffffff00" | perl -pe '$_ = unpack("B32", pack("H*", $_)); s/0+$//g; $_ = length'
=> 24
```
