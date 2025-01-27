# kek - the deno module
<!-- aka. Kommandoexekutionskonsole / Krampfhafte Entwicklungs-Kooperation / Knowledge Extending Karate -->

[![nest badge](https://nest.land/badge-large.svg)](https://nest.land/package/kek)

## Usage

This module is a collection of simple scripts that a developer might find handy.
To use it, simply type `deno run https://deno.land/x/kek/mod.ts --help` in your console and you will get an output like this:

```console
$ deno run https://deno.land/x/kek/mod.ts --help
List of commands and their description:

  test:         This command is for testing this deno module.
  hex2string:   Converts a hex value to a string.
  string2hex:   Converts a string to a hex value.
  hex2int:      Converts hex to integer.
  int2hex:      Converts integer to hex.
  base64:       Converts the provided string to base64.
  base64decode: Decodes a base64 encoded string.
  md5:          Computes the MD5 checksum of a given string.
  sha1:         Computes the SHA1 checksum of a given string.
  hash:         Computes the hash of a given string.
  cm2inch:      Converts cm to inch.
  inch2cm:      Converts inch to cm.

Syntax:
  deno run https://deno.land/x/kek/mod.ts <command>
```

If you want to know what a specific command can do and how to use it, simply type `deno run https://deno.land/x/kek/mod.ts COMMAND --help`.

For the command `test` this would result in the following:

```console
$ deno run https://deno.land/x/kek/mod.ts test --help
This command is for testing this deno module.

    test simply responds with the given command line arguments.
    This way you can check if the alias settings are correct and how we implemented them.
```

## Setting up an alias

### Windows (PowerShell)

If you want to use _kek_ as a command in your PowerShell, simply do the following steps:

1. Create a profile.ps1 file with the following input (you can change the version number of kek for your liking):

```ps1
function kekCommand {
    deno run https://deno.land/x/kek/mod.ts $args
}

Set-Alias kek kekCommand
```

2. Save this file to either `$Home\Documents` (C:\Users\yourname\Documents) -- only your user will be able to use `kek` **OR** to `$PsHome` (C:\Windows\System32\WindowsPowerShell\v1.0) -- every PowerShell user will be able to use `kek`.
3. Restart your PowerShell
4. Profit

### Linux (Bash)

If you want to use _kek_ as a command in your linux bash, simply do the following steps:

1. Edit either the `~/.bash_aliases` or the `~/.bashrc` file
2. Append the new alias as `alias kek='deno run https://deno.land/x/kek/mod.ts'` and save the file
3. Profit

### MacOS (zsh)

<!-- It doesn't have to be this way - use https://distrochooser.de/ to fix your problem -->

coming soon...
