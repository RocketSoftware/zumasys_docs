##  AR Invoice Distribution Listing (AR.R8)

<PageHeader />

##

![](./AR-R8-1.jpg)

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
  
**Start Date** Enter the start date range within which the date must fall to
be selected for this report. Leaving this field null will assume you wish to
select all invoices dated prior to the end date entered.  
  
**End Date** Enter the end date range within which the invoice date must fall
to be selected for this report. Leaving this field null assumes you wish to
select all invoices since the start date entered.  
  
**Sort By** If you wish to sort this report by AR Id (invoice number), enter
'I'. To sort by date, enter 'D'.  
  
**Co Code** Enter the company codes you wish to appear on this report. If left
blank all company codes will be included.  
  
**Last Status Message** Contains the last status message generated by the
program.  
  
**Last Status Date** The date on which the last status message was generated.  
  
**Last Status Time** The time at which the last status message was generated.  
  
**Credit Memos Only** Check this box, if you only wish to include credit memos
on the report. An invoice is classified as a credit memo if the invoice amount
is less than zero.  
  
**Invoices Only** Check this box, if you only wish to include invoices on the
report. If this box is checked and the invoice has an amount greater than
zero, it will be included in this report.  
  
  
<badge text= "Version 8.10.57" vertical="middle" />

<PageFooter />