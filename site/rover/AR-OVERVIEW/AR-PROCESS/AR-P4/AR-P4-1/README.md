##  A/R Service Charge Invoice Creation Procedure (AR.P4)

<PageHeader />

##

![](./AR-P4-1.jpg)

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
  
**Customer** Enter the customers you wish to run this report for. If left
blank all customers who meet the specified criteria will be selected.  
  
**Customer Name** The name of the associated customer.  
  
**Terms Code** If you wish to limit this report to customers with certain
terms codes, enter those terms codes here. Only customers with the referenced
code will be selected. Please note that this report looks at the terms code
posted to the CUST record and not the AR record. If this field is left blank,
the program will not use the terms code in determining which invoices to
include.  
  
**Last Status Message** Contains the last status message generated by the
program.  
  
**Last Status Date** The date on which the last status message was generated.  
  
**Last Status Time** The time at which the last status message was generated.  
  
**Percent** Enter the percentage that should be used when calculating the
service charge. If for example, the open or invoice amount on the invoice is
1000.00 and the percent is 10, the customer will be charged 10.00 as a service
charge. A new invoice or AR record will be created for the service charge.  
  
**Flat Amount** If you want to charge the customer a flat amount per invoice
instead of a percentage, enter that amount here.  
  
**Days Late** Enter the number of days late that an invoice must be for a
service charge to be applied to the customer's account. If, for example, you
enter 30 in this field, a service charge will be applied to all invoices that
are 30 days or older.  
  
**Grace Period** Enter the number of days which must pass before another
service charge can be applied to the customer's account for a given invoice.
If, for example, an invoice is 45 days past due and a service charge was
applied to the customer's account 15 days ago, how may days does this customer
have to remit payment before another service charge is posted to their
account.  
  
**G/L Account** Enter the g/l account number that the service charge should be
applied to.  
  
**Invoice Date** Enter the invoice date you wish applied to invoices that will
be created for the service charges.  
  
**Register Date** Enter the register date that should be applied to the
invoices that will be created in this procedure. This is the date you want the
charges applied to the general ledger. The invoice date will be loaded into
this field for you but can be changed as required.  
  
**Co Code** Enter the company code that should be referenced on the invoices
being created.  
  
**Use Invoice Amount** Check this box if you wish the service charge based on
the invoice amount and not the open balance. For example, if you have an
invoice for $1000.00 and a $500.00 payment has been applied to the invoice,
you have an open balance of $500.00. If this box is checked, the service
charge will be based on the $1000.00 and not $500.00. If this box is not
checked, the service charge will be based on $500.00. This box should only be
checked when using a percentage to calculate the service charge.  
  
**Include Service Invoices** Check this box if you wish to apply a service
charge (or late fee) to an invoice that was created via this procedure to bill
the customer for another service charge.  
  
  
<badge text= "Version 8.10.57" vertical="middle" />

<PageFooter />