# Cheats

## Installation

``` shell
$ brew install navi
```

## Usage

``` shell
user="vurihuang"
repo="cheats"
$ git clone https://github.com/${user}/${repo}.git "$(navi info cheats-path)/${user}__${repo}"
$ navi
```

## Auto updating

``` shell
user="vurihuang"
repo="cheats"

$ crontab -e
# Add these cron job.
*/0 0 * * * bash -c 'cd "$(/usr/local/bin/navi info cheats-path)/${user}__${repo}" && /usr/local/bin/git pull -q origin master'
```
