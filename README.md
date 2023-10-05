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
