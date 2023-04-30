from tkinter import *
import datetime
import winsound
import time

def alarm(set_alarm_timer):
    while True:
        time.sleep(1)
        current_time = datetime.datetime.now()
        now = current_time.strftime("%H:%M:%S")
        date = current_time.strftime("%d/%m/%Y")
        if now == set_alarm_timer:
            print("Wake up, Make things happen!")
            winsound.PlaySound("sound.wav",winsound.SND_ASYNC)
            break

def actual_time():
    set_alarm_timer = f"{hour.get()}:{min.get()}:{sec.get()}"
    alarm(set_alarm_timer)

clock = Tk()
clock.title("Alarm Clock")
clock.geometry("600x600")

setYourAlarm = Label(clock,text = "Alarm Clock",fg="brown",font=("Helevetica",20)).place(x=70, y=20)
time_format=Label(clock, text= "Enter time to wake up in 24-Hour format", fg="Black",font="Arial").place(x=10,y=70)
addTime = Label(clock,text = "Hour",font=40).place(x=20,y=105)
addTime = Label(clock,text = "Minutes",font=40).place(x=20,y=130)
addTime = Label(clock,text = "Seconds",font=40).place(x=20,y=155)


hour = StringVar()
min = StringVar()
sec = StringVar()

hourTime= Entry(clock,textvariable = hour,bg = "white",width = 15).place(x=120,y=110)
minTime= Entry(clock,textvariable = min,bg = "white",width = 15).place(x=120,y=135)
secTime = Entry(clock,textvariable = sec,bg = "white",width = 15).place(x=120,y=160)

submit = Button(clock,text = "Set Alarm",font=40,fg="purple",width = 20,command = actual_time).place(x =70,y=200)

clock.mainloop()
