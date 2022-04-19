local VLib = loadstring(game:HttpGet("https://raw.githubusercontent.com/vep1032/VepStuff/main/VL"))()

game.StarterGui:SetCore("ChatMakeSystemMessage", {
Text = "script built by nar";
Color = Color3.new(255, 0, 0);
Font = Enum.Font.SourceSansBold;
FontSize = Enum.FontSize.Size24;
})
 
local s = VLib:Window("Random Gui", "By nar", "emo")
 
local ss = s:Tab("Main")

ss:Button("Fly - C To Fly",function()
    loadstring(game:HttpGet('https://raw.githubusercontent.com/W9K/roblox-scripts/main/DHC/Fly.lua'))()
end)

ss:Button("Anti Slow",function()
    loadstring(game:HttpGet('https://pastebin.com/raw/3DQVwKfk'))()
end)

ss:Button("Infinite Jump",function()
    loadstring(game:HttpGet('https://pastebin.com/raw/KBjXt9rW'))()
end)

ss:Button("Big Head (RTHRO HEAD AND R15 REQUIRED)",function()
    loadstring(game:HttpGet('https://pastebin.com/raw/vahidDqX'))()
end)

ss:Button("Anti Stomp",function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/BlueaqeR/scripts-lol/main/Da%20Hood%20Anti%20Stomp%20(Optimized)"))()
end)

ss:Button("Lock (Q)",function()
    loadstring(game:HttpGet('https://pastebin.com/raw/JcfqHEUz'))()
end)

ss:Button("God Mode",function()
    loadstring(game:HttpGet('https://pastebin.com/raw/fqAMYD8x'))()
end)

ss:Button("No Textures (Gives More FPS)",function()
    loadstring(game:HttpGet('https://pastebin.com/raw/XG1Rep1S'))()
end)

ss:Button("Korblox (NOT FE, PREFERED SKINNY)",function()
    loadstring(game:HttpGet('https://pastebin.com/raw/wYfvrD4C'))()
end)

ss:Button("Headless (NOT FE)",function()
    loadstring(game:HttpGet('https://pastebin.com/raw/4wESFR1h'))()
end)

ss:Button("Animation Changer",function()
    loadstring(game:HttpGet('https://pastebin.com/raw/ZSEJM0yx'))()
end)

ss:Button("Anti AFK",function()
    local vu = game:GetService("VirtualUser")
    game:GetService("Players").LocalPlayer.Idled:connect(function()
       vu:Button2Down(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
       wait(1)
       vu:Button2Up(Vector2.new(0,0),workspace.CurrentCamera.CFrame)
    end)
end)

local ss = s:Tab("Player")

ss:Slider("JumpPower",0,500,50,function(t)
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = t
 end)

ss:Slider("WalkSpeed",0,500,16,function(t)
   game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = t
end)
 
ss:Button("Reset Walk and Jump to Normal",function()
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = 16
    game.Players.LocalPlayer.Character.Humanoid.JumpPower = 50
end)

local ss = s:Tab("Quick Teleport")

ss:Button("Admin Base",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-799.420227, -39.6492119, -886.431885, 0.00734946132, -2.7381879e-09, -0.999972999, -1.96182803e-09, 1, -2.75268053e-09, 0.999972999, 1.98200567e-09, 0.00734946132)
end)

ss:Button("Gunshop #1 (Shotgun)",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-583.550232, 8.31477833, -736.083374, 0.0155641753, -4.13069259e-08, -0.999878883, -7.5154194e-09, 1, -4.14289154e-08, 0.999878883, 8.15931589e-09, 0.0155641753)
end)

ss:Button("Gunshop #2 (Tactical Shotgun)",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(481.967377, 48.0704918, -622.48291, -0.999142826, -4.59601779e-08, 0.0413958244, -4.61406842e-08, 1, -3.40509154e-09, -0.0413958244, -5.31220445e-09, -0.999142826)
end)

ss:Button("Bank",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-477.527405, 39.0876045, -284.432373, -0.00350706372, -3.32849872e-08, -0.999993861, -7.88508281e-09, 1, -3.32575389e-08, 0.999993861, 7.76839837e-09, -0.00350706372)
end)

ss:Button("Bank Food Store",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-333.274323, 23.682642, -298.435089, -0.0198831819, -1.02589631e-07, 0.999802291, -1.77884569e-08, 1, 1.02256152e-07, -0.999802291, -1.57517626e-08, -0.0198831819)
end)

ss:Button("Uphill Food Store",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(299.039032, 49.2826538, -619.744263, -0.999999464, -8.79183781e-10, -0.00103831524, -8.80863049e-10, 1, 1.61680691e-09, 0.00103831524, 1.61772074e-09, -0.999999464)
end)

ss:Button("Taco Shop",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(599.604675, 51.0576744, -452.68927, 0.999841511, -9.64418803e-08, -0.0178023502, 9.62277511e-08, 1, -1.28847581e-08, 0.0178023502, 1.11696359e-08, 0.999841511)
end)

ss:Button("Sewers",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(112.620247, -26.7500305, -277.320007, -0.999657452, 9.20699179e-08, -0.0261730645, 9.20406578e-08, 1, 2.32255393e-09, 0.0261730645, -8.72278014e-11, -0.999657452)
end)

ss:Button("Park",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(282.175751, 63.9999962, -446.649902, 0.0261927843, 4.30053397e-08, -0.999656916, 5.02474435e-08, 1, 4.43366694e-08, 0.999656916, -5.13915062e-08, 0.0261927843)
end)

ss:Button("Playground",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-248.030945, 22.149868, -742.987671, 0.999907017, 2.19137632e-08, 0.0136352126, -2.15693259e-08, 1, -2.54079353e-08, -0.0136352126, 2.5111472e-08, 0.999907017)
end)

ss:Button("SkatePark",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-825.685974, 21.9998188, -549.29303, 1, -1.30498528e-08, -9.43054804e-15, 1.30498528e-08, 1, -7.78443088e-09, 9.53213355e-15, 7.78443088e-09, 1)
end)

ss:Button("Casino",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-861.637695, 21.7499943, -131.336044, 0.99980247, 1.81383459e-08, 0.0198747013, -1.87716722e-08, 1, 3.16794306e-08, -0.0198747013, -3.20462554e-08, 0.99980247)
end)

ss:Button("Therate / Film",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-1005.96436, 25.1000233, -128.196075, 0.999986827, -1.64551583e-09, -0.00512879482, 2.11179607e-09, 1, 9.09087561e-08, 0.00512879482, -9.09183981e-08, 0.999986827)
end)

ss:Button("Furniture",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-489.651825, 21.8498497, -75.8652725, 0.999662101, -6.73830485e-08, 0.0259939991, 6.66437145e-08, 1, 2.93089411e-08, -0.0259939991, -2.75667009e-08, 0.999662101)
end)

ss:Button("School",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-587.08429, 21.8749924, 286.612946, -0.999999583, 6.32880131e-08, -0.000904109795, 6.3226814e-08, 1, 6.77215652e-08, 0.000904109795, 6.76643737e-08, -0.999999583)
end)

ss:Button("Church",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(205, 21.7499943, -82, 1, -6.71148257e-08, 5.02749545e-15, 6.71148257e-08, 1, 6.87438799e-08, -9.64122886e-15, -6.87438799e-08, 1)
end)

ss:Button("Circus",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(142, 24.7549973, -988, 1, -6.78601575e-09, 6.93875567e-14, 6.78601575e-09, 1, 6.94779434e-09, -6.94347059e-14, -6.94779434e-09, 1)
end)

ss:Button("Key",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-271, 21.7499943, -247, 1, -5.42960663e-08, -3.31323248e-15, 5.42960663e-08, 1, 8.66604353e-08, -1.39208827e-15, -8.66604353e-08, 1)
end)

ss:Button("Safe Zone #1",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-871.34845, -42.154213, -1166.10889, -0.999804676, 1.83988575e-08, -0.0197644699, 1.79295707e-08, 1, 2.39211513e-08, 0.0197644699, 2.35621105e-08, -0.999804676)
end)

ss:Button("Safe Zone #2",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(196.024551, 38.2499886, 200014.953, -0.999352872, 6.44363851e-08, -0.0359703414, 6.33232204e-08, 1, 3.20858682e-08, 0.0359703414, 2.97873477e-08, -0.999352872)
end)

ss:Button("Safe Zone #3",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-117.270287, -58.7000618, 146.536087, 0.999873519, 6.40794418e-10, -0.0159031227, -6.5288791e-10, 1, -7.5525719e-10, 0.0159031227, 7.65544628e-10, 0.999873519)
end)

ss:Button("Ufo",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(67.3056641, 139, -690.603027, -0.897383451, -6.36553352e-08, -0.441251516, -5.02039015e-08, 1, -4.2160039e-08, 0.441251516, -1.56811719e-08, -0.897383451)
end)

ss:Button("Gas Station",function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(593.900024, 49.0000305, -258.109253, 0.00797744654, -5.46651719e-08, 0.999968171, 5.64564075e-08, 1, 5.42165175e-08, -0.999968171, 5.60221025e-08, 0.00797744654)
end)
