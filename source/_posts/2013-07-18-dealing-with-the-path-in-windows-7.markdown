---
layout: post
title: "Dealing with the Path in Windows 7. I"
date: 2013-07-18 09:57
comments: true
categories: 
- Windows 7
- Path
---

The `Path` environment variable in Windows is always a problem to deal with.

This seems to be the hard way to manage:

You get to open the `System Dialog` first, which is in the `Control Panel`.

### Control Panel:
{% img /images/control_panel.png "Control Panel" "Control Panel in Windows 7" %}

### Control Panel Search:
If you just type "path" in the search box at the upper right corner, `Control Panel` items will be filtered as:

{% img /images/control_panel_search_path.png "Control Panel Search Path" "Control Panel Search Path in Windows 7" %}

Now you have three options:

1. If you click on `System`, you get the `System` Dialog.

2. If you click on `Edit environment variables for your account`, you get the `Environment Variables` dialog but the `System Variables` option is disabled, and you can only change the `User variables`.  
{% img /images/environment_variables_user.png "Environment Variables User Dialog" "Environment Variables in Windows 7" %}

3. If you click on `Edit the system environment variables` option you get the `Environment Variables` dialog.

Or, if you prefer to right-click on `Computer` and select `Properties`, you get the `System` dialog as well, and now you can just click `Change Settings` here, then click `Environment Variables` at the `System Properties` dialog.

### System Dialog:
{% img /images/system.png "System Dialog" "System Dialog in Windows 7" %}

### System Properties:
{% img /images/system_properties.png "System Properties Dialog" "System Properties Dialog in Windows 7" %}

### Environment Variables:
{% img /images/environment_variables.png "Environment Variables Dialog" "Environment Variables in Windows 7" %}

You have to select the `Path` variable at the `System variables` and click the `Edit` button to finally get to `Edit System Variable` dialog.

### Edit System Variable:
{% img /images/edit_system_variable.png "Edit System Variable Dialog" "Edit System Variable Dialog in Windows 7" %}

Here you have to edit the `Path` variable value and click `OK`, which is terrifying if your `Path` looks like this:

    C:\Python27\;C:\Program Files (x86)\HP SimplePass\x64;C:\Program Files (x86)\HP SimplePass\;C:\Program Files (x86)\HP SimplePass\x64;C:\Program Files (x86)\HP SimplePass\;C:\Program Files (x86)\Intel\iCLS Client\;C:\Program Files\Intel\iCLS Client\;C:\Program Files\Common Files\Microsoft Shared\Windows Live;C:\Program Files (x86)\Common Files\Microsoft Shared\Windows Live;C:\Windows\system32;C:\Windows;C:\Windows\System32\Wbem;C:\Windows\System32\WindowsPowerShell\v1.0\;C:\Program Files (x86)\Windows Live\Shared;C:\Program Files (x86)\Common Files\Roxio Shared\DLLShared\;C:\Program Files (x86)\Common Files\Roxio Shared\DLLShared\;C:\Program Files (x86)\Common Files\Roxio Shared\12.0\DLLShared\;C:\Program Files (x86)\Intel\OpenCL SDK\2.0\bin\x86;C:\Program Files (x86)\Intel\OpenCL SDK\2.0\bin\x64;C:\texlive\2012\bin\win32;C:\Program Files (x86)\Inkscape;C:\Program Files (x86)\Pandoc\bin;C:\Program Files\7-Zip;C:\Program Files (x86)\Calibre2\;C:\Program Files (x86)\Intel\OpenCL SDK\2.0\bin\x86;C:\Program Files (x86)\Intel\OpenCL SDK\2.0\bin\x64;C:\Program Files\Intel\Intel(R) Management Engine Components\DAL;C:\Program Files\Intel\Intel(R) Management Engine Components\IPT;C:\Program Files (x86)\Intel\Intel(R) Management Engine Components\DAL;C:\Program Files (x86)\Intel\Intel(R) Management Engine Components\IPT;C:\Program Files (x86)\Lua\5.1;C:\Program Files (x86)\Lua\5.1\clibs;C:\Program Files\Calibre2\;C:\Program Files (x86)\infogridpacific\AZARDI\bin;C:\Program Files\Microsoft\Web Platform Installer\;C:\Program Files (x86)\Microsoft SDKs\TypeScript\;C:\Program Files\Microsoft SQL Server\110\Tools\Binn\;C:\Program Files (x86)\QuickTime\QTSystem\;C:\Program Files (x86)\infogridpacific\AZARDI\bin;C:\nodejs\;C:\Program Files (x86)\Git\cmd;C:\Program Files (x86)\Git\bin

It is probably better to `Copy` and `Paste` this value to a text editor, carefully edit and `Paste` back.
