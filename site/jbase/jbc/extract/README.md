# EXTRACT

<PageHeader />

**Tags:**
<badge text='dynamic arrays manipultation' vertical='middle' />

## Description

The **EXTRACT** function is an alternative method of accessing values in a dynamic array other than using the &lt;n,n,n&gt; syntax. It takes the general form:

```
EXTRACT(expression1, expression2 {, expression3 {, expression4}})
```

Where:

- **expression1**┬áspecifies the dynamic array to work with and will normally be a previously assigned variable,
- **expression2**┬áspecifies the field to extract,
- **expression3** the value to extract and ,
- **expression4** the subvalue to extract.

## Note

> **expressions 2** through **4** should all return a numeric value or a runtime error will occur and the program will enter the debugger.

An example of use is as:

```
numArray = "0"; numArray<2> = "1"; numArray<3> = "2"
CRT EXTRACT(numArray, 2)
```

to display the value "1".

Go back to [jBASE BASIC](./../README.md)

Go back to [Programmers' Reference Guide](./../../reference-guides/jbc/README.md)

<PageFooter />
