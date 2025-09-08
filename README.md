# Zen-Zest-UILibrary
My Second Ever Published UI Library. I Hope You Like It!

## Credits.

Solo Dev, TheLostStar7.

## Change Log.

Future:

Adding A DownDrop.

## Loadstring.
```lua
local ZenZest = loadstring(game:HttpGet(('https://raw.githubusercontent.com/TheLostStar7/Zen-Zest-UILibrary/refs/heads/main/ZenZestLib')))()
--[[
Loads The UI Library/UI Lib
]]
```

### Destroy.
```lua
ZenZest:Destroy()
--[[
Destroys The UI Lib
]]
```

### Visible.
```lua
ZenZest:Visible()
--[[
This Would Turn It On And Off But Adding A Argument[1] true Or false To Turn It On And Off.
]]
```

### KeyBind.
```lua
ZenZest:SetKeybind("K")
--[[
Argument[1] = <string> - New
 KeyBind To Close The UI With.
]]
```

```lua
ZenZest:GetKeybind()
--[[
Returns The Keybind.
]]
```

### Init.
```lua
local ok,msg = ZenZest:Init()
print(ok,msg)
--[[
Init Waits For The Things Such As The Icons To Load Before Showing The UILibrary.
]]
```

## Window.
```lua
local win = ZenZest:CreateWindow({
    Title = "Zen Zest UI Library | "..game.Players.LocalPlayer.Name,
    Settings = {
        Minimize_Settings = {
            Keybind = "Z"
        },
        Theme_Settings = {
            Theme = "bloom"  -- Themes: "Bloom", "Red", "Orange".
        }
    }
})
--[[
Title = <string> - The Name Of The UI.
KeyBind = <string> - The Keybind To Close/Open The UI.
Theme = <string> - The Theme Of The Objects Inside The UI.
]]
```

## Tab.
```lua
local Tab = win:AddTab({Title = "Main Tab"})
--[[
Title = <string> - The Name Of The Tab.
]]
```

## Group.
```lua
local Group = Tab:AddGroup({Title = "Hello"})
--[[
Title = <string> - The Name Of The Group. Could Also Be Used Like: ("Hello") or () which defaults to Group.
]]
```

## Button.
```lua
local Button = Group:AddButton({Title = "Hello",Flag = "Hello Button",Callback = function()
    print("sup g")
end,})
--[[
Title = <string> - The Name Of The Button.
Flag = <string> - The Name Of The Flag Report.
Callback = <function> - The Function Of The Button.
]
```

## Toggle.
```lua
local Toggle = Group:AddToggle({Title = "YO",Flag = "Hello Togglers Gooners",Callback = function(v)
    print("Toggle:",v)
end,})
--[[
Title = <string> - The Name Of The Toggle.
Flag = <string> - The Name Of The Flag Report.
Callback = <function> - The Function Of The Toggle.
]]
```

## Slider.
```lua
local Slider = Group:AddSlider({Title = "WalkSpeed",Flag = "Slider",Callback = function(v)
  print(v)
end,
  Min = 16,
  Max = 500,
  Default = 150
})
--[[
Title = <string> - The Name Of The Slider.
Flag = <string> - The Name Of The Flag Report.
Callback = <function> - The Function Of The Slider.
Also You Could Use Min And Max And Default In The Top Behind The Callback.
]]
```
### Slider Subtitle Functions.
```lua
Slider:GetValue()
--[[
Returns The Value / Amount.
]]
```
```lua
Slider:SetValue(50)
--[[
Sets The Value / Amount.
]]
```

## Label.
```lua
local Text = Group:AddLabel({Text = "Yappers"})
--[[
Text = <string> - The Text Of Label. Could Also Be Used Like: ("Hello") or () which defaults to Label.
]]
```
### Label Subtitle Functions.
```lua
Text:Update("Hello")
--[[
Argument[1] = <string> - The New Text Of The Label.
]]
```
```lua
Text:Get()
--[[
Gives You The Current Text.
]]
```

## Input.
```lua
local Input = Group:AddInput({Title = "Printer",Callback = function(v)
    print(v)
end,})
--[[
Title = <string> - The Name Of The Input.
Callback = <function> - The Function Of The Input.
Both Could Be Used Like:
local Input = Group:AddInput("Printer",function(v)
    print(v)
end,)
]]
```
### Input Subtitle Functions.
```lua
Input:GetText()
--[[
Returns The Text Of The Input From The Variable Of The AddInput.
]]
```
```lua
Input:SetText("Hello")
--[[
Argument[1] = <string> - Inputs The Text You Put In.
]]
```
