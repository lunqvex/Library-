📌 NOTE: This script is modified into pink color!

Local Library:
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/yourname/yourrepo/main/library.lua"))()

Window:
local window = library:CreateWindow("Your Title")

Folder:
local folder = window:AddFolder("Folder")

Button:
folder:AddButton({
    text = "Click me",
    callback = function()
        print("hello world")
    end
})

Toggle:
folder:AddToggle({
    text = "Toggle",
    callback = function(v)
        print(v)
    end
})

Label:
folder:AddLabel({
    text = "This Is Sick!"
})

Slider:
folder:AddSlider({
    text = "Fov",
    min = 70,
    max = 170,
    callback = function(v)
        print(v)
    end
})

Textbox:
folder:AddBox({
    text = "Enter Text",
    callback = function(txt)
        print(txt)
    end
})

Color Picker:
folder:AddColor({
    text = "Color Picker",
    callback = function(color)
        print(color)
    end
})

List / Dropdown:
folder:AddList({
    text = "Color",
    values = {"Red", "Green", "Blue"},
    callback = function(value)
        print("Selected:", value)
    end
})

Keybind:
folder:AddBind({
    text = "Bind",
    key = "X",
    callback = function()
        print("Pressed!")
    end
})

Close Library:
library:Close()

Init Library:
library:Init()

Credits:Vex Hub
