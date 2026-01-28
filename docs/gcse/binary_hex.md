# Data Representation

## Denary system

Denary (Decimal) has 10 digits:

```
0   1   2   3   4   5   6   7   8   9
```

We can count from zero to nine in one "units" column, consider:

To represent `1`, there are no *hundreds*, no *tens*, just *one unit* represented but the character `1`:

```text
| Hundreds  | Tens  | Ones (Units) |
| 0         | 0     | 1            |
```

Same for, let's say seven:

```text
| Hundreds  | Tens  | Ones (Units) |
| 0         | 0     | 7            |
```

To represent **ten**, we have one "Ten" and no units:

```text
| Hundreds  | Tens  | Ones (Units) |
| 0         | 1     | 0            |
```

To represent "one hundred", we have one "Hundred", no tens, no units:

```text
| Hundreds  | Tens  | Ones (Units) |
| 1         | 0     | 0            |
```

You know how to count in **`Base10`**, what's important is remembering that there are columns, that go from right to left, each extra column appended to the right is 10 to the power of x:

| Column 2 - Hundreds 10^2^     | Column 1 - Tens 10^1^   | Columns 0 - Ones (Units) 10^0^  |
| ------------------------------|-------------------------|---------------------------------|
| 10^2^ = 10 * 10 = 100         | 10^1^ = 10              | N/A (We have 0-9)               |
| 4                             | 7                       | 6                               |

`476`

Work this the other way, taking 672 for example, we have 6 one hundreds, 7 tens, and 2.

## Binary System

With binary we don't have ten digits (units) 0-9, we only have **two** - "0" & "1", which represents "off" or "on", or "false" or "true".
This is called boolean, it can only have one of two states like a light switch "on" or "off".

So to represent numbers in binary, we need a different system, or columns which represent a number larger than "1".

```text
| Four  | Two  | One  |
| 0     | 0    | 1    |
```

To convert a decimal number into binary, take the decimal number 3 for example, starting from the left hand column:

* ask yourself how many fours are needed. In this case four is greater the three, so "0" fours are required.
* ask yourself how many 2 are needed. In this case 2 can be subtracted from out values "3", so "1" two IS required, leaving "1".
* ask yourself how many 1 are needed. In this case we have "1" remaining, therefore need a "1"

```text title="binary representing the decimal number 3"
| Four  | Two  | One  |
| 0     | 1    | 1    |
```

With these three columns we can only add up to "7":

```text title="binary representing the decimal number 3"
| Four  | Two  | One  |
| 1     | 1    | 1    |
```

**4 + 2 + 1 = 7**

| Column 2 - 4s 2^2^            | Column 1 - 2s 2^1^      | Columns 0 - 1s  2^0^            |
| ------------------------------|-------------------------|---------------------------------|
| 2^2^ = 2 * 2 = 4              | 2^1^ = 2                | 2^0^ = 1                        |
| 1                             | 1                       | 1                               |

With computers, we deal with bytes, which is 8 bits, each `0` & `1` represents a bit. 

So to convert the number 182 in to binary simply work left to right subtracting as you go, When you can do a subtraction in the column, it a "1", if you can't subtract without it going negative it's a "0":

| Hundred Twenty-Eight | Sixty-Four | Thirty-Two | Sixteen | Eight | Four  | Two   | One  |
|----------------------|------------|------------|---------|-------|-------|-------|------|
| 128                  | 64         | 32         | 16      | 8     | 4     | 2     | 1    |
| 182 - 128 = 54       | N/A        | 54-32=22   | 22-16=6 | N/A   | 6-4=2 | 2-2=0 | N/A  |
| 1                    | 0          | 1          | 1       | 0     | 1     | 1     | 0    |


So the binary number that represents the decimal `182` is `10110110`.

## Hexadecimal

Hexadecimal means **sixteen**. So, in decimal we have the ten digits `0-9`, in binary we have only two digits `0` and `1`.

In hexadecimal we have sixteen `0-F` 

```text
0   1   2   3   4   5   6   7   8   9   A   B   C   D   E   F
```

Or

```text
Hex       0,...9    A   B   C   D   E   F
Decimal   0,...9    10  11  12  13  14  15
```

So the columns look like this, say the decimal number `12` would simply be `C`:


| Two-hundred-fifty-sixes (256) 16^2^ | Sixteens (16) 16^1^  | Ones (Units) 16^0^ |
|-------------------------------------|----------------------|--------------------|
| 0                                   | 0                    | C                  |

Lets convert `182`, how many 16's go into 182? The answer is `11`, and the "hex" for `11` is? The answer is `B`, with a remainder of `6`. 

| Two-hundred-fifty-sixes (256) 16^2^ | Sixteens (16) 16^1^  | Ones (Units) 16^0^ |
|-------------------------------------|----------------------|--------------------|
| 0                                   | B                    | 6                  |

OK, the reason `hexadecimal` is used in computing is because it simplifies the binary representation of numbers for us mere humans. 

We can break a `byte` (8 bits) in half, leaving two **nibbles** (a nibble is 4 bits).

Using our example of the binary number for the decimal `182` being `10110110`.

We can split it into half, leaving two nibbles:

`10110110`

`1011`      `0110`

Any **nibble** can be represents by a single hexadecimal unit `0-F`. (`1111` in binary is 15, and we can goto `F` which is hex for `15`)

Therefore:

nibble `1011` = decimal `11` = hex `B`.
nibble `0110` = decimal `6` = hex `6`.

Sandwich this together we get `B6`.

| Base        | Conversions|          |
|-------------|------------|----------|
| Binary      | `10110110` |          |
| Nibbles     | `1011`     |   `0110` |
| Decimal     | `11`       |   `6`    |
| Hexadecimal | `B`        |   `6`    |
