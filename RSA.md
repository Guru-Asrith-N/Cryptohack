# RSA 

## Starter

### RSA starter 1

```
a = pow(101,17,22663)
print (a)
```

`flag - 19906 ` 

### RSA starter 2

c = m^e mod N
```
a = pow(12,65537,17*23)
print (a)
```

`flag - 301`

### RSA starter 3

Eulers totient function gives the number of relative primes for the number from 1 to the number itself    
For any prime number p the number of relative primes are p-1   
phi(p*q) = phi(p)*phi(q)  if p and q are primes   

```
p = 857504083339712752489993810777
q = 1029224947942998075080348647219
a = (p-1)*(q-1)
print (a)
```

`flag - 882564595536224140639625987657529300394956519977044270821168 `

### RSA starter 4

d * e == 1 modulo (p-1)(q-1)
d = e ^-1 mod (p-1)*(q-1)
```
p = 857504083339712752489993810777
q = 1029224947942998075080348647219
e = 65537
a = (p-1)*(q-1)
d = pow(e,-1,a)
print (d)
```
`flag - 121832886702415731577073962957377780195510499965398469843281`

### RSA starter 5

d = e ^-1 mod (p-1)*(q-1)   
c = m ^d mod n

```
n = 882564595536224140639625987659416029426239230804614613279163
p = 857504083339712752489993810777
q = 1029224947942998075080348647219
e = 65537
c = 77578995801157823671636298847186723593814843845525223303932

phi = (p-1)*(q-1)
d = pow(e,-1,phi)
m = pow(c,d,n)

print (m)
```
`flag - 13371337`

### RSA starter 6

