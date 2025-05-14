# CODM CHECKER
![](https://i.imgur.com/SDlnfyp.jpeg)
Checking valid Garena accounts that are bound in CODM (Call of Duty Mobile) using the user combolist.

### Installing
• Clone this repository to your download folder
```bash
cd storage; cd downloads; git clone https://github.com/sintxcs/checker.git
```
After cloning the repository to your download folder, check if there is a folder name checker. Move all your txt/combolist to that folder and you're ready to go!

• Start or run the script
```bash
cd checker; python checker.sin
```
• Missing modules?
```bash
pip install -r requirements.txt
```

### Features:
• Full capture details
<br> • Sorted results
<br> • Clean check summary
<br> • Duplicate separator
<br> • Garena Account (CODM Fail) separator
<br> • Auto pause when Captcha (403) for changing IP and retry if Rate Limit (429) in Garena API
<br> • Auto-saving and rotating cookies
<br> • Auro url remover

### Credits.js
This is an API for calling back the endpoint to make a key for users to access the checker.sin

### Server.js
Another API to extract the valid account from the provided txt files. It uses the POST method to send the data from the checker.sin to the server side.

### Requirements.txt
List of modules that are used in this tool.
<br>
> [!WARNING]  
> *This tool is for educational purposes only. I won't take any responsibility if any users take advantage of this and exploit it for illicit activities.*
