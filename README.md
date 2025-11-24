Tora Library

Simple Ui Library. With Clean And Sexy Ui Credit To Tora

Setup The Library

local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/liebertsx/Tora-Library/main/src/library",true))()

Or Use The New

local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/liebertsx/Tora-Library/main/src/librarynew",true))()

Adding Tab

local tab = library:CreateWindow("Your Title")

Adding Folder

local folder = tab:AddFolder("Folder")

Adding Button

folder:AddButton({ 	text = "Click me", 	flag = "button", 	callback = function() 	print("hello world") end })

Adding Toggle

folder:AddToggle({ 	text = "Toggle", 	flag = "toggle", 	callback = function(v) 	print(v) end })

Adding Label

folder:AddLabel({ 	text = "This Is Sick!", 	type = "label" 	})

Adding Slider

folder:AddSlider({ 	text = "Fov", 	min = 70, 	max = 170, 	dual = true, 	type = "slider", 	callback = function(v) 	print(v) end })

Adding TextBox

folder:AddColor({ 	text = "Color Picker", 	flag = "color", 	type = "color", 	callback = function(v) 	print(v) end })

Adding Dropdown

folder:AddList({ text = "Color", values = {"Red", "Green", "Blue"}, callback = function(value) print("Selected color:", value) end, open = false, flag = "color_option" })

Adding Bind

folder:AddBind({ text = "bind", key = "X", hold = false, callback = function() end })

Close Lib

library:Close()

Final (REQUIRED OR THE UI WILL NOT SHOW)

library:Init()

Credits : Tora Is Me

