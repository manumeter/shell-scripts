# Simple Useful Shell Scripts

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

## thunderbird-sleep --help
    Usage: thunderbird-sleep
    Suspend all thunderbird processes
    See also: thunderbird-wake

## thunderbird-wake --help
    Usage: thunderbird-wake
    Wake up all thunderbird processes
    See also: thunderbird-sleep
