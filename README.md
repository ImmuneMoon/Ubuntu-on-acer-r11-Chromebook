---

## **Ubuntu-on-acer-r11-Chromebook**

2 Years ago, I put Ubuntu on a chromebook, and didnt think to document the process besides a social media post. **So I'm doing it now**, lets make more old devices **reusable** and **reduce e-waste.**

---

# **Installing Ubuntu on acer r11 Chromebook**

---

## **First off,**
youll need to remove the write protect screw from the motherboard. There are several screws on the back that can be romoved with a phillips head screwdriver, youll need a set from a specialty kit most likely,  
**especially for the actual write protect screw.**

### **Once you take the back off**
you'll see a big black screw nearish to the left-center of the motherboard, it'll have an arrow pointing to it. Just take it out and throw it away, theres no point and putting chrome os on it again. If you're not sure what to remove, just google "acer r11 Chromebook write protect screw". Also,  
**it strips easily, so be careful.**

---

# **Enable Developer Mode:**
Hold down the Esc and Refresh keys and Power button to enter recovery mode. At the recovery screen, press  
> **Ctrl+D,**

agree to the prompt, and you’ll boot into developer mode. When you transition to developer mode,  
### **your Chromebook’s local data will be erased,**  
it can take a little while, just be patient.

### **From now on**, 
whenever you boot your Chromebook, you’ll see a warning screen. **This is normal.**  
You’ll need to press  
> **Ctrl+D,**

or wait **30 seconds**  to continue booting.

Once in developer mode, **dont worry about setting up an account,** just skip through and log in under guest.

---

## **Now you install your new bios**
Log in to your wifi and press  
> **CTRL+ALT+T**

to open a crosh session in your browser.  

We're going to use the  **johnlewis BIOS,**  cuz I like it and it's simple and was the best choice at the time. The johnlewis BIOS is a custom version of seaBios

Then type  
> **shell**

and hit  
> **enter**

there, Type:
> **cd;bash <(curl https://johnlewis.ie/flash_cb_fw.sh)**

Choose the option to  
> **Modify my Chromebook’s RW_LEGACY slot**

and follow the on-screen instructions.

---

### **Enable USB boot**
Pressing  
> **Ctrl + D**
 
at the screen with the red exclamation mark on startup will take you to your **Chrome OS install**, but pressing  
> **Ctrl + L**

will take you to the **BIOS screen** where you will boot from your USB drive that you either have prepared, or will make after this.

---

### **Let’s turn on the Ctrl + L functionality next:**

1. Press:
   > **Ctrl + D**
   
   at the initial startup screen to load Chrome OS.  
2. Press:
   > **Ctrl + Alt + F2**
   
   at the Chrome OS login screen.  

Login using the password:
> **chronos**  

At the terminal prompt, type:
> **sudo crossystem dev_boot_usb=1 dev_boot_legacy=1**
  
Power off the Chromebook by typing in: 
> **sudo poweroff**

Now on startup, if you press  
> **Ctrl + L,**

you will get the  
> **BIOS screen**

instead of Chrome OS.

---

## **Ubuntu thumb drive,**  
After that, it's time to use or make a live Ubuntu thumb drive, or an operating system of your choice, the lighter the better. Some other recommendations are **Kubuntu**, **Kali** (for the hacker bros), and googling **"lightweight linux distros."** If you need help building a bootable USB, **google is your friend** once again.

---

### **After bootable drive is ready,**  
Turn off your Chromebook, plug it in to a power supply, then turn it back on. Hit  
> **Ctrl + L**

again, then  
> **esc**

and select the USB stick name. After, it might take a second to load but just follow the install prompts. I used  
> **RW_LEGACY**

I believe, but once the install is finished, turn off your Chromebook and unplug your thumbdrive.

And now when you turn it back on it'll be on that warning screen again, but just hit  
> **Ctrl + L, esc,**

then select the internal storage and it'll boot into your Ubuntu install.

You’ll have to do this every time unless you get another bios or modify it for a fast boot, or just wait 30 seconds for it to power on by itself. 
### **It'll beep a few times when you just let it boot on its own, that's normal.**

---

# **Congrats, you should have a working ex-chromebook linux machine!**
