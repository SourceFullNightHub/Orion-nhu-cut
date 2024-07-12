# Sourceg
```
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/SourceFullNightHub/Orion-nhu-cut/main/W-azureLib"))()
```

# Create Windows
```
local Window = Library:Start({
	["Name"] = "Sitink Hub",
	["Logo Player"] = "rbxassetid://18448428761",
	["Name Player"] = "@Nightx12082k11",
	["Tab Width"] = 120,
	["Color"] = Color3.fromRGB(6.000000117346644, 141.0000067949295, 234.00000125169754),
	["Custom Toggle"] = false,
	["CloseCallBack"] = function()
		Library:Notify({
			["Title"] = "Sitink Hub",
			["Content"] = "Closed UI!",
			["Logo"] = "rbxassetid://18374900760",
			["Time"] = 0.5,
			["Delay"] = 5
		})
	end
})
```

# Create Tab
```
local MainTab = Window:MakeTab("Tab")
```

# Notify
```
Library:Notify({
    ["Title"] = "Alert",
    ["Content"] = "Loaded UI!",
    ["Logo"] = "rbxassetid://18289959127",
    ["Time"] = 0.5,
    ["Delay"] = 5
})
```

# Section
```
local Section = MainTab:Seperator("Section")
```
# Create Button
```
MainTab:Button({
	["Title"] = "Button",
	["Content"] = "This is a button",
	["Logo"] = "rbxassetid://18271082015",
	["Callback"] = function()
		print("Button Clicked!")
	end
})
```
# Toggle 

```
local Toggle = MainTab:Toggle({
	["Title"]= "Toggle",
	["Content"] = "This is a Toggle",
	["Default"] = false,
	["Callback"] = function(Value) 
		print(Value)
	end
})
```

# Settings Toggle
```lua
local ToggleSetting = Toggle:AddSetting()
local SettingToggle = ToggleSetting:Toggle({
	["Name"] = "Toggle",
	["Default"] = false,
	["Callback"] = function(Value)
		print(Value)
	end
})

local SliderSetting = ToggleSetting:Slider({
	["Name"] = "Slider",
	["Min"] = 0,
	["Max"] = 100,
	["Increment"] = 1,
	["Default"] = 30,
	["Callback"] = function(Value)
		print(Value)
	end
})
```
#Create Slider

```
local Slider = MainTab:Slider({
	["Title"] = "Slider",
	["Content"] = "This is a Slider",
	["Min"] = 0,
	["Max"] = 100,
	["Increment"] = 1,
	["Default"] = 30,
	["Callback"] = function(Value) 
		print(Value)
	end
})
```

# Create Dropdown
```
local Dropdown = MainTab:Dropdown({
	["Title"] = "Dropdown",
	["Content"] = "This is a dropdown",
	["Multi"] = false,
	["Options"] = {"Option 1", "Option 2"},
	["Default"] = {"Option 1"},
	["Callback"] = function(Value)
		print(Value)
	end
})
```
# Multi Dropdown
```
local MultiDropdown = MainTab:Dropdown({
	["Title"] = "Multi Dropdown",
	["Content"] = "This is a multi dropdown",
	["Multi"] = true,
	["Options"] = {"Option 1", "Option 2"},
	["Default"] = {"Option 1"},
	["Callback"] = function(Value)
		print(Value)
	end
})
```
# Textbox
```
local TextInput = MainTab:TextInput({
	["Title"] = "Webhook",
	["Content"] = "Enter your webhook here",
	["Callback"] = function(Value)
		print(Value)
	end
})
```
