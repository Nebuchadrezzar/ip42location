## ip2location
A python script to lookup ip4 addresses and retrieve locational information about them. 

e.g : 

#### Default detail of an IP, read from a std_in here-string:
`$ip2location <<< echo 189.90.151.209`

Brazil, Rio Grande do Sul, Sao Luiz Gonzaga

#### Geo-coordinates of IPs string args:
`$ip2location -c 86.124.71.2`

26.133329391479, 44.46667098999

#### Piped verbose information:
`$echo "89.40.97.143\n62.76.8.138" | ip2location -v`

<...too long, but you get the idea...>
