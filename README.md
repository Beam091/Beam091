
if game:GetService("CoreGui"):FindFirstChild("BlackTrap") then
    game:GetService("CoreGui")["BlackTrap"]:Destroy()
end

-- Color -- 
_G.WindowBackgroundColor = Color3.fromRGB(12,12,12)
_G.BackgroundItemColor = Color3.fromRGB(20, 20, 20)
_G.TabWindowColor = Color3.fromRGB(30, 30, 30)
_G.ContainerColor = Color3.fromRGB(30, 30, 30)
_G.TitleTextColor = Color3.fromRGB(150, 150, 150)
_G.ImageColor = Color3.fromRGB(150, 150, 150)
_G.LineThemeColor = Color3.fromRGB(150, 150, 150)
_G.TabTextColor = Color3.fromRGB(150, 150, 150)
_G.TabImageColor = Color3.fromRGB(150, 150, 150)
_G.TabThemeColor = Color3.fromRGB(250, 0, 0)
_G.SectionColor = Color3.fromRGB(150, 150, 150)
_G.SectionImageColor = Color3.fromRGB(150, 150, 150)
_G.SectionTextColor = Color3.fromRGB(150, 150, 150)
_G.SectionOn = Color3.fromRGB(0, 250, 0)

-- Link Blacklib --
local Blacklib = loadstring(game:HttpGet('https://raw.githubusercontent.com/kickTh/New-Ui/main/BlackTrap_Gui_V1.3.txt'))()
-- Blacklib Window --
local Win = Blacklib:Window("Gui")
-- Tabes --
local Main = Win:Tab("โ€ข Main", "rbxassetid://8825667942")
local Home = Win:Tab("โ€ข Home", nil)
local Game = Win:Tab("โ€ข Game", nil)
-- Section --
local Main_1 = Main:NewSection("")
local Home_1 = Home:NewSection("")
local Game_1 = Game:NewSection("")

-- function Main --

Main_1:Line()
Main_1:Label("Label")


Main_1:Button("Button", function()
end)


Main_1:Toggle("Toggle", function()
end)
Main_1:TextBox("Text Box", "Enter", function()
end)

Main_1:Slider("Slider",0,500,50, function(tl)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = t
end)


local DropdownTXT = {
      "1";
      "2";
      "3";
      "4";
      "5";
}
local TestDropdown = Main_1:Dropdown("Testing",DropdownTXT, function(value)
    _G.Dropdown = value
end)

Main_1:Button("Clear Dropdown", function()
    TestDropdown:Clear()
end)


Main_1:Button("Notification", function()
    Blacklib:Notification("Notification")
end)


-- function Home --

Home_1:Line()

Home_1:Label("Label")


Home_1:Button("Button", function()
end)


Home_1:Toggle("Toggle", function()
end)

Home_1:TextBox("Text Box", "Enter Value", function()
end)

Home_1:Slider("Slider",0,500,50, function(tl)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = t
end)

local Lizet = {
      "1";
      "2";
      "3";
      "4";
      "5";
}
local TestDropdown = Home_1:Dropdown("Testing", Lizet, function(value)
    _G.Vasted = value
end)

Home_1:Button("Clear Dropdown", function()
    TestDropdown:Clear()
end)


Home_1:Button("Notification", function()
    Blacklib:Notification("Notification")
end)
