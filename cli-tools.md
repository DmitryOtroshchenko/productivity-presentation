---
marp: true
---

# ripgrep

*Grep as it should have been built.*

https://github.com/BurntSushi/ripgrep

`brew install ripgrep`

- Fast
- Sane defaults: smartcase, colors, logical flag names
- Filter files by type, glob pattern, parent directory
- Multiline search
- Respects .gitignore
- Supports multiple encodings

---

# fd 1

*A simple, fast and user-friendly alternative to 'find'*

https://github.com/sharkdp/fd

`brew install fd`

- Convenient syntax: `fd PATTERN` instead of `find -iname '*PATTERN*'`
- Supports both regex and glob search
- Smart case
- Ignores hidden directories and files, by default
- Respects .gitignore
- Unicode-aware

---

# fd 2

![height:500px](./fd-github-screencast.svg)

---

# unp

*Unpack everything with one command*

`brew install unp`

- Full of perl and shit, but... does the job!
- **WARNING:** `man unp` is a lie, use `unp -h`
- Glorious glory: `unp -s`

---

# tldr 1

*Simplified, example based and community-driven man pages.*

https://github.com/dbrgn/tealdeer

`brew install tealdeer`

Output of `tldr fd`:

---

# tldr 2

![height:500px](tldr-output.png)

---

# coreutils 1

*Normal Linux ls, pwd, etc without OSX / BSD shit.*

`brew install coreutils`

See https://apple.stackexchange.com/questions/69223/how-to-replace-mac-os-x-utilities-with-gnu-core-utilities

People suggest `brew install coreutils findutils gnu-tar gnu-sed gawk gnutls gnu-indent gnu-getopt grep` for full Linux-like experience, but in my opinion `coreutils` are more than enough unless you write your own shell scripts and rely on Linux-like utils flavor.

---

# coreutil 2
**Coreutils bring a minor inconvenience:**

```
Commands also provided by macOS have been installed with the prefix "g".
If you need to use these commands with their normal names, you
can add a "gnubin" directory to your PATH from your bashrc like:
    PATH="$(brew --prefix)/opt/coreutils/libexec/gnubin:$PATH"
```

From my experience using coreutils without "g" prefix does not break anything.

---

# bat 1

*A (way) better cat.*

`brew install bat`

- Syntax highlighting
- Git integration
- Show non-printable characters
- Automatic paging

- **WARNING:** Integrations with ripgrep, man, watch look broken.

---

# bat 2

![height:500px](bat.png)
