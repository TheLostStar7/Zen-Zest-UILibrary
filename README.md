# Zen-Zest-UILibrary
My Second Ever Published UI Library. I Hope You Like It!

## Credits.

Solo Dev, TheLostStar7.

## Change Log.

Future:

Adding A DownDrop.

## Information: I'M TOO LAZY TO ADD EVERYTHING, PLEASE READ THE SOURCE FOR MORE FLEXIBILITY OR CUSTOMIZATIONS

## Usage.
```lua
local ZenZest = loadstring(game:HttpGet(('https://raw.githubusercontent.com/TheLostStar7/Zen-Zest-UILibrary/refs/heads/main/ZenZestLib')))()

ZenZest:Init()

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

local Tab = win:AddTab({Title = "Main Tab"})

local Group = Tab:AddGroup({Title = "Hello"})

local Button = Group:AddButton({Title = "Hello",Flag = "Hello Button",Callback = function()
    print("Yo Yo Yo Yo.")
end,})

local Toggle = Group:AddToggle({Title = "Gooning",Flag = "Hello Togglers Gooners",Callback = function(v)
    print("Toggle:",v)
end,})

local Slider = Group:AddSlider({Title = "WalkSpeed",Flag = "Slider",Callback = function(v)
  print(v)
end,
  Min = 16,
  Max = 500,
  Default = 150
})

local Text = Group:AddLabel({Title = "Yappers"})

local Input = Group:AddInput({Title = "Printer",Callback = function(v)
    print(v)
end,})
```
