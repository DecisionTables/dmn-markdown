# DMN compliant decision tables in Markdown

## Overview

```shell
$ dsntk --version
```

Output:

```text
0.2.0-dev
```

## Examples

### Rules as rows (horizontal)

#### No inputs

> [H_000010.md](./H_000010.md)

| C |             |
|:-:|:-----------:|
|   |    `Out`    |
| 1 |  "Monday"   |
| 2 |  "Tuesday"  |
| 3 | "Wednesday" |
| 4 | "Thursday"  |
| 5 |  "Friday"   |
| 6 | "Saturday"  |
| 7 |  "Sunday"   |

```shell
$ dsntk edt --markdown I_000010.ctx H_000010.md
```

Output:

```text
["Monday", "Tuesday", "Wednesday", "Thursday", "Friday", "Saturday", "Sunday"]
```

### Rules as columns (vertical)
