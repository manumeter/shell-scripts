# Simple Useful Shell Scripts

## calc --help
    Usage: calc expression
    Use awk for arithemetic operations
    
    Operations: 
    
        x + y       Addition
        x - y       Subtraction
        - x         Negation
        x * y       Multiplication
        x / y       Division
        x % y       Modulo
        x ^ y       Exponentiation
        int(x)      Truncate integer toward zero
        sqrt(x)     Positive square root
        exp(x)      Exponentiation e ^ x
        log(x)      Natural logarithm
        sin(x)      Sine (in radians)
        cos(x)      Cosine (in radians)
        atan2(x, y) Arctangent of x / y (in radians)
        rand()      Random number between zero and one
        srand(x)    Random number starting at x

## create-deb-depends --help
    Usage: create-deb-depends name version depends [file.deb]

    Create a deb package for Debian / Ubuntu only containing dependency
    information. This helps recognizing relationship of packages and
    installed software. It also avoids accidental uninstalls.

    Examples: 

        create-deb-depends mutt-dependencies 1.3.17-1 "libc6 (>= 2.2.1), exim | mail-transport-agent" test.deb
        create-deb-depends config5-dependencies 0.1 "perl-modules, libtemplate-perl, lsb-release, curl, udev"

## create-repo
    Usage: ./repo.sh path

## de --help
    usage: de [-h] {ru,fr,en,pl,pt,ch,it,es} word
    
    Translate a word from or to german with dict.leo.org.
    
    positional arguments:
      {ru,fr,en,pl,pt,ch,it,es}
                            language to translate from or to german
      word                  word(s) to translate
    
    optional arguments:
      -h, --help            show this help message and exit

## deb-sign
    Usage: ./sign.sh package1.deb [package2.deb [...]]

## dict --help
    Usage: dict "word"
    Translate the given word(s) with dict.leo.org [English -- Deutsch]

## file-crypt --help
    Usage: file-crypt file
    Use tar and gpg to encrypt a file or directory
    See also: file-uncrypt

## file-uncrypt --help
    Usage: file-uncrypt file
    Use tar and gpg to uncrypt a file
    See also: file-crypt

## firefox-sleep --help
    Usage: firefox-sleep
    Suspend all Firefox (and plugin) processes
    See also: firefox-wake

## firefox-wake --help
    Usage: firefox-wake
    Wake up all Firefox (and plugin) processes
    See also: firefox-sleep

## host2ip --help
    Usage: host2ip dns-name
    Use host to convert dns-name to IP address

## ipcalc --help
    Usage: ipcalc [HHHHHHHH | HH.H.HH.H | DDDDDDDDDDDD | DDD.DD.D.DDD]
    Convert IPv4-Adresses HEX <--> DEC

## md2pdf --help
    Usage: ./md2pdf /path/to/file.md [/path/to/file.pdf]

## mp3-vbrfix --help
    Usage: mp3-vbrfix [file]
    Use vbrfix to fix wrong vbr header (e.g. song length) in all .mp3 files (recursively)

## mutex-lock --help
    Usage: mutex-lock [name]
    Use mkdir (atomicly) to realize mutex on file system level. If no
    name is specified, a default lock will be used.
    See also: mutex-unlock

## mutex-unlock --help
    Usage: mutex-unlock [name]
    Use mkdir (atomicly) to realize mutex on file system level. If no
    name is specified, a default lock will be used.
    See also: mutex-lock

## ssh-unlock-disk --help
    Usage: ssh-unlock-disk [ssh-options] hostname/ip
    
    Use this script to send a password through ssh to unlock luks encrypted disks
    (in initrds). It will use its own known_hosts file since the initrd's all have
    a different identity than the actual host (uses dropbear instead of openssh).

## ssh-keyup --help
    Usage: ssh-keyup hostname
	Update ssh-key of given hostname and ip address in ~/.ssh/known_hosts

## thunderbird-sleep --help
    Usage: thunderbird-sleep
    Suspend all thunderbird processes
    See also: thunderbird-wake

## thunderbird-wake --help
    Usage: thunderbird-wake
    Wake up all thunderbird processes
    See also: thunderbird-sleep
