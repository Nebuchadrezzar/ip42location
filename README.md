## ip2location
A python script to lookup ip4 addresses and retrieve locational information about them. 

e.g : 

### Standard use-cases: 
  `$ip2location 189.90.151.209`<br/>
  `Brazil, Rio Grande do Sul, Sao Luiz Gonzaga`
  
  `$sudo cat /var/log/nginx/access.log | ag -o "^[\d\.]+ " | uniq | ip2location`<br/>
  `Brazil, Rio Grande do Sul, Sao Luiz Gonzaga`
   `...`
  
#### Default detail of an IP, read from a std_in here-string:
`$ip2location <<< echo 189.90.151.209`<br/>
`Brazil, Rio Grande do Sul, Sao Luiz Gonzaga`

#### Geo-coordinates of IP4 string args:
  `$ip2location -c 86.124.71.2`<br/>
  `26.133329391479, 44.46667098999`

#### Piped verbose information:
`$echo "89.40.97.143\n62.76.8.138" | ip2location -v`<br/>
<...too long, but you get the idea...>

#### Read a file(s) of IP4 addresses, one per line:
  `$ip2location < ips.txt`<br/>
  <...too long, but you get the idea...><br/>
  Press `Ctrl-C` to gracefully quit.  
