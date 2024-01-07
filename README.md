

The script uses the pynput library to monitor and log keystrokes.
It records keystrokes in a file named "key_log.txt."


It gathers information about the computer, such as hostname, IP addresses (both public and private), processor, system details, machine type, etc.
This information is saved in a file named "syseminfo.txt."


It captures data from the clipboard and saves it in a file named "clipboard.txt."


The script records audio from the computer's microphone for a specified duration (controlled by the microphone_time variable) and saves it as an audio file named "audio.wav."


It takes a screenshot of the desktop and saves it as an image file named "screenshot.png."


The collected information (key logs, system info, clipboard data, screenshot, and audio recording) is emailed to a specified email address. The email is sent using Gmail's SMTP server.


It encrypts sensitive files (system information, clipboard data, and key logs) using the cryptography library and a specified encryption key.
Encrypted files are then emailed to the specified email address.


After sending the information, the script sleeps for 120 seconds (controlled by time.sleep(120)).
It then deletes the original unencrypted files, leaving only the encrypted versions.
