## ip2location
A python script to lookup ip4 addresses and retrieve locational information about them. 

e.g : 

#### Default detail of an IP, read from a std_in here-string:
`$ip2location <<< echo 189.90.151.209`
`Brazil, Rio Grande do Sul, Sao Luiz Gonzaga`

#### Geo-coordinates of IPs string args:
`$ip2location -c 86.124.71.2`
`26.133329391479, 44.46667098999`

#### Piped verbose information:
`$echo "89.40.97.143\n62.76.8.138" | ip2location -v`
`89.40.97.143
Romania
RO
Bacau
Bacau
607075
26.89999961853
46.566669464111
SC Vesatel SRL
AS8708 RCS & RDS SA
62.76.8.138
Russian Federation
RU
Sverdlovskaya oblast'
Mikhaylovsk
450074
59.119998931885
56.435829162598
Bashkir State University
AS8475 State Educational Institute of Higher Professional Education Bashkirskiy State University
Romania, Bacau, Bacau
Russian Federation, Sverdlovskaya oblast', Mikhaylovsk`
