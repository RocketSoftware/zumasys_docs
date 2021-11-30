##  A/R Invoice Printing (AR.F1)

<PageHeader />

##

![](./AR-F1-1.jpg)

**Job ID** Enter a unique ID if you wish to enter and save the parameters to
this procedure for future use. If you only need to run the procedure and do
not want to save your entry then you may leave this field empty.  
  
**Destination** Select the destination for the output from this procedure.  
  
**Process** Select the method to be used for processing the report. Foreground
is always available and must be used when output is directed to anything other
than a system printer (i.e. printers spooled through the database on the host
computer.) Depending on your setup there may be various batch process queues
available in the list that allow you to submit the job for processing in the
background or at a predefined time such as overnight. A system printer must be
specified when using these queues.  
  
**Format** Select the format for the output. The availability of other formats
depends on what is allowed by each procedure. Possible formats include Text,
Excel, Word, PDF, HTML, Comma delimited and Tab delimited.  
  
**Layout** You may indicate the layout of the printed page by specifying the
appropriate setting in this field. Set the value to Portrait if the page is to
be oriented with the shorter dimension (usually 8.5 inches) at the top or
Landscape if the longer dimension (usually 11 inches) is to be at the top.
Portrait will always be available but Landscape is dependent on the output
destination and may not be available in all cases.  
  
**Copies** Enter the number of copies to be printed.  
  
**Run Process** Click on the button to run the process. This performs the save
function which may also be activated by clicking the save button in the tool
bar or pressing the F9 key or Ctrl+S.  
  
**AR Item** Enter the numbers of all the invoices you would like printed. If
you want to print all of the invoices that have not been printed previously,
then leave this and all of the other prompts blank. If you want to print a
range of invoices, or invoices printed before in a date range, leave this
field blank.  
  
**Co Code** This option is used in connection with the date/ invoice range
fields. If left blank all companies will be selected else only those specified
will be selected.  
  
**Start Date** If you want to re-print the invoices for a period of time,
enter the start date of the period in this field.  
  
**End Date** If you want to re-print invoices that were printed within a date
range, enter the end date of that range.  
  
**Starting Invoice** To print invoices within a range of numbers, enter the
starting invoice number in this field.  
  
**Ending Invoice** To print a range of invoice numbers, enter the ending
number of the range in this field.  
  
**Last Status Message** Contains the last status message generated by the
program.  
  
**Last Status Date** The date on which the last status message was generated.  
  
**Last Status Time** The time at which the last status message was generated.  
  
  
<badge text= "Version 8.10.57" vertical="middle" />

<PageFooter />