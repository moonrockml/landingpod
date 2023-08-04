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

# Window Elements
Tab/SectionTabs
## Creating a Tab
```lua
local tab1 = Library:CreateTab("reee")
```
## Creating a SectionTab
```lua
local sectiontab = Library:CreateTabSection("Section1")
sectiontab.CreateSectionTab("SectionButton")
sectiontab.CreateSectionTab("SectionButton")
sectiontab.CreateSectionTab("SectionButton")
sectiontab.CreateSectionTab("SectionButton")
```
