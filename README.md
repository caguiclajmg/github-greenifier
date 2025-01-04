# github-greenifier

A Bash script that makes your contribution graph green.

Want to greenify your contribution graph?

![Contribution Graph 1](docs/snapshot1.png "Contribution Graph 1")

or write anything you want?

![Contribution Graph 2](docs/snapshot2.png "Contribution Graph 2")

## Requirements

+ Bash (>= 3.2.57)
+ GNU Coreutils

## Usage

Create commits such that it spells out certain text:

```shell
$ ./greenify.sh -m 'DEEZ NUTS' /home/user/my-repository
```

Generate random number of commits each day throughout the specified dates on a specified repository:

```shell
$ ./greenify.sh -df 2024-01-07 -dt 2025-01-05 /home/user/my-repository
```

### Options

`-df|--date-from` - Date to start generating commits

`-dt|--date-to` - Date to end generating commits

`-f|--target-file` - File used to generate commits

`-m|--draw-message` - Make commits on certain days as to make the specified message appear on the contribution graph

`--commit-count` - Amount of commits to make each day. If this is specified, `--commit-min` and `--commit-max` are ignored.

`--commit-min` - Minimum amount of commits each day

`--commit-max` - Maximum amount of commits each day

<sup>Note: No remotes are added so the user will have to manually add a remote and push the changes.</sup>

`-h|--help` - Show help options
