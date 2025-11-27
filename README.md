ðŸ“Œ NOTE  
This script is modified into pink color!

---

Local Library
---
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/lunqvex/Library-/refs/heads/main/Latest"))()

---

Window
---
local window = library:CreateWindow("Your Title")

---

Folder
---
local folder = window:AddFolder("Folder")

---

Button
---
folder:AddButton({
    text = "Click me",
    callback = function()
        print("hello world")
    end
})

---

Toggle
---
folder:AddToggle({
    text = "Toggle",
    callback = function(v)
        print(v)
    end
})

---

Label
---
folder:AddLabel({
    text = "This Is Sick!"
})

---

Slider
---
folder:AddSlider({
    text = "Fov",
    min = 70,
    max = 170,
    callback = function(v)
        print(v)
    end
})

---

Textbox
---
folder:AddBox({
    text = "Enter Text",
    callback = function(txt)
        print(txt)
    end
})

---

Color Picker
---
folder:AddColor({
    text = "Color Picker",
    callback = function(color)
        print(color)
    end
})

---

Dropdown / List
---
folder:AddList({
    text = "Color",
    values = {"Red", "Green", "Blue"},
    callback = function(value)
        print("Selected:", value)
    end
})

---

Keybind
---
folder:AddBind({
    text = "Bind",
    key = "X",
    callback = function()
        print("Pressed!")
    end
})

---

Close Library
---
library:Close()

---

Init Library (REQUIRED)
---
library:Init()

---

Credits
---
LunqVex