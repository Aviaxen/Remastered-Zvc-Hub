local Rayfield = loadstring(game:HttpGet("https://sirius.menu/gen2"))()

local window = Rayfield:CreateWindow({
    name = "Zvc Hub Remastered",
    subtitle = "Remastered By Inky",
    theme = "cobalt",
    configuration = {
        autoSave = true,
        autoLoad = true,
        fileName = "Zvc Hub Remastered",
    },
})

-- FIXED: Restored Gen2 style configuration tables
local homeTab = window:CreateTab({ name = "Home", icon = 93364949241311 })

-- FIXED: Added proper Gen2 configuration table syntax for consistency
homeTab:CreateSection({ Name = "Featured" })

homeTab:CreateButton({
    name = "Infinite Yield",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/edgeiy/infiniteyield/master/source"))()
    end,
})

homeTab:CreateButton({
    name = "Nameless Admin",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/ltseverydayyou/Nameless-Admin/main/Source.lua"))()
    end,
})

homeTab:CreateButton({
    name = "Dex Explorer",
    callback = function()
        loadstring(game:HttpGet("https://github.com/AZYsGithub/DexPlusPlus/releases/latest/download/out.lua"))()
    end,
})

homeTab:CreateButton({
    name = "Remote Spy",
    callback = function()
        loadstring(game:HttpGet("https://github.com/exxtremestuffs/SimpleSpySource/raw/master/SimpleSpy.lua"))()
    end,
})


-- FIXED: Changed 'tab' to 'homeTab' to fix the indexing crash
homeTab:CreateSlider({
    name = "Walkspeed",
    range = { 20, 150 },
    increment = 1,
    value = 16, -- 16 is the default Roblox walkspeed
    suffix = " studs",
    callback = function(value)
        local player = game:GetService("Players").LocalPlayer
        if player and player.Character and player.Character:FindFirstChildOfClass("Humanoid") then
            player.Character:FindFirstChildOfClass("Humanoid").WalkSpeed = value
        end
    end,
})

-- FIXED: Restored Gen2 style configuration tables
local hubsTab = window:CreateTab({ name = "Hubs", icon = 93364949241311 })

-- FIXED: Changed string parameter to proper Gen2 table dictionary layout
hubsTab:CreateSection({ Name = "Universal" })

hubsTab:CreateButton({
    name = "Xvc Hub",
    callback = function()
        loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-XVC-Hub-202396"))()
    end,
})

hubsTab:CreateButton({
    name = "Dfxclan Hub",
    callback = function()
        loadstring(game:HttpGet("https://pastebin.com/raw/HK1Xpajw"))()
    end,
})

hubsTab:CreateButton({
    name = "Degent Hub",
    callback = function()
        loadstring(game:HttpGet("https://pastebin.com/raw/cr20JxP9"))()
    end,
})

hubsTab:CreateButton({
    name = "Zvc Hub (Old)",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/Aviaxen/Zvc-Hub/refs/heads/main/README.md"))()
    end,
})

hubsTab:CreateButton({
    name = "Galactic Hub",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/GalacticScripts/Galactic-Hub/refs/heads/main/WindUI"))()
    end,
})

hubsTab:CreateButton({
    name = "Yunus Hub",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/yunus154524/YunusLo1545-HUB/refs/heads/main/YunusLo1545%20HUB"))()
    end,
})

hubsTab:CreateButton({
    name = "Opiam Hub",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/HydraRBXM/opiamhub/refs/heads/main/OpiamMain"))()
    end,
})

hubsTab:CreateButton({
    name = "Altair Hub",
    callback = function()
        loadstring(game:HttpGet("https://pastefy.app/hiwjpLFi/raw"))()
    end,
})

hubsTab:CreateButton({
    name = "Trolling Hub",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/yofriendfromschool1/Sky-Hub/main/FE%20Trolling%20GUI.luau"))()
    end,
})

hubsTab:CreateButton({
    name = "Universal Script Searcher",
    callback = function()
        loadstring(game:HttpGet("http://scripthub.ultimatex.store"))()
    end,
})

local scriptsTab = window:CreateTab({ name = "Scripts", icon = 93364949241311 })

-- FIXED: Changed string parameter to proper Gen2 table dictionary layout
scriptsTab:CreateSection({ Name = "Gui" })

scriptsTab:CreateButton({
    name = "Coolkid Gui V1",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/cfsmi2/c00lguiv1/refs/heads/main/Main.lua"))()
    end,
})

scriptsTab:CreateButton({
    name = "Coolkid Gui V2",
    callback = function()
        loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-c00lgui-134417"))()
    end,
})

scriptsTab:CreateButton({
    name = "Coolkid Gui V3",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/MiRw3b/c00lgui-v3rx/main/c00lguiv3rx.lua"))()
    end,
})

scriptsTab:CreateButton({
    name = "Coolkid Gui V4",
    callback = function()
        loadstring(game:HttpGet("https://rawscripts.net/raw/Natural-Disaster-Survival-c00lkidds-op-trolling-gui-of-nds-30335"))()
    end,
})

local toolsTab = window:CreateTab({ name = "Tools", icon = 93364949241311 })

toolsTab:CreateSection({ Name = "Tools" })

toolsTab:CreateButton({
    name = "Youtube Music Player",
    callback = function()
        loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-YouTube-Music-Player-V8-236600"))()
    end,
})

toolsTab:CreateButton({
    name = "Pshade (Shaders)",
    callback = function()
        loadstring(game:HttpGet('https://raw.githubusercontent.com/randomstring0/pshade-ultimate/refs/heads/main/src/cd.lua'))()
    end,
})

toolsTab:CreateButton({
    name = "Shiftlock",
    callback = function()
        loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-Universal-Shiftlock-No-Disappear-after-die-23318"))()
    end,
})

toolsTab:CreateButton({
    name = "Fly 1",
    callback = function()
        loadstring(game:HttpGet("https://pastefy.app/9bilwWLP/raw"))()
    end,
})

toolsTab:CreateButton({
    name = "Fly 2",
    callback = function()
        loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-Fly-script-v3-16742"))()
    end,
})

local trollingTab = window:CreateTab({ name = "Trolling", icon = 93364949241311 })

trollingTab:CreateSection({ Name = "Trolling" })

trollingTab:CreateButton({
    name = "Grab Npcs",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/GUI-Offical/FileTest/refs/heads/main/Grab%20R6.txt", true))()
    end,
})

trollingTab:CreateButton({
    name = "Dropkick Fling",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/platinww/CrustyMain/refs/heads/main/universal/DropKick.lua"))()
    end,
})

trollingTab:CreateButton({
    name = "Fling Gui 1",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/sypcerr/scripts/refs/heads/main/UFGUI", true))()
    end,
})

local fescriptsTab = window:CreateTab({ name = "Fe Scripts", icon = 93364949241311 })

fescriptsTab:CreateSection({ Name = "Animation" })

fescriptsTab:CreateButton({
    name = "R15 Emotes",
    callback = function()
        loadstring(game:HttpGet("https://luascript-on.vercel.app/raw/0ea85807-4441-4bcd-a469-55481b6fe5b5"))()
    end,
})

fescriptsTab:CreateButton({
    name = "R6 Animations",
    callback = function()
        loadstring(game:HttpGet("https://pastefy.app/UC2OHMhe/raw"))()
    end,
})

local funTab = window:CreateTab({ name = "Fun", icon = 93364949241311 })

funTab:CreateSection({ Name = "Fun" })

funTab:CreateButton({
    name = "Verity V1",
    callback = function()
        loadstring(game:HttpGet("https://pastebin.com/raw/pQjRMdiG"))()
    end,
})

funTab:CreateButton({
    name = "Welding Abuse",
    callback = function()
        loadstring(game:HttpGet("https://raw.githubusercontent.com/rangell8/Rexys-Welding-Hub/refs/heads/main/script"))()
    end,
})


