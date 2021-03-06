# CHECKSUM

<PageHeader />

## Description

The **CHECKSUM** function returns a simple numeric checksum of a character string. It takes the general form:

```
CHECKSUM(expression)
```

Where:

**expression** may evaluate to any result but will usually be a string.

The function scans every character in **expression** and returns a numeric addition of the characters within **expression**. This is done by calculating the checksum by summing the product of the ASCII value of each character and its position within the string.

An example of use is as:

```
INPUT DataBlock,128:
IF CHECKSUM(DataBlock) = ExpectedChk THEN
    CRT AckChar:
END
ELSE
......

```

Go back to [jBASE BASIC](./../README.md)

Go back to [Programmers' Reference Guide](./../../reference-guides/jbc/README.md)

<PageFooter />
