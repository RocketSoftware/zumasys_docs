# Creating Stub Files

<PageHeader />

## DescriptionÂ  

In order to access a remote file, a STUB file is required on the client side. This file is a plain text file with one line specifying basic information about the server host and the remote file:

```
JBC__SOB JediInitREMOTE
```
Special note.  That is two underlines after JBC!

Remote filename does not have to specify the remote path as the remote file will be located in the directory specified by the JEDIFILEPATH environment variable on the server.

If the remote file is again a STUB file, then the following entry has to be added to the jnet\_env file (on the server, where this stub file is located):

```
ENV: servername server_u_name client_u_name
```

e.g:

```
ENV:jRFS 10.44.5.70 jason jdean
```
When you are having issues turn on the logging features on both the client and server.  The log files are very detailed and will assist on what is misconfigured.

Back to [Remote Files](./../jbase-remote-file-service/README.md)

<PageFooter />
