### Renamed the `init` method in `BitArray` to `initialize`

`ocean.core.BitArray`

The `BitArray` struct had an `init` method which was used for initializing
with a set of parameters. However, this would make `BitArray.init` unusable,
and would emit a compiler error. This is problematic for generic code which
expects T.init to always work.

The method has been renamed to `initialize`.
