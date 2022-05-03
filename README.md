# sh-radio
Listen to internet radio stations from the command line with mpv.

## Usage
This script reads from `~/.local/share/radio-stations.tsv` to get both names and urls for your internet radio stations.
This script should have one stations on each line with the name and url being separated by a tab.
```
Name 1  https://example.com
Longer name two ftp://example.com
n3  ytdl://example.com
```
You can use various protocols thanks to `mpv`.
To see what protocols your version of `mpv` has run `mpv --list-protocols`

## Dependencies
- A posix shell
  + read
  + printf
  + trap
- mpv
- sed
- A terminal to run the program in (tested with urxvt)
