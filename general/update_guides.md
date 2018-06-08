
# Creating "Update" guides

Each major release of MyTardis needs a corresponding [update guide](https://github.com/mytardis/mytardis/tree/develop/docs/updates)
with instructions on how to manually upgrade from the previous major release.

1. Copy the previous update guide to use as a template:

    ```sh
    # NOTE: This command is an example! Update it to reflect new version numbers.
    cp docs/update/3.8-to-3.9.md doc/update/3.9-to-3.10.md
    ```

1. Update the versions in the top-level header.
1. Update the name of the latest `series-X.Y` branch **Get latest code**.
   There are two occurrences.
1. Update the names of the `series-X.Y` branches in **Update configuration
   files**.
1. Update references to the "previous version" in **Things went south?** and the
   link to the previous guide.
1. Add any special instructions specific to this version. For example, maybe
   this version adds a new external dependency not in the previous version.
1. Read through the entire guide to make sure it makes sense. For example, maybe
   the previous version required special steps that no longer apply this
   version.