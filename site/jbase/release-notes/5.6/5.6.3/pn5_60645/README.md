# PN5_60645

<PageHeader />

## Description

Util: New command **viewindex** to view a jBASE Secondary Index

### Previous Release Behavior

None

### Current Release Behavior

```
jsh home ~ -->viewindex -?

Description:  Views an ascending jBASE Secondary Index

Usage: viewindex filename {indexname {indexkey {id}}}

   If 'indexname' is not specified then view the first index found.
   If 'indexkey' is not specified then start at the beginning of 'indexname'.
   If 'id' is not specified then start at 'indexkey'.

Examples:

   viewindex CUSTOMERS
   [View the first index of the CUSTOMERS file starting at the beginning of the index]

   viewindex CUSTOMERS LASTNAME
   [View the LASTNAME index starting at the beginning]

   viewindex CUSTOMERS LASTNAME K
   [View the LASTNAME index starting at index keys beginning with 'K']

   viewindex CUSTOMERS LASTNAME K 123456
   [View the LASTNAME index starting at ID '123456' of index keys beginning with 'K']
```

Back to [5.6.3 Release Notes](./../README.md)

<PageFooter />
