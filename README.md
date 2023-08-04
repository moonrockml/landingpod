[![landingpod](ImageAssets/MoonRockLogo_D.png)](https://discord.gg/rXbGpfuKmV)

## Features Like No Other
- Custom Optional Loading popup
- Unique Design, Mixed with csgo and a modern styled ui
- Tab Button Sections
- built-in Settings Tab
- And More To Come
  
<br/>


### Initializing The Library (Coming Very Soon)
```lua
local Library = loadstring(game:HttpGet("comingsoon.lua"))()
```

### Loading Popup (optional)
```lua
Library.load.CreateLoader({
    Title = "MoonRock",
    Thumbnail = "35500340", -- only ID
    Discord = {
        Invite = "rXbGpfuKmV" -- only invite code is needed
    },
    ConfigSaving = {
        Enabled = true,
        FolderTitle = "MoonRockConfigs",
        FileTitle = "MyConfigFile"
    }
})
```

### Creating Window
```lua
Library:CreateWindow({
    Title = "MoonRock │ https://discord.gg/rXbGpfuKmV │ Be Cool",
    Discord = {
        Invite = "rXbGpfuKmV" -- only invite code is needed
    },
    ConfigSaving = {
        Enabled = true,
        FolderTitle = "MoonRockConfigs",
        FileTitle = "MyConfigFile"
    }
})
```
<br/>

# Window Elements ᭼
Tabs / SectionTabs

## Creating a Tab
```lua
local Tab = Library:CreateTab("reee")
```
## Creating a SectionTab
```lua
local sectiontab = Library:CreateTabSection("Section1")
sectiontab.CreateSectionTab("SectionButton")
sectiontab.CreateSectionTab("SectionButton")
sectiontab.CreateSectionTab("SectionButton")
sectiontab.CreateSectionTab("SectionButton")
```
## Creating groupbox (Required For Tab Elements To Work)
```lua
local GroupBox = Tab:CreateGroupBox({Title = "Donuts",Side = "Left"})
```
<br/>

# Tab Elements ᭼
## Creating a button
```lua
GroupBox:CreateButton({
	Title = "Button",
	Callback = function()
		print("hello world")
	end,
})
```

## Creating a Toggle
```lua
GroupBox:CreateToggle({
	Title = "Toggle",
	Callback = function(v)
		print(v)
	end,
})
```
## Creating a Keybind
```lua
GroupBox:CreateKeybind({
	Title = "KeyBind",
	Bind = nil, -- Starting Key ex.("Q")
	Callback = function()
		print("Hello World")
	end,
})
```
## Creating a Slider
```lua
GroupBox:CreateSlider({
	Title = "Slider",
	Range = {0, 500}, -- Minimum and maximum values of the slider
	StartValue = 50,
	Increment = 5,    -- Increment value for each step
	Callback = function(newValue)
		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = newValue
		print(newValue)
	end
})
```

## Creating a DropDown
```lua
GroupBox:CreateDropdown({
	Title = "Dropdown",
	Options = {"option1", "option2"}, 
	MultipleOptions = true,
	Callback = function(option)
		print("Selected option:", option)
	end,
})
```

## Creating a ColorPicker
```lua
GroupBox:CreateColorPicker({
	Name = "ColorPicker",
	Color = Color3.fromRGB(150, 129, 255),
	Callback = function(Value)
		print(Value)
	end
})
```
