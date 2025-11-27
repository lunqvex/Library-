Local Library
---
```lua
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/lunqvex/Library-/refs/heads/main/Latest"))()

```
---

Window
---
```lua
local window = library:CreateWindow("Your Title")

```
---

Folder
---
```lua
local folder = window:AddFolder("Folder")
```
---

Button
---
```lua
folder:AddButton({
    text = "Click me",
    callback = function()
        print("hello world")
    end
})

```

---

Toggle
---
```lua
folder:AddToggle({
    text = "Toggle",
    callback = function(v)
        print(v)
    end
})

```
---

Label
---
```lua
folder:AddLabel({
    text = "This Is Sick!"
})
```
---

Slider
---
```lua
folder:AddSlider({
    text = "Fov",
    min = 70,
    max = 170,
    callback = function(v)
        print(v)
    end
})
```
---

Textbox
---
```lua
folder:AddBox({
    text = "Enter Text",
    callback = function(txt)
        print(txt)
    end
})
```
---

Color Picker
---
```lua
folder:AddColor({
    text = "Color Picker",
    callback = function(color)
        print(color)
    end
})
```
---

Dropdown / List
---
```lua
folder:AddList({
    text = "Color",
    values = {"Red", "Green", "Blue"},
    callback = function(value)
        print("Selected:", value)
    end
})
```
---

Keybind
---
```lua
folder:AddBind({
    text = "Bind",
    key = "X",
    callback = function()
        print("Pressed!")
    end
})
```
---
Close Library
---
```lua
library:Close()
```
---

Init Library (REQUIRED)
---
```lua
library:Init()
```