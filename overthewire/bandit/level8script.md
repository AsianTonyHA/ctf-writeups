from collections import Counter
import tkinter as tk
from tkinter import filedialog

# Open file picker dialog
root = tk.Tk()
root.withdraw()
file_path = filedialog.askopenfilename(title="Select data.txt")

with open(file_path, "r") as f:
    lines = f.readlines()

counts = Counter(lines)

for line, count in counts.items():
    if count == 1:
        print("Password:", line.strip())

is my python program basically just checks like whats on the line and then if count == 1 then give me whatever that line is and thats the flag
