# Nostromo

This is a CLI application for [Nostromo] digital product management.

[Nostromo]: https://nostromo.io

## Usage

### Step 1 - Download CLI

The CLI binaries distributed do not require any external dependencies.
So, to get started, you need to download only the appropriate binary for you
operational system from the [releases page]. After extracting the file and
test with the following command.

```
./nostromo
```

You should see the list of available commands. In this first version, we provide
simple commands to manage cards and projects.

[releases page]: https://github.com/digitalnatives/nostromo-cli/releases

### Step 2 - Set up API token

The next step is fill in your personal API token. You can find this token in the
user settings page. After that, the `.env` file content should look like this

```
NOSTROMO_API_TOKEN=YOUR_PERSONAL_TOKEN
```

Having done that, test if everything is working fine by listing the projects.

```
./nostromo project list
```

### Step 3 - Path configuration and project settings [Optional]

Feel free to add the CLI to your shell's path. This configuration is specific to
your shell.  After you have it in your path, you can drop the `./`.

You can then set up project specific values.  These are the project name of a
specific directory and your default activity type.  For that, just create a file
named `.nostromo.yml` in the project's working directory.

```yml
project: nostromo
activity_type: Development
```

Then you can run commands like the following without specifying the project's name.

```
nostromo project work
```

## Troubleshooting and Feedback

If you run into troubles when configuring then CLI in your environment, please
open an issue in this repository. We will try to solve your issue as fast as we
can.
