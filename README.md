# BitLocker

I experienced this problem on my Dell xps 13 9360, but apparently it is common to many different models. 
It happens every now and then that after a BIOS update, BitLocker starts encrypting your harddrive without any apparent reasons. The huge problem is that you can't boot your laptop without the key ID, which does not exist!

The suggested solution to have you computer back is to reinstall windows from scratch, implying the complete loss of all your data.

Actually there is a reason behind this and it is that Dell screwed up with the latest update. 
This problem is very annoying and I spent a few hours worrying about all my data. 

The solution is simpler that it may sound and you need just to follow these simple steps:
1. Power on your laptop
2. Enter the BIOS by pressing F2 when the Dell logo appears
3. Go in **Boot Sequence** and select **UEFI**
4. Go in **Security**, **TPM 2.0 Secuity** and restore it to the factory settings
5. Exit the BIOS and restart your laptop

If you don't see the TPM item of the list, there are different ways to proceed:
- disconnect your battery for 30 seconds 
- drain your battery down until your laptop is no longer able to switch on and press the on button for a minute

At this point, repeat the previous list of steps and the TPM item should appear in the list.

This procedure let me overcome this crazy BitLocker problem without losing a single bit of data.

