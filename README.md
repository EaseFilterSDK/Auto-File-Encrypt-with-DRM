# [Auto File DRM Encryption SDK](https://www.easefilter.com/kb/auto-file-drm-encryption-tool.htm)
The EaseFilter Encryption Filter Driver(EEFD) SDK allows you to develop the auto file encryption application. The DRM encryption application allows you to embed the custom digital rights management( DRM) data to the encrypted files. With the embedded DRM in the encrypted file, you can protect and monitor your business critical document such as intellectual property and product design, wherever it lives or travels, you can allow or block the encrypted file access, you can expire the encrypted file, grant or revoke the access of the encrypted files anywhere and anytime even they were distributed.

![File Encryption](https://www.easefilter.com/Images/TransparentFileEncryption.png)

[EaseFilter Encryption Filter Driver(EEFD) SDK](https://www.easefilter.com/kb/transparent-on-access-file-encryption-SDK.htm)

EEFD is a file system file level encryption filter driver. It intercepts the I/O requests targeted at a file system. By intercepting the request before it reaches its intended target file system, the filter driver can encrypt or decrypt the data buffer provided by the original target of the request. 

![DRM Encryption Demo](https://www.easefilter.com/images/IsolationFilter.png)

The EEFD provides a comprehensive security solution to develop the transparent on access file level encryption products, to encrypt the newly created files transparently, to authorize or block the on access encryption/decryption under the control of client-defined policy. With the EEFD SDK, you can setup the control policies to protect your encrypted files, prevent your sensitive files from being read or copied out. 

With the access control policies, you can setup the whitelist processes or users who can read the encrypted files, they can get the clear text of the encrypted files. You can setup the blacklist processes or users who cant read the encrypted files, they will get the raw cipher text of the encrypted files.
 
## The advantages of the EEFD SDK:
1. **Completely transparent file encryption in file system level.** The encryption process was done in the write IO request, the decryption process was done in the read IO request, there are no extra IO request needed, it is completely transparent to the applications or users, the encryption or decryption doesn't require the application to interfere. 
2. **Keep encrypted file on disk all the time.** Since the decryption data only was kept in memory, there are no extra file created for the decryption.
3. **Process Access Restriction.** EaseFilter Encryption SDK was implemented with [Isolation Mini Filter Driver](https://www.easefilter.com/kb/Isolation_Filter_Driver.htm). The EEFD uses the unique private memory session for every encrypted file open, the clear data won't be shared with other processes even it was opened with memory mapped. 
4. **Random block level decryption.** You can decrypt the blocks of the file, you don't need to decrypt the whole file for all the time. For large encrypted file, if you only want to read the blocks of the data, it will improve the performance dramatically.
5. **High encryption or decryption performance.** EaseFilter Encryption Engine utilizes the US FIPS 140-2 compliant Microsoft CNG libraries, it can support AES-NI (or the Intel Advanced Encryption Standard New Instructions; AES-NI), at an algorithm level AES-NI provides significant speedup of AES. For non-Parallel modes of AES operation (CBC encrypt), AES-NI can provide 2-3 fold gain in performance over a completely software encryption. For parallel modes of AES operation (CBC-decrypt, CTR), AES-NI can provide 10x improvement over a completely software encryption.

## A C# Auto File DRM Encryption Example
The C# auto file DRM encryption example allows you to embed the build in DRM data to the new encrypted file, the build in DRM data includes the access control policies, allow you to control the encrypted file access without the center server. You also can embed the custom DRM data to the new encrypted file, and store your access control policies in the center server, the encrypted file access can be controlled and monitored by the center server, you can expire the encrypted file, grant or revoke the access of the encrypted files anywhere and anytime even they were distributed, you will know who and when your encrytped file was accessed.

![File Encryption Demo](https://www.easefilter.com/images/autoencrypt.png) 
![drm setting](https://www.easefilter.com/images/DRM.png)

[Read more about auto file encryption example](https://www.easefilter.com/kb/auto-file-drm-encryption-tool.htm)

## EaseFilter File System Filter Driver SDK Reference
| Product Name | Description |
| --- | --- |
| [Cloud File System SDK](https://www.easefilter.com/cloud/cloud-file-system-sdk.htm) | EaseFilter Cloud File System SDK Introduction. |
| [CloudTier Storage Tiering SDK](https://www.easefilter.com/cloud/storage-tiering-sdk.htm) | EaseFilter Storage Tiering Filter Driver SDK Introduction. |
| [File Monitor SDK](https://www.easefilter.com/kb/file-monitor-filter-driver-sdk.htm) | EaseFilter File Monitor Filter Driver SDK Introduction. |
| [File Control SDK](https://www.easefilter.com/kb/file-control-file-security-sdk.htm) | EaseFilter File Control Filter Driver SDK Introduction. |
| [File Encryption SDK](https://www.easefilter.com/kb/transparent-file-encryption-filter-driver-sdk.htm) | EaseFilter Transparent File Encryption Filter Driver SDK Introduction. |
| [Registry Filter SDK](https://www.easefilter.com/kb/registry-filter-drive-sdk.htm) | EaseFilter Registry Filter Driver SDK Introduction. |
| [Process Filter SDK](https://www.easefilter.com/kb/process-filter-driver-sdk.htm) | EaseFilter Process Filter Driver SDK Introduction. |
| [EaseFilter SDK Programming](https://www.easefilter.com/kb/programming.htm) | EaseFilter Filter Driver SDK Programming. |

## EaseFilter SDK Sample Projects
| Sample Project | Description |
| --- | --- |
| [CloudTier Storage Tiering Demo](https://www.easefilter.com/cloud/cloudtier-storage-tiering-demo.htm) | A HSM File System Filter Driver Demo. |
| [CloudTier S3 Tiering Demo](https://www.easefilter.com/cloud/cloudtier-s3-intelligent-tiering-demo.htm) | CloudTier S3 Intelligent Tiering Demo. |
| [Cloud File DR S3 Demo](https://www.easefilter.com/cloud/cloud-file-dr-demo.htm) | Cloud File DR S3 Demo. |
| [Amazon S3 File Explorer Demo](https://www.easefilter.com/cloud/s3-browser-demo.htm) | Amazon S3 File Explorer Demo. |
| [Auto File DRM Encryption](https://www.easefilter.com/kb/auto-file-drm-encryption-tool.htm) | Auto file encryption with DRM data embedded. |
| [Transparent File Encrypt](https://www.easefilter.com/kb/AutoFileEncryption.htm) | Transparent on access file encryption. |
| [Secure File Sharing with DRM](https://www.easefilter.com/kb/DRM_Secure_File_Sharing.htm) | Secure encrypted file sharing with digital rights management. |
| [File Monitor Example](https://www.easefilter.com/kb/file-monitor-demo.htm) | Monitor file system I/O in real time, tracking file changes. |
| [File Protector Example](https://www.easefilter.com/kb/file-protector-demo.htm) | Prevent sensitive files from being accessed by unauthorized users or processes. |
| [FolderLocker Example](https://www.easefilter.com/kb/FolderLocker.htm) | Lock file automatically in a FolderLocker. |
| [Process Monitor](https://www.easefilter.com/kb/Process-Monitor.htm) | Monitor the process creation and termination, block unauthorized process running. |
| [Registry Monitor](https://www.easefilter.com/kb/RegMon.htm) | Monitor the Registry activities, block the modification of the Registry keys. |
| [Secure Sandbox Example](https://www.easefilter.com/kb/Secure-Sandbox.htm) |A secure sandbox example, block the processes accessing the files out of the box. |
| [FileSystemWatcher Example](https://www.easefilter.com/kb/FileSystemWatcher.htm) | File system watcher, logging the file I/O events. |
| [ZeroTrust Example](https://www.easefilter.com/kb/zero-trust-file-access-control-demo.htm) | Zero trust file access control with encryption feature. |

## Filter Driver Reference

* [Understand MiniFilter Driver](https://www.easefilter.com/kb/understand-minifilter.htm)
* [Understand File I/O](https://www.easefilter.com/kb/File_IO.htm)
* [Understand I/O Request Packets(IRPs)](https://www.easefilter.com/kb/understand-irps.htm)
* [Filter Driver Developer Guide](https://www.easefilter.com/kb/DeveloperGuide.htm)
* [MiniFilter Filter Driver Framework](https://www.easefilter.com/kb/minifilter-framework.htm)
* [Isolation Filter Driver](https://www.easefilter.com/kb/Isolation_Filter_Driver.htm)

## Support
If you have questions or need help, please contact support@easefilter.com 

[Home](https://www.easefilter.com/) | [Solution](https://www.easefilter.com/solutions.htm) | [Download](https://www.easefilter.com/download.htm) | [Demos](https://www.easefilter.com/online-fileio-test.aspx) | [Blog](https://blog.easefilter.com/) | [Programming](https://www.easefilter.com/kb/programming.htm)
