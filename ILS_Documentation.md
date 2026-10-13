# Troubleshooting During ILS Building

During ILS building, I did not have many issues--I found the Burns book and coding videos to be pretty straightforward. One issue I did have was the Wordpress file not unzipping due to the command not being installed on my VM. Unfortunately, I do not have the error messages from when it happened, but I did run my history to show the command I used to fix it. 

<img width="391" height="130" alt="Screenshot 2026-10-13 at 5 13 38 PM" src="https://github.com/user-attachments/assets/2fa37a93-03c7-468f-a21d-dd158d208f9e" />

After pulling the Wordpress zip to my VM I attempted the following code: 
```
sudo unzip latest.zip
```

The output was 'sudo: unzip: command not found.'
Fortunately, I was following the coding video provided by Dr. R which had the same issue. If I were not following the video, a simple search of the error would have brought me to the same conclusion. Nonetheless, I was able to copy the code from the video to install the command:
```
sudo apt-get install unzip
```

After installing the unzip command, I was able to unzip my Wordpress file using 
```
sudo unzip latest.zip
```

This allowed me to complete my Wordpress installation and carried over to unzipping my Omeka file on the same VM. 

## Condensed Steps: 

If you are trying to unzip a file in Ubuntu and you get the error 'sudo: unzip: command not found,' you need to install the unzip command using 
```
sudo apt-get install unzip
```
Try unzipping your file again. This should solve your issue, unless a different error is thrown. 
