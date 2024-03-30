# MyUILib (Unamed) UI
This documentation is for MyUILib (Unamed) UI Credit To The Owner

## Booting the MyUILib (Unamed) UI Library
```lua
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/Vcsk/UI-Library/main/Source/MyUILib(Unamed).lua"))()
```




## Creating a MyUILib (Unamed) UI Window
```lua
local Window = Library:Create("Example") -- any name
```

## Creating a Tab
```lua
local Tab1 = Window:Tab("Tab 1","rbxassetid://10888331510")
```

## Creating a Tab 2
```lua
local Tab2 = Window:Tab("Players","rbxassetid://12296135476")
```

## Creating a Warning Label
```lua
Tab1:WarningLabel("This is a warning")
```

## Creating a Info Label
```lua
Tab1:InfoLabel("This is a info")
```

## Creating a Label
```lua
Tab1:Label("This is a label")
```

## Creating a Button
```lua
Tab1:Button("Button 1", function() -- button
	print("Pressed Button 1!")
end)
```

## Creating a Toggle
```lua
Tab1:Toggle("Toggle 1", function(state) -- toggle
	print(state)
end)
```

## Creating a Slider
```lua
Tab1:Slider("Slider 1", 1,100, function(value) -- slider | min,max
	print(value)
end)
```

## Creating a Destroy UI
```lua
Tab1:Button("Destroy UI", function()
	Library:DestroyUI()
end)
```

## Creating a Walkspeed (Slider) (Optional)
```lua
Tab2:Slider("WalkSpeed", 16,500, function(value)
	game:GetService("Players").LocalPlayer.Character.Humanoid.WalkSpeed = value
end)
```

## Creating a JumpPower (Slider) (Optional)
```lua
Tab2:Slider("JumpPower", 50,1000, function(value)
	game:GetService("Players").LocalPlayer.Character.Humanoid.JumpPower = value
end)
```
