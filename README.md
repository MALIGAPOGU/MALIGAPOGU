import tkinter as tk
# Create the main window
root = tk.Tk()
root.title("Basic Human Body Simulation")

# Create a canvas to draw on
canvas = tk.Canvas(root, width=400, height=600)
canvas.pack()

# Draw a head
canvas.create_oval(150, 50, 250, 150, fill="peachpuff")

# Draw a torso
canvas.create_rectangle(175, 150, 225, 300, fill="lightblue")

# Draw arms
canvas.create_line(175, 175, 100, 200, fill="black", width=5)
canvas.create_line(225, 175, 300, 200, fill="black", width=5)

# Draw legs
canvas.create_line(190, 300, 150, 450, fill="black", width=5)
canvas.create_line(210, 300, 250, 450, fill="black", width=5)

# Run the GUI event loop
root.mainloop()
