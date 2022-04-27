#importing modules

import random
import array
import tkinter as Tk
from tkinter import *
from tkinter import messagebox

#Creating Window

FirstWindow=Tk()
FirstWindow.title("Random Password Generator")
FirstWindow.minsize(width=600, height=400)
FirstWindow.resizable(True, True) #Width, Height
icon=PhotoImage(file="C:/Users/Aaditya/Desktop/Python New Project/icon.png") #Setting icon
FirstWindow.iconphoto(False, icon) #Setting icon
FirstWindow.configure(background="Black") #Background

#Creating Password Length Entry Box

length=Entry(FirstWindow, font=("Bahnschrift SemiBold", 20))
length.place(relx=0.5, rely=0.5, anchor=CENTER)

#Creating Generate Button

def PassGenerate():
    messagebox.askokcancel('Password', 'Your Randomly Generated Password is: ')
Generate=Button(FirstWindow, text="Generate", bd=5, bg="white", fg="black", command=PassGenerate)
Generate.place(relx=0.5, rely=0.5, anchor=CENTER)

#Creating Exit Button

Exit=Button(FirstWindow, text="Exit Password Generator", bd=1, bg="red", fg="white", command=FirstWindow.destroy)
Exit.pack(side='bottom')


lower=['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']
upper=['A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z']
number=['1','2','3','4','5','6','7','8','9','0']
symbol=['!','@','#','$','%','^','&','*','(',')','[',']','{','}','/','?']
all=(lower+upper+number+symbol)
length=int(input("Enter the length of the password: "))
password="".join(random.sample(all,length))
print("The password you generated is: ",password)

FirstWindow.mainloop()
