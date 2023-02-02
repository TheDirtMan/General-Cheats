--Setup
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()

--Base
local Window = Library.CreateLib("General Cheats", "Ocean")

--Tabs
local PlayerMods = Window:NewTab("Player Mods")
local Fun = Window:NewTab("Fun")

--Sections
local SpeedM = PlayerMods:NewSection("Speed")
local JumpM = PlayerMods:NewSection("Jump Height")

--Speed
local SpeedOn = false
local Speed = 16

SpeedM:NewToggle("Speed Mod", "If The Players Speed Should Be Changed", function(state)
    if state then
        SpeedOn = true
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Speed
    else
        SpeedOn = false
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 16
    end
end)
SpeedM:NewSlider("Speed", "What The Players Speed Should Be", 500, 1, function(speed)
    if SpeedOn then
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = speed
        Speed = speed
    else
        game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 16
    end
end)

--Jump
local JumpOn = false
local Jump = 50

JumpM:NewToggle("Jump Mod", "If The Players Jump Height Should Be Changed", function(state)
    if state then
        JumpOn = true
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = Jump
    else
        JumpOn = false
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = 50
    end
end)
JumpM:NewSlider("Jump Height", "What The Players Jump Height Should Be", 2000, 1, function(jump)
    if JumpOn then
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = jump
        Jump = jump
    else
        game.Players.LocalPlayer.Character.Humanoid.JumpPower = 50
    end
end)

--Force Sit
local ForceSit = Fun:NewSection("Force Sit")
ForceSit:NewButton("Force Sit", "Force The Player Into Sitting", function()
    game.Players.LocalPlayer.Character.Humanoid.Sit = true
end)

--Suicide
local Suicide = Fun:NewSection("Suicide")
Suicide:NewButton("Suicide", "Die Instantly", function()
    game.Players.LocalPlayer.Character.Humanoid.Health = 0
end)
