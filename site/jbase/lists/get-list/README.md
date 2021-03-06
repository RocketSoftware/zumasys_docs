# GET-LIST

<PageHeader />

**Tags:**
<badge text='jql' vertical='middle' />
<badge text='lists' vertical='middle' />

## Description

Retrieves a previously stored list and makes it the current active (default) list. It takes the general form:

```
GET-LIST {list-name {account-name}}
```

where:

- **list-name** specifies the name of the list to be retrieved. If you do not specify a list name, the default list will be used.
- **account-name** is the name of the account from which the list was saved. If you do not specify account-name, the system will use the current account name.

## Note #1

> The GET-LIST command is used to retrieve a list previously stored using the [**SAVE-LIST**](./../save-list/README.md) command or the jBC [**WRITELIST**](./../../jbc/writelist/README.md) statement. If the list is retrieved successfully, it will become the current active (default) list and will be inherited by the next jBASE command or program.

### Example

```
:GET-LIST A.SALES
200 Records selected
>LIST SALES
```

Retrieves a list named A.SALES and generates an active list. You can then issue a subsequent command such as LIST SALES which will use the active list.

If **d3\_list\_processing = true** is set in the **$JBCRELEASEDIR/config/Config\_EMULATE** file then the command retrieves previously stored lists from a file or the POINTER-FILE, and it's use may be as:

```
GET-LIST {list1 list2 list3 ... listX} {(options}
```

or

```
GET-LIST {DICT} filename id1 {id2 id3 ...} {{options}
```

where options may be:

**A**- All Lists are in the POINTER-FILE, useful if the list name is the same as a file name.

## Note #2

> If multiple lists are specified then the resulting list is sorted and all entries in the resulting list are unique.

See also [List storage](./../list-storage).

Back to [List Processing](./../list-processing)

  
<PageFooter />
