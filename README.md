# epsonsimplecups

Suitable for *Raspbian GNU/Linux 10 (buster)*

1) `sudo -i`
2) `apt-get install libcups2-dev`
3) `apt-get install libcupsimage2-dev`
4) `usermod -a -G lpadmin pi`
5) Complete the following steps to acces the CUPS management inside the browser [https://raspberrytips.com/install-printer-raspberry-pi/](https://raspberrytips.com/install-printer-raspberry-pi/)
5) `git clone` this repo.
6) `cd` into the cloned folder.
7) Run `make` to build this package.
8) When finished run `make install`

Go to the CUPS Management URL [https://{yourIP}:631](https://{yourIP}:631) to install the Epson TM-T20 POS printer.


A simple CUPS driver for the Epson TM-T20 POS printer.
Epson provides a driver for this printer, but they only provide x86 and x64 linux binary builds instead of source. As a result, the driver can't be used on ARM systems, such as the Raspberry PI.
