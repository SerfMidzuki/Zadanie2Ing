# Zadanie2Ing
from tkinter import *
from tkinter import messagebox

def click():
    Name= Name_entry.get()
    messagebox.showinfo ('Имя получено', f"Привет,{Name}")

root= Tk()
root.title('Приветствие')
root.geometry('500x400')
root['bg'] = 'black'

main_label = Label(root, text="Введите имя", font="Arial 13", bg="black",fg='white')
main_label.pack()

Name_label = Label(root, text="Имя",font='Arial 10', bg='black',fg='white', padx=9, pady=7)
Name_label.pack()

Name_entry = Entry(root, bg='black', fg='Green',font='Arial 15')
Name_entry.pack()

Otpravit_btn = Button(root, text='Отправить имя',command=click)
Otpravit_btn.pack(padx=10, pady=8)


root.mainloop()
