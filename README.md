<img align="right" src="https://raw.githubusercontent.com/FoxXix/FoxXix.github.io/master/L13/img/l131.png">

## Lucky 13 Gaming Bot

This bot takes all the fundamental commands from [Airhorn bot](https://airhorn.solutions)
and adds even more functionality through channel commands.

**Check out the [Lucky 13 Gaming Discord chat channel](https://discord.gg/kCc4EWTn4D) for support.**

### Build

This assumes you already have a working Go environment setup and that
DiscordGo is correctly installed on your system. If not go [here to install GO](https://go.dev/doc/install)
and follow instructions [here](https://pkg.go.dev/github.com/bwmarrin/discordgo#section-readme) to setup DiscordGo.

From within the L13Bot folder, run the below command to compile the project.

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

See the below example of creating a DCA file from a MP3 file.  This also works 
with WAV, FLAC, and many other file formats. Of course, you will need to 
[install](https://github.com/bwmarrin/dca/tree/master/cmd/dca#Getting-Started) FFmpeg and the DCA CLI first. :)

```sh
ffmpeg -i test.mp3 -f s16le -ar 48000 -ac 2 pipe:1 | dca > test.dca
```
