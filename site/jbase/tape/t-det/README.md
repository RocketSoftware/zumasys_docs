# T-DET

<PageHeader />

**Tags:**
<badge text='spooler tape' vertical='middle' />

## DescriptionÂ  

The T-DET command detaches one or more previously attached tape devices. The command takes the general form:

```
T-DET {CHANNEL=channel} {(Uportno}
```

where:

- **channel** is the specific channel attachment (0-9) to be detached. If the channel is not specified then all tape device attachments for the port are detached.
- **U** this option used from another process will override the attachment and detach the device without regard for the process which performed the initial attach.. This option may fail if the executing user is a different user group than the attached jBASE process.
- **portno** is the port which has the tape attached. This can be obtained from the [T-STATUS](./../t-status) command.

An example of use would be:

```
T-DET
```

to detach all tape devices attached to this port.

Back to [Tape Commands](./../tape-commands/README.md)

<PageFooter />
