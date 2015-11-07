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

## dict --help
    Usage: dict [word]
    Translate the given word(s) with dict.leo.org [English -- Deutsch]

## firefox-sleep --help
    Usage: firefox-sleep
    Suspend all Firefox (and plugin) processes
    See also: firefox-wake

## firefox-wake --help
    Usage: firefox-wake
    Wake up all Firefox (and plugin) processes
    See also: firefox-sleep

## mkdeb-depends --help
    Usage: mkdeb-depends name version depends [file.deb]

    Create a deb package for Debian / Ubuntu only containing dependency
    information. This helps recognizing relationship of packages and
    installed software. It also avoids accidental uninstalls.

    Examples: 

        mkdeb-depends mutt-dependencies 1.3.17-1 "libc6 (>= 2.2.1), exim | mail-transport-agent" test.deb
        mkdeb-depends config5-dependencies 0.1 "perl-modules, libtemplate-perl, lsb-release, curl, udev"

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

## thunderbird-sleep --help
    Usage: thunderbird-sleep
    Suspend all thunderbird processes
    See also: thunderbird-wake

## thunderbird-wake --help
    Usage: thunderbird-wake
    Wake up all thunderbird processes
    See also: thunderbird-sleep
