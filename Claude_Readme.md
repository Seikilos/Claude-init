# What is it
This repo is designed to provide a starting point for claude agents.

# Purpose
I am using claude through WSL. So storing and accessing claude's user memory is somewhat not elegant because the files are not directly accessible and managable outside of the WSL distro.
To avoid storing claude instructions into `/home/<user>` which is only accessible via weird paths, this repo should provide a starting ground for claude.

# Why?
Giving claude clear actions usually results in good code. However, claude code seems always start as a junior developer on day 1, know how to code but explicitly requiring instructions to not repeat itself, use maging strings or numbers everywhere, and follow some good coding standards.
I lost count, in how many projects I had to copy my tailored "what-makes-a-good-software-engineer" Claude.md file. This repo, while not ideal, should provide a central location.