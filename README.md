#### Description:

This repository is forked from https://github.com/mit-pdos/xv6-public
As part of an assignment to add a trace syscall to xv6.


#### How to execute / test:

This adds a trace system call to xv6, which enables/disables verbose output of every system call made and its return value.

`int trace(int)`

The argument can be T_UNTRACE, which unsets tracing, or T_TRACE which sets tracing, or T_TRACE | T_ONFORK which sets tracing for current process and also any child created using fork.

we have a test program trd which just runs some syscalls to confirm.

We can also enable or disable tracing from shell itself. `trace` command enables syscall printing for any command invoked from shell. `untrace` disables it.

