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