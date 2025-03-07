Identity by Kjallstrom (ultranurd@yahoo.com)
Guild: Mellonea
Server: Kirin Tor

---

This addon allows you to specify your main character's name, an identity format
string, and which channels will have your identity tag prepended. It
also allows you to specify a nickname for use in Raid and Party
channels.

All options are configured on a per-character basis.

Slash Commands:

/id <command> [<options>]
/identity <command> [<options>]

help
Displays this help text.

config
Prints the current Identity configuration. Default subcommand.

off
Turns Identity off, but all settings are preserved. No labels will be
sent. Identity is turned on by default.

on
Turns Identity on, using the currently stored settings. Configured
labels will be sent. Identity is turned on by default.

main [<name>]
Sets the main character's Identity. This is the name used for all
enabled channels except Raid and Party. If no main name is specified,
the name is cleared.

nick [<name>]
Sets the nickname Identity. This is the name used in Raid,
Battleground, and Party, if enabled. If no nickname is specified, the
name is cleared.

enable <channel> [...]
Enables Identity for the specified space-separated channels.
  Valid channel identifiers:
    guild, g
    officer, o
    raid, r
    party, p
    whisper, w, tell, t
    1-10

disable <channel> [...]
Disables Identity for the specified space-separated channels.

zone on|off
Sets whether zone information should be added to your Identity.

format [<format>]
Sets the string used to display your Identity. The default is [%s],
where %s is replaced by the current name information. The default can
be restored by specifying no format string. All format strings must
contain %s, which will be replaced by your Identity. Recommended for
advanced users only.

reset
Clears your character's Identity settings.

---

Known Bugs

2.0-20003

Trying to use more than one %s in the format string, or trying to use
% characters on their own, might cause problems, depending on how many
are in the format string.

---

Version History

2.0-20003

Near-complete rewrite of the original identity, with an emphasis on
greater configurability. My original motivations were:

1) My guild splits /g and /o into in-character and out-of-character
   channels, because we play on an RP server.
2) I wanted to use [Name] instead of (Name):.
3) I wanted to be able to change settings on individual numbered
   channels.

I believe all of that has been achieved. Comments welcome!

---

Original IDENTITY by Ferusnox
Guild: Heaven and Earth
Server: Cenarion Circle
"Just call me Nox"
