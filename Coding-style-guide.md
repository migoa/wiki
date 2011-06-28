## Variables

Meaningful self documenting names should be used, if the variable name does not make it reasonably obvious as to the meaning, appropriate comments should be added.

Preferred naming convention is to use `snake_case` names, and not `CamelCase` or `somethingElse`.

`ALL_CAPS` is reserved for globals, any local variables should be in `snake_case`

Variables name should not clobber command names, such as `dir`, `pwd`


## Functions

Braces should be on the same line as the function name:

    function helpful() {
      ...
    }

Private or utility functions should be prefixed with an underscore:

    function _helper_util() {
      ...
    }


## General

Indenting should be done with 2 spaces.

When possible, use environment variables instead of forking a command.

    $(pwd) # don't use, forks a new process
    $PWD   # do use

`if-then` statements should be on one line:

    if [[ -f $1 ]]; then
      ...
    fi