Microsoft Outlook Plugin for Alfresco 5.2 from EisenVault. This allows one-way communication - i.e. saving of emails and attachments from Outlook to Alfresco. It has been tested with Outlook 2010, 2013 and 2016 on Windows 7, 8.1 and 10. 
It is compatible with Alfresco Community 5.2 as it uses the 5.2 REST APIs. It doesn't work with older versions of Alfresco.

You can either download installer binaries, or download the source code and compile with Microsoft Visual Studio 2015. Code is in C#.

Released under GNU LGPLv3. Please write to us at contact@eisenvault.com with any questions or comments.

Visit us at https://www.eisenvault.com

Note: This also works with self-signed certificates and trusted SSL Certificates (not self signed ones). This does not work with Alfresco Cloud (my.alfresco.com).

# Patching instructions

In order to allow self-signed certificates for HTTPs Alfresco servers, you can install the product as is. Once it's working, you can replace the patched DDL `EisenVaultOutlookPlugin.Data.dll` available in ZIP format at `Installer-Binaries` directory

Following instructions are only seudo-code, they do not work at all. Just only for further explanation on the patching process.

```
$ unzip ev-outlook-plugin-github/Installer-Binaries/EisenVaultOutlookPlugin.Data.dll-patched.zip
$ cp ev-outlook-plugin-github/Installer-Binaries/EisenVaultOutlookPlugin.Data.dll C:\Program Files\EisenVault Outlook Plugin
```