_G.auto = true
while _G.auto  do wait(4) 
	



	

local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.Out,0,false,0 ),
{CFrame = CFrame.new(1059.75586, 16.3627472, 1548.59851, -0.987375617, 1.39881342e-08, 0.158396393, 2.30001458e-08, 1, 5.50621735e-08, -0.158396393, 5.80101869e-08, -0.987375617)}):Play()

local args = {
    [1] = "StartQuest",
    [2] = "BanditQuest1",
    [3] = 1
}

game:GetService("ReplicatedStorage").Remotes.CommF_:InvokeServer(unpack(args))

local CombatFramework = require(game:GetService("Players").LocalPlayer.PlayerScripts.CombatFramework)
local Camera = require(game.ReplicatedStorage.Util.CameraShaker)
Camera:Stop()
coroutine.wrap(function()
    game:GetService("RunService").Stepped:Connect(function()
        if getupvalues(CombatFramework)[2]['activeController'].timeToNextAttack then
            getupvalues(CombatFramework)[2]['activeController'].timeToNextAttack = 0
            getupvalues(CombatFramework)[2]['activeController'].hitboxMagnitude = 25
            getupvalues(CombatFramework)[2]['activeController']:attack()
        end
    end)
end)()
Weapon = "Combat"
game.Players.LocalPlayer.Character.Humanoid:EquipTool(game:GetService("Players").LocalPlayer.Backpack:FindFirstChild(Weapon))
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.Out,0,false,0 ),
{CFrame = CFrame.new(1127.07324, 16.2736206, 1576.84644, -0.999728203, -0, -0.0233147852, -0, 1, -0, 0.0233147852, 0, -0.999728203)}):Play()
wait(5)
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.Out,0,false,0 ),
{CFrame = CFrame.new(1199.98083, 16.2736206, 1668.48767, -0.381666601, -6.71909177e-08, -0.924300075, -2.60219029e-08, 1, -6.19487395e-08, 0.924300075, 4.08281575e-10, -0.381666601)}):Play()
wait(5)
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.Out,0,false,0 ),
{CFrame = CFrame.new(1261.61719, 16.3373146, 1632.0072, 0.206790164, -6.81194656e-09, -0.978385329, -2.14672582e-08, 1, -1.14997274e-08, 0.978385329, 2.33812809e-08, 0.206790164)}):Play()
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.Out,0,false,0 ),
{CFrame = CFrame.new(1239.54773, 16.4328537, 1567.04456, 0.940980792, -5.81878012e-08, 0.338459909, 4.27872386e-08, 1, 5.29629354e-08, -0.338459909, -3.53553418e-08, 0.940980792)}):Play()
local TweenService = game:GetService("TweenService")
local Tw = TweenService:Create(game.Players.LocalPlayer.Character.HumanoidRootPart,TweenInfo.new(1,Enum.EasingStyle.Linear,Enum.EasingDirection.Out,0,false,0 ),
{CFrame = CFrame.new(1306.60754, 16.2735634, 1567.68677, -0.00938363373, -2.09850004e-08, -0.999955952, 9.14980447e-08, 1, -2.18445475e-08, 0.999955952, -9.16989933e-08, -0.00938363373)}):Play()
end




































