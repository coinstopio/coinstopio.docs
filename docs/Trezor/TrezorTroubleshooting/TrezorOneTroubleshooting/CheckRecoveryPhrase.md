# Check Recovery Phrase / Dry-Run Recovery

The dry-run recovery is a useful way to test your recovery seed. It is recommended to test your seed before you wipe the Trezor device or before every a firmware update. It allows you to double check that your recovery seed backup is correct.

By starting the verification process, you are telling the device that you want to run the recovery process, but you do not want the device to remember the seed. Instead, in the end, the device compares the seed saved in its storage and the seed you have just “recovered,” and the result of this comparison is sent to the Wallet interface. If the seeds match, a message on your Trezor device screen will tell you your backup is okay. If it is not the same, then the ice screen will show you an error.

_Note: The warnings shown on the device during this process are related to a full recovery. If you are running dry-run, you can ignore the warnings related to the recovery process._

  

**DRY RUN RECOVERY**

  

1.  Go to [wallet.trezor.io](http://wallet.trezor.io)
2.  Click on your **Trezor device name** in the top-left corner and go to the **advanced** tab
3.  Go to the **check recovery seed** section and click on **check recovery seed**
4.  Select the **number of words** in your recovery seed and click on **continue**
5.  **Follow the instructions** on your computer screen and your Trezor device