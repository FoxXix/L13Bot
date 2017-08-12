<img align="right" src="https://github.com/FoxXix/L13Bot/blob/master/l131.png">

## Lucky 13 Gaming Bot

This bot takes all the fundamental commands from [Airhorn bot](https://airhorn.solutions)
and adds even more functionality through channel commands.

**Check out the [Lucky 13 Gaming](http://lucky-13gaming.com/) website or our
[Discord chat channel](https://discord.gg/DBXzhdv) for support.**

### Build

This assumes you already have a working Go environment setup and that
DiscordGo is correctly installed on your system.

From within the L13Bot folder, run the below command to compile the
project.

```sh
go build
```

### Usage

```
Usage of ./L13Bot:
  -t string
        Bot Token
```

The below example shows how to start the bot from the L13Bot folder.

```sh
./L13Bot -t YOUR_BOT_TOKEN
```

### Creating sounds

L13 Bot uses [DCA](https://github.com/bwmarrin/dca) files, which are 
pre-computed files that are easy to send to Discord.

If you would like to create your own DCA files, please use:
* [dca-rs](https://github.com/nstafie/dca-rs)

See the below example of creating a DCA file from a WAV file.  This also works 
with MP3, FLAC, and many other file formats. Of course, you will need to 
[install](https://github.com/nstafie/dca-rs#installation) dca-rs first :)

```sh
./dca-rs -i <input wav file> --raw > <output file>
```