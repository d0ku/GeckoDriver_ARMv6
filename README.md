# TL;DR

This repo contains geckodriver binaries compiled for ARMv6. These should work for example on Raspberry Pi Zero W and similar hardware. GeckoDriver version you are going to download has to match with your selenium version and Firefox version. You should find necessary information in Selenium documentation.

## How to download
Open [Releases tab](https://github.com/d0ku/GeckoDriver_ARMv6/releases), find version that suits you, click on Assets and download attached geckodriver binary.

## Disclaimer
Sad thing is, if you own RPi Zero or anything of similar computing capacities, it's probably too slow to run firefox anyway. First try to run firefox alone and check if it's performance is enough for you. If it is, have some fun with binaries in these repo.

I have not used binaries newer than v.0.18.0 so I am not sure whether they work or not. Download and try your luck with those.

### Issues
Please DO NOT open issues which are about Selenium or Firefox. If your program does not run and it outputs some error, first try to google for answer, take a quick look at documentation and if this does not help then consider adding issue to adequate repository ([Selenium](https://github.com/SeleniumHQ/selenium), [GeckoDriver](https://github.com/mozilla/geckodriver)). Remember that you should always try to find answer for your problems first, and only if you don't find anything open a new issue.

If output of your program clearly indicates that there was a problem with this particular compiled binary, you should:

1. Redownload binary and try again
2. Give binary permission to execute (chmod +x geckodriver) and run it. If it runs, it means that binary probably is not the problem. If you get some strange error trying just to run the binary, then open a new issue.

### Versions
Already compiled:

- Release v0.26.0

- Release v0.25.0

- Release v.0.24.0

- Release v.0.22.0

- Release v.0.21.0

- Release v.0.19.1

- Release v.0.19.0

- Release v.0.18.0

- Release v.0.17.0

- Release v.0.16.1

Error in compilation:

- Release v.0.20.0

- Release v.0.20.1

- Release v.0.23.0

### Inspiration:
I could not find any compiled geckodriver binaries for my RPi Zero W. That was quite frustrating so I googled a bit, found [Docker crosscompiler for Rust image by dlecan](https://github.com/dlecan/rust-crosscompiler-arm), and decided to gve it a try.
