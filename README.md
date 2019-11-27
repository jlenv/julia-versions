# julia-versions

A repository of metadata for [Julia](https://julialang.org) versions.

## Directory Structure

* `[julia]/`
  * [`versions.txt`](julia/versions.txt) - an exhaustive list of every released
    version. Versions must be listed in natural order.
  * [`stable.txt`](julia/stable.txt) - a list of current stable versions.
    Versions must be listed in natural order.
  * [`signatures.gpg`](julia/signatures.gpg) - a list of filenames of every
    released archive.
  * [`signatures/`](julia/signatures/) - a folder of GPG signature files of
    every released archive.

## Contributing

Use `update.sh`, or manually do the following:

1. Add the new version to `versions.txt`.
   * Versions should be listed incrementally.
2. Add new _stable_ versions to `stable.txt`, replacing any previous stable
   version for that version family.
   * Should only contain the latest stable version for each version family.
3. Append the filename for _all_ released files to `signatures.gpg`.
4. Save the GPG signature file for _all_ released files to `julia/signatures/`.

* Never remove a version from `versions.txt`.
* Never remove checksums from a `signatures.*` file, unless the file is
  literally no longer available on the Internet.
