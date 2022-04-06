The general syntax for the alias command varies somewhat according to the shell. In the case of the bash shell it is
alias [-p] [name="value"]

To set a variable in the shell, use

VARNAME="value"

A variable created like the ones in the example above is only available to the current shell. It is a local variable: child processes of the current shell will not be aware of this variable. In order to pass variables to a subshell, we need to export them using the export built-in command. Variables that are exported are referred to as environment variables. Setting and exporting is usually done in one step:

export VARNAME="value"


