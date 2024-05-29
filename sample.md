
**Name:** list
```
list [<options>]
```
**Description**
Lists all issues if no options passed, otherwise filters issues based on the specified arguments. See below for details.

**Options**

  `--status`, `-s <status>`
    &nbsp;&nbsp;&nbsp;&nbsp; Returns only the issues with the same status as `<status>`


`--release`, `-r <release-version>`
   &nbsp;&nbsp;&nbsp;&nbsp;Returns only the issues with the same release version as `<release-version>`

`--product`, `-p <product>`
&nbsp;&nbsp;&nbsp;&nbsp; Returns the issues related to `<product>`


**Examples**

`list -s {completed or in-progress}`
&nbsp;&nbsp;&nbsp;&nbsp; Returns all the issues which are completed or are in progress

`list -r 4.9.1`
&nbsp;&nbsp;&nbsp;&nbsp; Returns all the issues which are associated with release 4.9.1

`list -p toaster`
&nbsp;&nbsp;&nbsp;&nbsp; Returns all the issues associated with toasters
