# Web stack debugging #3

This was the fourth in a series of web stack debugging projects. In these
projects, I was given broken/bugged webstacks in isolated containers,
and tasked with fixing the web stack to a working state. For each
task, I wrote a script automating the commands necessary to fix the
web stack.

## Tasks

- **0. Strace is your friend**

  - [0-strace_is_your_friend.pp](./0-strace_is_your_friend.pp): Using `strace`, find out why Apache is returning a 500 error. Once you find the issue, fix it and then automate it using Puppet (instead of using Bash as you were previously doing).

- **Hint:**

  - `strace` can attach to a current running process
    You can use `tmux` to run `strace` in one window and `curl` in another one

- **Requirements:**
  - Your `0-strace_is_your_friend.pp` file must contain Puppet code
  - You can use whatever Puppet resource type you want for you fix
