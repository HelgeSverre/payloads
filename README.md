# Rubber Ducky Payloads

These files are [Rubber Ducky](https://hakshop.myshopify.com/collections/usb-rubber-ducky/products/usb-rubber-ducky-deluxe) payloads that I have personally written and tested.

All .bin files are encoded to work with NORWEGIAN keyboard layouts, if you want to encode them for other countries, you have to copy-paste the script into [this encoder](http://www.ducktoolkit.com/Encoder.jsp) and select the keyboard layout that is relevant for you.

## Payloads

### dl-run-no-powershell.bin
This payload will open the run prompt (Windows key + r), write notepad.exe and press enter, it will then write out a VB Script that will download a file and save it to the temporary directory as "program.exe", it will then save the VB script as test.vbs in the %temp% folder.

The file it currently downloads is this file: test.helgesverre.com/bot/example.exe which is a program I have created in AutoIT that will play a sound at 1000Hz for 1 second.


It will then open the run prompt again and run the VB Script by using the command:  
```
cscript %temp&\test.vbs
```

which will download the program mentioned above.

it will wait 5 seconds, then it opens the run prompt again and runs the program.exe file by using this command:
```
%temp%\program.exe
```


## License
All script files and .bins are free to use and modify, however, if it breaks your computer it is your own responsibility.


Do no evil.