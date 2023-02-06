# IMPORTANT

ReVanced manager has been released. Please go [here](https://github.com/revanced/revanced-manager/releases/latest) to download the latest version.

# Termux 

Watch this [YouTube video](https://youtu.be/CAp8X0fC1to) for reference.

Now at first download termux app from [f-droid](https://f-droid.org/en/packages/com.termux) or release files from [this repo](https://github.com/n-34/revanced-termux/releases/download/main/Termux_0.118.0.apk).


Then run the following commands serially:


- `termux-setup-storage`

- `pkg upgrade`

- `pkg install wget openjdk-17 -y`

- `wget https://github.com/n-34/revanced-termux/releases/download/main/aapt2.zip`

- `wget https://github.com/n-34/revanced-termux/releases/download/main/cli.jar`

- `wget https://github.com/n-34/revanced-termux/releases/download/main/integrations.apk`

- `wget https://github.com/n-34/termux/releases/download/main/patches.jar`

- `unzip aapt2.zip`

- `cd aapt2`

- `chmod +x aapt2`

- `cd`

- `java -jar cli.jar -b patches.jar -m integrations.apk -c -a /storage/emulated/0/apps/revanced/youtube.apk -o /storage/emulated/0/apps/revanced/revanced.apk --custom-aapt2-binary aapt2/aapt2 -e premium-heading -e custom-branding -e theme`

> - `-a /xxx/xxx/*.apk` it is the location of the *.apk file to be patch. 

> - `-o /xxx/xxx/*.apk` it is the location of the output patched *.apk.

**All available patches are listed [here](https://github.com/nibir34/termux/blob/main/patch%20list(youtube)).**



# Remove files from termux home directory

- `rm file_name.xxx`

- `rm -rf folder_name`
