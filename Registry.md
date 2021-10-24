# Windows Registry 

The Windows Registry is a hierarchical database that stores low-level settings for the Microsoft Windows operating system and for applications that opt to use the registry. The kernel, device drivers, services, Security Accounts Manager, and user interfaces can all use the registry. The registry also allows access to counters for profiling system performance.

## Registry Value Type :
<div class="table-scroll-wrapper has-inner-focus" tabindex="0" role="group" aria-label="Horizontally scrollable data"><table class="table"><caption class="visually-hidden">Registry Value Types</caption>
<thead>
<tr>
<th>Value</th>
<th>Type</th>
</tr>
</thead>
<tbody>
<tr>
<td>REG_BINARY</td>
<td>Binary data in any form.</td>
</tr>
<tr>
<td>REG_DWORD</td>
<td>A 32-bit number.</td>
</tr>
<tr>
<td>REG_DWORD_LITTLE_ENDIAN</td>
<td>A 32-bit number in little-endian format. Windows is designed to run on little-endian computer architectures. Therefore, this value is defined as REG_DWORD in the Windows header files.</td>
</tr>
<tr>
<td>REG_DWORD_BIG_ENDIAN</td>
<td>A 32-bit number in big-endian format. Some UNIX systems support big-endian architectures.</td>
</tr>
<tr>
<td>REG_EXPAND_SZ</td>
<td>A null-terminated string that contains unexpanded references to environment variables (for example, "%PATH%"). It will be a Unicode or ANSI string depending on whether you use the Unicode or ANSI functions. To expand the environment variable references, use the ExpandEnvironmentStrings function.</td>
</tr>
<tr>
<td>REG_LINK</td>
<td>A null-terminated Unicode string that contains the target path of a symbolic link that was created by calling the RegCreateKeyEx</strong></a> function with REG_OPTION_CREATE_LINK.</td>
</tr>
<tr>
<td>REG_MULTI_SZ</td>
<td>A sequence of null-terminated strings, terminated by an empty string (\0). The following is an example: <em>String1</em>\0<em>String2</em>\0<em>String3</em>\0<em>LastString</em>\0\0 The first \0 terminates the first string, the second to the last \0 terminates the last string, and the final \0 terminates the sequence. Note that the final terminator must be factored into the length of the string.</td>
</tr>
<tr>
<td>REG_NONE</td>
<td>No defined value type.</td>
</tr>
<tr>
<td>REG_QWORD</td>
<td>A 64-bit number.</td>
</tr>
<tr>
<td>REG_QWORD_LITTLE_ENDIAN</td>
<td>A 64-bit number in little-endian format. Windows is designed to run on little-endian computer architectures. Therefore, this value is defined as REG_QWORD in the Windows header files.</td>
</tr>
<tr>
<td>REG_SZ</td>
<td>A null-terminated string. This will be either a Unicode or an ANSI string, depending on whether you use the Unicode or ANSI functions.</td>
</tr>
</tbody>
</table></div>

[ This Table was taken From ](https://docs.microsoft.com/en-us/windows/win32/sysinfo/registry-value-types)

## Roots Keys :
|Key | Descriptions 
|-----|------------
|HKEY_CLASSES_ROOT (HKCR) | information related to file types and Properties
|HKEY_CURRENT_CONFIG (HKCC) | information related to the hardware configurations 
|HKEY_CURRENT_USER (HKCU) | inforamtion related the setting configuration for the current user 
| HKEY_LOCAL_MACHINE | information about the local machine related to input/output devices, memory, and drivers. 
| HKEY_PERFORMANCE_DATA | Provides information related to system performance 
|HKEY_USERS | Provides information related to the default settings assigned to new users 

# Run and RunOnce 
Run and RunOnce registry keys cause programs to run each time a user logs on. The data value for a key is a command line no longer than 260 characters. Register programs to run by adding entries of the form description-string=commandline. You can write multiple entries under a key. If more than one program is registered under any particular key, the order in which those programs run is indeterminate.

The Windows registry includes the following four Run and RunOnce keys:

    HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Run
    HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\RunOnce
    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\Run
    HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\RunOnce

```reg ``` : reg is command line to interacte with registry 

sccren shot 

``` reg query  HKEY_LOCAL_MACHINE\Software\Microsoft\Windows\CurrentVersion\Run ``` : to query a reg

sccrenn shot 

``` reg delete ``` : to delete a registry 

sccren shot 

``` reg add ``` : to add a registry 

scren shot 

