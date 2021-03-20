
# Pride Prompt

Add a splash of color to your workspace by adding a pride flag to your terminal prompt!

Note: This requires a terminal emulator that supports ANSI true-color formatting codes.

## Installation and Usage

Download the `prideprompt` file from this repo and place it somewhere it can be easily accessed via the terminal, for example in `/usr/bin`. You may need to give it executable permissions, which can be done with the following command:

```sh
$ chmod +x path/to/prideprompt
```

Once you've installed it, you'll need to add it to your `~/.bashrc`. Add the following line, replacing `flag_name` with your desired flag: 

```sh
export PS1="$(prideprompt -f flag_name) \u@\h:\w\$"
```

This is the important part; you can customize the rest of your prompt around this as much as you want!

```sh
$(prideprompt -f flag_name)
```

You can see a list of all flags, or add your own, by opening the config file with this command:

```sh
$ prideprompt -c
```

Or you can reset your config file with this command (this is also the best way to update and include new defaults):

```sh
$ prideprompt -r
```
