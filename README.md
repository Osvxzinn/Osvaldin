-- Carregar Script
local Fluent = loadstring(game:HttpGet("https://github.com/dawid-scripts/Fluent/releases/latest/download/main.lua"))()

local Window = Fluent:CreateWindow({
    Title = "Osvaldin Menu " .. Fluent.Version,
    TabWidth = 160, Size = UDim2.fromOffset(580, 460), Theme = "Dark"
})

local Tabs = {
    Main = Window:AddTab({ Title = "Main" }),
    Settings = Window:AddTab({ Title = "Settings", Icon = "settings" })
}
--Paragrafos
Tabs.Main:AddParagraph({ Title = "Osvaldin", Content = "This is a paragraph.\nSecond line!" })

--Botoes
Tabs.Main:AddButton({ Title = "AutoFarm", Callback = function() loadstring(jogo:HttpGet("https://raw.githubusercontent.com/StormSKz12/StirkeHub1/main/Gameincluded"))() end })
Tabs.Main:AddButton({ Title = "Teleport", Callback = function() loadstring(jogo:HttpGet("https://raw.githubusercontent.com/Kaizenofficiall/ZenHub/main/Loader", true))() end })
