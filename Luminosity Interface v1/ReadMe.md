# V3rmillon: https://v3rmillion.net/showthread.php?tid=1095130

# documentation:
Luminosity Interface never uses Methods for class creation; Methods (such as Array:Function()) are almost always exclusively for functions that operate on the instance, instead, for element creation, it always looks like: Luminosity.new().

Classes:
Window
Luminosity.new(Title, Header, Icon)

Tab
Window.Tab(Title, Icon)

Container
Tab.Folder(Title, Value)
Tab.Cheat(Title, Value)

Options
Container.TextLabel(Text)
Container.Button(Text, Callback)
Container.Switch(Text, Callback)
Container.Toggle(Text, Callback)
Container.Textbox(Text, PlaceHolder, Callback)

# Examples
```lua
local Luminosity = loadstring(game:HttpGet("https://raw.githubusercontent.com/iHavoc101/Genesis-Studios/main/UserInterface/Luminosity.lua", true))()

local Window = Luminosity.new("Luminosity UI", "v1.0.0", 4370345701)

local Tab1 = Window.Tab("Tab 1", 6026568198)
local Folder = Tab1.Folder("Options", "A bunch of options you can use")
Folder.Button("Button", "Click", function()
print("Button Clicked")
end)
Folder.Switch("Switch", function(Status)
print("Switch Triggered: " .. tostring(Status))
end)
Folder.Toggle("Toggle", function(Status)
print("Toggle Triggered: " .. tostring(Status))
end)
Folder.Toggle("Toggle", function(Status)
print("Toggle Triggered: " .. tostring(Status))
end)
Folder.TextBox("Textbox", "Placeholder", function(Text)
print("TextBox Triggered: " .. Text)
end)[/align]
[align=center]Folder.Slider("Slider", {Precise = true, Default = 18, Min = 10, Max = 125}, function(Status)
print("Slider Triggered" .. tostring(Status))
end)
Tab1.Folder("Lipsum Expanded", "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur eu mollis urna, quis feugiat tellus. Integer ut ligula sodales, sodales ipsum ut, imperdiet ipsum. In aliquet quam et venenatis pulvinar. Nullam fermentum porta felis sit amet interdum. Sed tristique fringilla mollis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Nam quis tempus mauris, nec ultrices metus. Suspendisse mi urna, accumsan at nisi a, tristique porta libero. Integer lobortis elementum lacus cursus consectetur. Morbi mauris ante, posuere at malesuada et, tristique non ipsum. Proin vitae purus pretium, convallis est vitae, dignissim leo. Praesent nec felis vitae.")

local Cheat = Tab1.Cheat("Options", "A bunch of options you can use", function(Status)
print("Cheat Triggered: " .. tostring(Status))
end)
Cheat.Button("Button", "Click", function()
print("Button Clicked")
end)
Cheat.Switch("Switch", function(Status)
print("Switch Triggered: " .. tostring(Status))
end)
Cheat.Toggle("Toggle", function(Status)
print("Toggle Triggered: " .. tostring(Status))
end)
Cheat.Toggle("Toggle", function(Status)
print("Toggle Triggered: " .. tostring(Status))
end)
Cheat.TextBox("Textbox", "Placeholder", function(Text)
print("TextBox Triggered: " .. Text)
end)

Tab1.Cheat("Lipsum Expanded", "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur eu mollis urna, quis feugiat tellus. Integer ut ligula sodales, sodales ipsum ut, imperdiet ipsum. In aliquet quam et venenatis pulvinar. Nullam fermentum porta felis sit amet interdum. Sed tristique fringilla mollis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Nam quis tempus mauris, nec ultrices metus. Suspendisse mi urna, accumsan at nisi a, tristique porta libero. Integer lobortis elementum lacus cursus consectetur. Morbi mauris ante, posuere at malesuada et, tristique non ipsum. Proin vitae purus pretium, convallis est vitae, dignissim leo. Praesent nec felis vitae.", function(Status)
print("Cheat Triggered: " .. tostring(Status))
end)

-- Tab 2 --
local Tab2 = Window.Tab("Tab 2", 6022668945)
local Folder = Tab2.Folder("Options", "A bunch of options you can use")
Folder.Button("Button", "Click", function()
print("Button Clicked")
end)
Folder.Switch("Switch", function(Status)
print("Switch Triggered: " .. tostring(Status))
end)
Folder.Toggle("Toggle", function(Status)
print("Toggle Triggered: " .. tostring(Status))
end)
Folder.Toggle("Toggle", function(Status)
print("Toggle Triggered: " .. tostring(Status))
end)
Folder.TextBox("Textbox", "Placeholder", function(Text)
print("TextBox Triggered: " .. Text)
end)
Tab2.Folder("Lipsum Expanded", "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur eu mollis urna, quis feugiat tellus. Integer ut ligula sodales, sodales ipsum ut, imperdiet ipsum. In aliquet quam et venenatis pulvinar. Nullam fermentum porta felis sit amet interdum. Sed tristique fringilla mollis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Nam quis tempus mauris, nec ultrices metus. Suspendisse mi urna, accumsan at nisi a, tristique porta libero. Integer lobortis elementum lacus cursus consectetur. Morbi mauris ante, posuere at malesuada et, tristique non ipsum. Proin vitae purus pretium, convallis est vitae, dignissim leo. Praesent nec felis vitae.")

local Cheat = Tab2.Cheat("Options", "A bunch of options you can use", function(Status)
print("Cheat Triggered: " .. tostring(Status))
end)
Cheat.Button("Button", "Click" function()
print("Button Clicked")
end)
Cheat.Switch("Switch", function(Status)
print("Switch Triggered: " .. tostring(Status))
end)
Cheat.Toggle("Toggle", function(Status)
print("Toggle Triggered: " .. tostring(Status))
end)
Cheat.Toggle("Toggle", function(Status)
print("Toggle Triggered: " .. tostring(Status))
end)
Cheat.TextBox("Textbox", "Placeholder", function(Text)
print("TextBox Triggered: " .. Text)
end)

Tab2.Cheat("Lipsum Expanded", "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Curabitur eu mollis urna, quis feugiat tellus. Integer ut ligula sodales, sodales ipsum ut, imperdiet ipsum. In aliquet quam et venenatis pulvinar. Nullam fermentum porta felis sit amet interdum. Sed tristique fringilla mollis. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Nam quis tempus mauris, nec ultrices metus. Suspendisse mi urna, accumsan at nisi a, tristique porta libero. Integer lobortis elementum lacus cursus consectetur. Morbi mauris ante, posuere at malesuada et, tristique non ipsum. Proin vitae purus pretium, convallis est vitae, dignissim leo. Praesent nec felis vitae.", function(Status)
print("Cheat Triggered: " .. tostring(Status))
end)

game:GetService("UserInputService").InputBegan:Connect(function(Input)
if Input.KeyCode == Enum.KeyCode.F then
Window:Toggle()
end
end)
```