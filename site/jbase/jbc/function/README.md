# FUNCTION

<PageHeader />

## Description

Identifies a user-defined function, which can be invoked by other jBASE BASIC programs. Arguments to the function can optionally be declared. It takes the general form:

```
FUNCTION name {({MAT} variable, {MAT} variable...) }
```

## Syntax

**Name** is the name by which the function is invoked.

**Variable** is an expression used to pass values between the calling program and the function.

## Notes

The **FUNCTION** statement is used to identify user-written source code functions. Each function must be coded in a separate record and the record Id must match that of the Function Name, which in turn should match the reference in the calling program.

The optional comma separated variable list can be a number of expressions that pass values between the calling programs and the function. To pass an array the variable name must be preceded by the MAT keyword. When a user-written function is called, the calling program must specify the same number of variables that are specified in the **FUNCTION** statement.

An extra 'hidden' variable is used to return a value from the user-written function. The value to be returned can be specified within the Function by the [RETURN(value)](./../return/README.md) statement. If using the [RETURN](./../return/README.md) statement without a value then by default it returns an empty string.

The calling program must specify a [DEFFUN](./../deffun/README.md) or DEFB statement to describe the function to be called and the function source must be cataloged and locatable similar to subroutines.

## Example

An example of use would be:

```
FUNCTION MyFunction(A, B)
Result = A * B
RETURN (Result)
```

Go back to [jBASE BASIC](./../README.md)

Go back to [Programmers' Reference Guide](./../../reference-guides/jbc/README.md)

<PageFooter />
