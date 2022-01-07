# shell-scripting

## List filtering and pipes
List 7 largest files in `/usr/bin` in descending order

```bash
ls -laSh /usr/bin | head -7
```

options `-`
- `l` long format
- `a` all (include hidden)
- `S` Sorted (descending default)
- `h` human readable
<br>
Next pass output of ls using a pipe, `|`, into head to get top 7.

## Command line args
`$1` default positional argument that can be passed in

```bash
argsExample.sh <something-to-pass-in>
```

The script would look like:

```bash
#!/bin/bash
echo $1
```
## Save web data
Script named `geturl` with two *args*: pass url and destination file

```bash
./geturl http://wttr.in/BEND bendWeather.html
```
where $1 = http://wttr.in/BEND
and `$2 = bendWeather.html`


Script details
```bash
#!/bin/bash
curl $1 >> $2
```
