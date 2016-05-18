Enterprise Patterns
==================
Stellt sicher, dass das richtige passiert, egal was gemacht wird

Enterprise Loop
---------------

Enterprise Exception Handling
-----------------------------
ggf ersetzbar durch enterprise loop.


Enterprise Installation
-----------------------

Rebooting
----------

Enterprise Einschalter (eon)
----------------------------
Device that turns something on as soon as possible.

Supernintendo Pattern
---------------------

Enterprise Root
---------------
scripts which need root access but are called with lower privileges. The Enterprise Root Pattern provides a Solution for this issue by calling the script itself as sudo.
```
<code>
if test "${nosudo-false}" != true -a `id -u` != 0; then
  echo "we're going sudo..." >&2
  exec sudo "$0" "$@"
  exit 23 # go to hell
fi
</script> // enterprise ist, wenn <code> ... </script> trotzdem matcht
```

Enterprise Shutdown
------------------
Mittel der Wahl um einen Shutdown zu erzwingen

Bsp: das Not-Aus in der Maschinensicherheit

Enterprise Deep Copy
--------------------
Bsp: var copy = JSON.parse(JSON.stringify(source))

Enterprise Thinking
-------------------
Prozess um auf Enterprise Patterns zu kommen

Bug-Driven Development
---------------------

Source-based Documentation / Help
---------------------------------
<code>
  #! /bin/sh
  if echo "$*" | grep -q '\(^\| \)-h\( \|$\)'; then
    cat "$0"
  fi
  # [more code]
</code>

Literate Programming
--------------------
Omit all the comments.

Litterate Programming
---------------------
Write throw-away code and it will become production code

Enterprise Expect
-----------------
Because you always know what you want, `expect(3)` script code can be replaced
by a `subshell and pipe` pattern :

<code>
    ( echo "$username"; sleep 1; echo "$password"; sleep 1; echo "cp old new" ) | telnet 
</code>

painload example: `//retiolum/bin/announce_pubkey`

Enterprise Waiting
------------------
Quietly wait until someone else solves the problem.
Passive variant of Complainterprise Waiting.

Complainterprise Waiting
------------------------
Submit a bug report and do Enterprise Waiting.
Active variant of Enterprise Waiting.
