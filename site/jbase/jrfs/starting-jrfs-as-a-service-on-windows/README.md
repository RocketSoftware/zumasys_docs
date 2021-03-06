# Starting jRFS as a Service on Windows

<PageHeader />

## DescriptionÂ  

On Windows, you can setup jRFS so that it runs as a Windows service. There needs to be a few environment variable changes done to windows first to allow this to happen. As a service, the jRFS does not use the local user settings (It uses the local SYSTEM user on the Windows machine), so the environment needs to be set up in the Global Environment variable area.  

The following are the main variables required.

- JBCRELEASEDIR={Where jBASE is installed}
- JBCGLOBALDIR={Where jBASE is installed}
- JEDIFILEPATH={Path to your files}
- PATH={Where the jBASE bin files are installed};%PATH%

Other environment variables if needed, for example, JEDI\_FILENAME\_MD and JEDIFILENAME\_SYSTEM, will also need to be set globally. An example setup would be:

- JBCRELEASEDIR=C:\jBASE\5.7.0
- JBCGLOBALDIR=C:\jBASE\5.7.0
- JEDIFILEPATH=c:\jbase\home\data
- PATH=C:\jBASE\5.7.0\bin;{Remainder of path that already exists}

Remember to make sure that the local SYSTEM user has permissions to access the directories you set up. Once you have made these global environment variable changes, re-boot the machine so that they are available to all users on the machine.  

Next from a command prompt or jshell type:

```
jservcontrol jRFS install
jservcontrol jRFS start
```

Now have a look at the task manager and make sure the jRFS is running and you can check via the Administrative Tools menu to see that the jBASE Remote File Service is showing.

Back to [Remote Files](./../jbase-remote-file-service/README.md)
  
<PageFooter />
