# fd

*A simple, fast and user-friendly alternative to 'find'*

https://github.com/sharkdp/fd

`brew install fd`

- Convenient syntax: `fd PATTERN` instead of `find -iname '*PATTERN*'`
- Supports both regex and glob search
- Smart case
- Ignores hidden directories and files, by default
- Ignores patterns from your .gitignore, by default
- Unicode-aware

![Screencast from fd github repo](./fd-github-screencast.svg)

---

# unp

*Unpack everything with one command*

`brew install unp`

- Full of perl and shit, but... does the job!
- **WARNING:** `man unp` is a lie, use `unp -h`
- Glorious glory: `unp -s`

---

# tldr / tealdeer

*Simplified, example based and community-driven man pages.*

https://github.com/dbrgn/tealdeer

`brew install tealdeer`

Output of `tldr fd`:

![tldr fd output](tldr-output.png)

---

# coreutils

*Normal Linux ls, pwd, etc without OSX / BSD shit.*

`brew install coreutils`

See https://apple.stackexchange.com/questions/69223/how-to-replace-mac-os-x-utilities-with-gnu-core-utilities

People suggest `brew install coreutils findutils gnu-tar gnu-sed gawk gnutls gnu-indent gnu-getopt grep` for full Linux-like experience, but in my opinion `coreutils` are more than enough unless you write your own shell scripts and rely on Linux-like utils flavor.

**Coreutils bring a minor inconvenience:**

```
Commands also provided by macOS have been installed with the prefix "g".
If you need to use these commands with their normal names, you
can add a "gnubin" directory to your PATH from your bashrc like:
    PATH="$(brew --prefix)/opt/coreutils/libexec/gnubin:$PATH"
```

From my experience using coreutils without "g" prefix does not break anything.

---

# bat

*A (way) better cat.*

`brew install bat`

- Syntax highlighting
- Git integration
- Show non-printable characters
- Automatic paging

- **WARNING:** Integrations with ripgrep, man, watch look broken.


![tldr fd output](bat.png)
