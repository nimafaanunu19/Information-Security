# Almost Gotcha!  
## Evil USB  

### Requirements  
- **USB Rubber Ducky** (or any small computer that can act as a HID and reads DuckyScript)  
- **MicroSD card**  
- The `almost_gotcha.txt` file compiled into an `inject.bin` file  

---

### Introduction  
The **Evil USB** is a password-stealing penetration tool. It utilizes **DuckyScript** to transfer an encoded Python script. This script:  
1. Opens Google Chrome.  
2. Extracts all usernames and passwords from whoever is logged in.  
3. Compiles these credentials into an email draft.  

The attack concludes by ALMOST sending the credentials to a recipient of your choice.  

---

### Usage  
1. Download the DuckyScript and input it into Hak5's Payload Generator: [https://payloadstudio.com/login/](https://payloadstudio.com/login/)  
2. Transfer the generated `inject.bin` file onto a microSD card.  
   - **Note:** The microSD card must:  
     - Be formatted as **FAT/FAT32**.  
     - Contain **no other files or folders**.  
3. Insert the microSD card into the Rubber Ducky.  
4. Deploy the Evil USB for a surprising result.  

---

### Potential Customization  
This template can be customized in various ways:  
- **Simple changes:** Modify the email address the usernames and passwords are sent to.  
- **Advanced tweaks:** Hide processes in the background to prevent user detection.  

> **Note:** The targeted machines for this template already had Python installed.  
> If Python isn't installed on your target system, you'll need to include its installation in the DuckyScript.  

---

### Usage Agreement  
The contents of this repository are intended for **educational purposes only**.  

---

Enjoy responsibly!
