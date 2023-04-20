# com.adobe.Reader

Now available on Flathub! https://github.com/flathub/com.adobe.Reader

This is a work-in-progress Flatpak of Acrobat Reader 9.5.5 for Linux

I really which this would just work, but it's broken and produces a `Bad system call` error. If you can help me figure it out, I would be immensely grateful. 

```bash
flatpak run --command=bash --devel com.adobe.Reader
```

```
[📦 com.adobe.Reader com.adobe.Reader]$ gdb /app/Adobe/Reader9/Reader/intellinux/bin/acroread
GNU gdb (GDB) 11.2
Copyright (C) 2022 Free Software Foundation, Inc.
License GPLv3+: GNU GPL version 3 or later <http://gnu.org/licenses/gpl.html>
This is free software: you are free to change and redistribute it.
There is NO WARRANTY, to the extent permitted by law.
Type "show copying" and "show warranty" for details.
This GDB was configured as "x86_64-unknown-linux-gnu".
Type "show configuration" for configuration details.
For bug reporting instructions, please see:
<https://www.gnu.org/software/gdb/bugs/>.
Find the GDB manual and other documentation resources online at:
    <http://www.gnu.org/software/gdb/documentation/>.

For help, type "help".
Type "apropos word" to search for commands related to "word"...
Reading symbols from /app/Adobe/Reader9/Reader/intellinux/bin/acroread...
(No debugging symbols found in /app/Adobe/Reader9/Reader/intellinux/bin/acroread)
(gdb) run
Starting program: /app/Adobe/Reader9/Reader/intellinux/bin/acroread 

Program terminated with signal SIGSYS, Bad system call.
The program no longer exists.
```
