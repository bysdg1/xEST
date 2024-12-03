
Config = {}
_G.Config = Config

repeat wait() until game:IsLoaded()

warn("ANTI AFK STARTING")
game:GetService("Players").LocalPlayer.Idled:connect(function()
    game:GetService("VirtualUser"):CaptureController()
    game:GetService("VirtualUser"):ClickButton2(Vector2.new())
end)

local Rayfield = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()
local Window = Rayfield:CreateWindow({
    Name = "xEST HUD",
    Icon = 0, -- Icon in Topbar. Can use Lucide Icons (string) or Roblox Image (number). 0 to use no icon (default).
    LoadingTitle = "Welcome to xEST HUD",
    LoadingSubtitle = "by xEST",
    Theme = "DarkBlue", -- Check https://docs.sirius.menu/rayfield/configuration/themes
 
    DisableRayfieldPrompts = false,
    DisableBuildWarnings = false, -- Prevents Rayfield from warning when the script has a version mismatch with the interface
 
    ConfigurationSaving = {
       Enabled = true,
       FolderName = nil, -- Create a custom folder for your hub/game
       FileName = "xEST Hub"
    },
 
    Discord = {
       Enabled = false, -- Prompt the user to join your Discord server if their executor supports it
       Invite = "noinvitelink", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ABCD would be ABCD
       RememberJoins = true -- Set this to false to make them join the discord every time they load it up
    },
 
    KeySystem = false, -- Set this to true to use our key system
    KeySettings = {
       Title = "Untitled",
       Subtitle = "Key System",
       Note = "No method of obtaining the key is provided", -- Use this to tell the user how to get a key
       FileName = "Key", -- It is recommended to use something unique as other scripts using Rayfield may overwrite your key file
       SaveKey = true, -- The user's key will be saved, but if you change the key, they will be unable to use your script
       GrabKeyFromSite = false, -- If this is true, set Key below to the RAW site you would like Rayfield to get the key from
       Key = {"Hello"} -- List of keys that will be accepted by the system, can be RAW file links (pastebin, github etc) or simple strings ("hello","key22")
    }
})

do 
	AllFuncs = {}
	Players = game.Players
	LocalPlayer = game.Players.LocalPlayer
	Client = game.Players.LocalPlayer


	-- \\ Module GetService // --

	ReplicatedStorage = game:GetService('ReplicatedStorage')
	RunService = game:GetService("RunService")
	VirtualInputManager = game:GetService('VirtualInputManager')
	CollectionService = game:GetService("CollectionService")
	CoreGui = game:GetService("CoreGui")
	HttpService = game:GetService("HttpService")
	TeleportService = game:GetService("TeleportService")
	VirtualUser = game:GetService("VirtualUser")
	VirtualInputManager = game:GetService("VirtualInputManager")
	UserInputService = game:GetService("UserInputService")


	-- \\ Normal Module // --
	
	PlayerGui = LocalPlayer.PlayerGui
	Backpack = LocalPlayer.Backpack
	request = (syn and syn.request) or (http and http.request) or http_request or (fluxus and fluxus.request) or request

	Char = Client.Character
	Character = Client.Character

	repeat 
		LocalPlayer = Players.LocalPlayer
		wait()
	until LocalPlayer

end

PositionCrabCage_Vertigo ={
    CFrame.new(-104.4007568359375, -732.6099243164062, 1204.3885498046875) * CFrame.Angles(0, -0.3745659589767456, -0),
    CFrame.new(-107.8782730102539, -732.9066772460938, 1203.5081787109375) * CFrame.Angles(0, 0.15302927792072296, -0),
    CFrame.new(-110.3257064819336, -733.0648193359375, 1204.068115234375) * CFrame.Angles(0, 0.8794254660606384, -0),
    CFrame.new(-111.78292083740234, -733.1909790039062, 1205.9537353515625) * CFrame.Angles(3.1415927410125732, 1.5097243785858154, -3.1415927410125732),
    CFrame.new(-111.40582275390625, -733.4566650390625, 1211.8505859375) * CFrame.Angles(3.1415927410125732, 1.315722107887268, -3.1415927410125732),
    CFrame.new(-108.41249084472656, -733.5914306640625, 1213.6343994140625) * CFrame.Angles(3.1415927410125732, 0.5387042164802551, -3.1415927410125732),
    CFrame.new(-104.26063537597656, -733.8704833984375, 1214.82373046875) * CFrame.Angles(3.1415927410125732, 0.07061933726072311, -3.1415927410125732),
    CFrame.new(-101.0369873046875, -734.5581665039062, 1214.208984375) * CFrame.Angles(3.1415927410125732, -0.5564708113670349, 3.1415927410125732),
    CFrame.new(-100.00860595703125, -734.03759765625, 1211.9615478515625) * CFrame.Angles(3.1415927410125732, -1.3737242221832275, 3.1415927410125732),
    CFrame.new(-100.0895767211914, -733.7638549804688, 1208.46728515625) * CFrame.Angles(0, -1.1984872817993164, -0),
    CFrame.new(-99.45345306396484, -736.806396484375, 1203.780517578125) * CFrame.Angles(0, -0.7756390571594238, -0),
    CFrame.new(-128.2958221435547, -736.9212646484375, 1249.3873291015625) * CFrame.Angles(3.1415927410125732, -0.49176692962646484, 3.1415927410125732),
    CFrame.new(-126.23558807373047, -736.9212646484375, 1248.9913330078125) * CFrame.Angles(3.1415927410125732, -1.3704849481582642, 3.1415927410125732),
    CFrame.new(-127.13520050048828, -736.9212646484375, 1247.425537109375) * CFrame.Angles(0, -0.7374275922775269, -0),
    CFrame.new(-129.7357635498047, -736.9213256835938, 1250.44580078125) * CFrame.Angles(3.1415927410125732, 0.48840808868408203, -3.1415927410125732),
    CFrame.new(-126.94432067871094, -736.9213256835938, 1250.362060546875) * CFrame.Angles(0, 1.3505123853683472, -0),
    CFrame.new(-137.91253662109375, -736.86376953125, 1237.849365234375) * CFrame.Angles(3.1415927410125732, 0.36204245686531067, -3.1415927410125732),
    CFrame.new(-140.8370819091797, -736.8637084960938, 1236.3424072265625) * CFrame.Angles(3.1415927410125732, 0.9996036887168884, -3.1415927410125732),
    CFrame.new(-141.37989807128906, -736.8637084960938, 1234.0299072265625) * CFrame.Angles(0, 1.3418757915496826, -0),
    CFrame.new(-139.26658630371094, -736.8638305664062, 1228.5595703125) * CFrame.Angles(0, 1.198739767074585, -0),
    CFrame.new(-128.93934631347656, -736.86376953125, 1234.6160888671875) * CFrame.Angles(0, -1.4478051662445068, -0),
    CFrame.new(-129.29656982421875, -736.86376953125, 1231.5958251953125) * CFrame.Angles(0, -0.8000301122665405, -0),
    CFrame.new(-132.85195922851562, -736.86376953125, 1228.7213134765625) * CFrame.Angles(0, -0.3877910375595093, -0),
    CFrame.new(-141.87591552734375, -736.40478515625, 1219.1295166015625) * CFrame.Angles(0, -1.124761939048767, -0),
    CFrame.new(-141.81040954589844, -736.40478515625, 1214.68896484375) * CFrame.Angles(0, -0.6741452813148499, -0),
    CFrame.new(-143.65065002441406, -736.40478515625, 1213.477783203125) * CFrame.Angles(0, 0.13982975482940674, -0),
    CFrame.new(-144.58094787597656, -736.40478515625, 1214.1685791015625) * CFrame.Angles(0, 1.1899499893188477, -0),
    CFrame.new(-144.914306640625, -736.4047241210938, 1217.4248046875) * CFrame.Angles(3.1415927410125732, 1.3227832317352295, -3.1415927410125732)
}

HopServer = function(FullServer) -- Hop Server (Low)
	local FullServer = FullServer or false

	local Http = game:GetService("HttpService")
	local Api = "https://games.roblox.com/v1/games/"

	local _place = game.PlaceId
	local _servers = Api.._place.."/servers/Public?sortOrder=Asc&limit=100"
	local ListServers = function (cursor)
		local Raw = game:HttpGet(_servers .. ((cursor and "&cursor="..cursor) or ""))
		return Http:JSONDecode(Raw)
	end

	local Server, Next; repeat
		local Servers = ListServers(Next)
		Server = Servers.data[1]
		Next = Servers.nextPageCursor
	until Server
	repeat
		if not FullServer then
			game:GetService("TeleportService"):TeleportToPlaceInstance(_place,Server.id,game.Players.LocalPlayer)
		else
			if request then
				local servers = {}
				local req = request(
					{
						Url = string.format("https://games.roblox.com/v1/games/%d/servers/Public?sortOrder=Desc&limit=100&excludeFullGames=true", game.PlaceId)
					}
				).Body;
				local body = game:GetService("HttpService"):JSONDecode(req)
				if body and body.data then
					for i, v in next, body.data do
						if type(v) == "table" and tonumber(v.playing) and tonumber(v.maxPlayers) and v.playing < v.maxPlayers and v.id ~= game.JobId then
							table.insert(servers, 1, v.id)
						end
					end
				end
				if #servers > 0 then
					game:GetService("TeleportService"):TeleportToPlaceInstance(game.PlaceId, servers[math.random(1, #servers)], game.Players.LocalPlayer)
				else
					return "Couldn't find a server."
				end
			end
		end
		wait()
	until game.PlaceId ~= game.PlaceId
end

_hasItem = function(name)
	if Backpack:FindFirstChild(name) then return true end
	if LocalPlayer.Character:FindFirstChild(name) then return true end
end

CheckBait = function(bait)
    for i,v in pairs(PlayerGui.hud.safezone.equipment.rods.scroll.safezone:GetChildren()) do
        if v:IsA("Frame") then
            if tostring(v) == bait then
                return true
            end
        end
    end
end

FPSBoost = function()
    pcall(function()
        local Players, Lighting, StarterGui, MaterialService = game:GetService("Players"), game:GetService("Lighting"), game:GetService("StarterGui"), game:GetService("MaterialService")
        local ME, CanBeEnabled = Players.LocalPlayer, {"ParticleEmitter", "Trail", "Smoke", "Fire", "Sparkles"}
        local function PartOfCharacter(Instance)
            for i, v in pairs(Players:GetPlayers()) do
                if v ~= ME and v.Character and Instance:IsDescendantOf(v.Character) then
                    return true
                end
            end
            return false
        end
        local function DescendantOfIgnore(Instance)
            for i, v in pairs(_G.Ignore) do
                if Instance:IsDescendantOf(v) then
                    return true
                end
            end
            return false
        end
        local function CheckIfBad(Instance)
            pcall(function()
                if not Instance:IsDescendantOf(Players) and not PartOfCharacter(Instance) and ME.Character and not Instance:IsDescendantOf(ME.Character) and not Instance:IsA("BackpackItem") and not Instance:FindFirstAncestorWhichIsA("BackpackItem") then
                    if Instance:IsA("DataModelMesh") then
                            Instance.MeshId = ""
                            Instance.TextureId = ""
                            Instance:Destroy()
                    elseif Instance:IsA("FaceInstance") then
                            Instance.Transparency = 1
                            Instance.Shiny = 1
                            Instance:Destroy()
                    elseif Instance:IsA("ShirtGraphic") then
                            Instance.Graphic = ""
                            Instance:Destroy()
                    elseif table.find(CanBeEnabled, Instance.ClassName) then
                            Instance.Enabled = false
                            Instance:Destroy()
                    elseif Instance:IsA("PostEffect") then
                        Instance.Enabled = false
                    elseif Instance:IsA("Explosion") then
                            Instance.BlastPressure = 1
                            Instance.BlastRadius = 1
                            Instance.Visible = false
                            Instance:Destroy()
                    elseif Instance:IsA("Clothing") or Instance:IsA("SurfaceAppearance") or Instance:IsA("BaseWrap") then
                            Instance:Destroy()
                    elseif Instance:IsA("BasePart") and not Instance:IsA("MeshPart") then
                            Instance.Material = Enum.Material.Plastic
                            Instance.Reflectance = 0
                    elseif Instance:IsA("TextLabel") and Instance:IsDescendantOf(workspace) then
                        Instance.Font = Enum.Font.SourceSans
                        Instance.TextScaled = false
                        Instance.RichText = false
                        Instance.TextSize = 14
                        Instance.Visible = false
                        Instance:Destroy()
                    elseif Instance:IsA("Model") then
                            Instance.LevelOfDetail = 1
                    elseif Instance:IsA("MeshPart") then
                        Instance.Reflectance = 0
                        Instance.Material = Enum.Material.Plastic
                        Instance.Transparency = 1
                        Instance.TextureID = ""
                        Instance.MeshId = ""
                        Instance:Destroy()
                    end
                end
            end)
        end
        for i, v in pairs(MaterialService:GetChildren()) do
            v:Destroy()
        end
        Lighting.GlobalShadows = false
        Lighting.FogEnd = 9e9
        Lighting.ShadowSoftness = 0
        if sethiddenproperty then
            sethiddenproperty(Lighting, "Technology", 2)
        end
        settings().Rendering.QualityLevel = 1
        settings().Rendering.MeshPartDetailLevel = Enum.MeshPartDetailLevel.Level04
        workspace:FindFirstChildOfClass("Terrain").WaterWaveSize = 0
        workspace:FindFirstChildOfClass("Terrain").WaterWaveSpeed = 0
        workspace:FindFirstChildOfClass("Terrain").WaterReflectance = 0
        workspace:FindFirstChildOfClass("Terrain").WaterTransparency = 0
        if sethiddenproperty then
            sethiddenproperty(workspace:FindFirstChildOfClass("Terrain"), "Decoration", false)
        end
        if game:GetService("Lighting"):FindFirstChild("Sky") then
            game:GetService("Lighting"):FindFirstChild("Sky").Parent = game:GetService("Lighting").bloom
        end
        setfflag("TaskSchedulerTargetFps", "1000")
        LocalPlayer.Character.client.oxygen.Disabled = true -- ดำน้ำไม่จำกัด
        game.DescendantAdded:Connect(function(value)
            wait(1)
            CheckIfBad(value)
        end)
        
        game:GetService("UserInputService").WindowFocused:Connect(function()
            game:GetService("RunService"):Set3dRenderingEnabled(true)
        end)
        game:GetService("UserInputService").WindowFocusReleased:Connect(function()
            game:GetService("RunService"):Set3dRenderingEnabled(false)
        end)
    end)
end

CheckFish = function(namefish)
    for i,v in pairs(game:GetService("Players").LocalPlayer.PlayerGui.hud.safezone.bestiary.fish.scroll:GetChildren()) do
        if v:IsA("Frame") then
            for i1,v1 in pairs(v:GetChildren()) do
                if tostring(v1) == "fishname" then
                    if tostring(v1.Text) == namefish then
                        return true
                    end
                end
            end 
        end
    end
    return false
end

do
    Config['Checkpoint'] = nil
    Config['Checkpoint1'] = nil
    Config['SellFish'] = false
end

local Tab = Window:CreateTab("Main", "box")
local TextMain = Tab:CreateSection("Main")
local Toggle = Tab:CreateToggle({ -- FarmLEVEl
   Name = "Farm LEVEL",
   CurrentValue = false,
   Flag = "", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
        Config.FarmLEVEL = Value
        -- Config.SellAllFish = Value
   end,
})
local Toggle = Tab:CreateToggle({ -- Farm Bait Kings Rod
   Name = "Farm Bait Kings Rod",
   CurrentValue = false,
   Flag = "", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
        Config['Checkpoint'] = CFrame.new(-2676.18237, 164.75058, 1754.23584, 0.0655031651, 3.32144232e-08, 0.997852385, -3.94333846e-08, 1, -3.06973398e-08, -0.997852385, -3.7337923e-08, 0.0655031651)
        Config.FarmKings = Value
        Config.SellAllFish = Value
   end,
})
local Toggle = Tab:CreateToggle({ -- Farm Bait Kings Rod
   Name = "Farm Bait The Depths",
   CurrentValue = false,
   Flag = "", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
   Callback = function(Value)
        if Value then
            Config['Checkpoint'] = CFrame.new(-105.406273, -731.702026, 1207.2074, 0.999523878, -4.93017431e-08, 0.0308549777, 4.89722787e-08, 1, 1.14335865e-08, -0.0308549777, -9.91710447e-09, 0.999523878)
            Config.BaitDepths = Value
            Config.SellAllFish = Value
        else
            Config.BaitDepths = Value
            Config.SellAllFish = Value
            Config.FarmLEVEL = Value
        end
   end,
})

task.spawn(function() -- Config.FarmLEVEL
    while true do
        local xEST_delay = 5
        if Config.FarmLEVEL then
            xEST_delay = 0
        end

        if Config.FarmLEVEL then
            pcall(function()
                local RodName = ReplicatedStorage.playerstats[LocalPlayer.Name].Stats.rod.Value
                if Backpack:FindFirstChild(RodName) then
                    LocalPlayer.Character.Humanoid:EquipTool(Backpack:FindFirstChild(RodName))
                end

                if not Config['SellFish'] and (LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame.Position - Vector3.new(Config['Checkpoint'])).magnitude > 20 then
                    LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame = Config['Checkpoint'] * CFrame.new(0, 10, 0)
                end

                if LocalPlayer.Character:FindFirstChild(RodName) and LocalPlayer.Character:FindFirstChild(RodName):FindFirstChild("bobber") then
                    repeat
                        pcall(function()
                            PlayerGui:FindFirstChild("shakeui").safezone:FindFirstChild("button").Size = UDim2.new(1001, 0, 1001, 0)
                            game:GetService("VirtualUser"):Button1Down(Vector2.new(1, 1))
                            game:GetService("VirtualUser"):Button1Up(Vector2.new(1, 1))
                        end)
                        RunService.Heartbeat:Wait()
                    until not LocalPlayer.Character:FindFirstChild(RodName) or LocalPlayer.Character:FindFirstChild(RodName).values.bite.Value or not Config.FarmLEVEL or Config['SellFish']
                    repeat
                        RunService.Heartbeat:Wait()
                        ReplicatedStorage.events.reelfinished:FireServer(1000000000000000000000000, true)
                    until not LocalPlayer.Character:FindFirstChild(RodName) or not LocalPlayer.Character:FindFirstChild(RodName).values.bite.Value or not Config.FarmLEVEL or Config['SellFish']
                else
                    LocalPlayer.Character:FindFirstChild(RodName).events.cast:FireServer(1000000000000000000000000)
                end
            end)
        end        
        task.wait(xEST_delay)
    end
end)

task.spawn(function()
    while true do
        local xEST_delay = 5
        local UpdateMoney, ____ = tostring(game.Players.LocalPlayer.leaderstats["C$"].Value):gsub(',', ''):gsub('C%$', '')
        local CheckMoney = tonumber(UpdateMoney)
        if Config.FarmKings then
            xEST_delay = 0
        end

        if Config.FarmKings then
            if CheckMoney > 120000 and not CheckBait("Kings Rod") and not Config['SellFish'] then
                Config.FarmLEVEL = false
                if LocalPlayer.Character:FindFirstChild("HumanoidRootPart").Position == Vector3.new(1378.80054, -804.293579, -302.879852) then
                    VirtualInputManager:SendKeyEvent(true, "E", false, game)
                    task.wait(.5)
                    VirtualInputManager:SendKeyEvent(false, "E", false, game)
                    if PlayerGui:WaitForChild("over"):WaitForChild("prompt"):WaitForChild("confirm") then
                        for i,v in next, getconnections(game.Players.LocalPlayer.PlayerGui.over.prompt.confirm.MouseButton1Click) do
                            v:Fire()
                        end
                    end
                else
                    LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame = CFrame.new(1378.80054, -804.293579, -302.879852, 0.975128829, -0.00192055583, 0.221630514, 0.00525561022, 0.999881625, -0.0144590577, -0.221576512, 0.0152642475, 0.975023508)
                end
            elseif CheckMoney < 120000 and not CheckBait("Kings Rod") then
                if LocalPlayer.Character:FindFirstChild("HumanoidRootPart").Position == Config['Checkpoint1'] then
                    Config.FarmLEVEL = true
                else
                    LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame = Config['Checkpoint2']
                end
            elseif CheckBait("Kings Rod") then
                if not _hasItem("Kings Rod") then
                    ReplicatedStorage.events.equiprod:FireServer("Kings Rod")
                end
                if LocalPlayer.Character:FindFirstChild("HumanoidRootPart").Position == Config['Checkpoint1'] then
                    Config.FarmLEVEL = true
                else
                    LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame = Config['Checkpoint2']
                end
            end
        end

        if Config.BaitDepths then
            if CheckMoney > 10000 and (not CheckFish("Night Shrimp") or not CheckFish("Spiderfish")) and not Config['SellFish'] then
                if not _hasItem("Crab Cage") then
                    LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame =  CFrame.new(476.072021, 153.499985, 231.742584, 0.745079458, -3.27618217e-08, 0.666975737, -1.03947633e-08, 1, 6.07319635e-08, -0.666975737, -5.21831929e-08, 0.745079458)
                    task.wait(1)
                    VirtualInputManager:SendKeyEvent(true, "E", false, game)
                    task.wait(.5)
                    VirtualInputManager:SendKeyEvent(false, "E", false, game)
                    if game:GetService("Players").LocalPlayer.PlayerGui.over:WaitForChild("prompt") then
                        game:GetService("Players").LocalPlayer.PlayerGui.over.prompt.amount.Text = 50
                        for i,v in next, getconnections(game:GetService("Players").LocalPlayer.PlayerGui.over.prompt.confirm.MouseButton1Click) do
                            v:Fire()
                        end
                    end
                end
                if _hasItem("Crab Cage") then
                    for _,v in PositionCrabCage_Vertigo do
                        LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame = v
                        task.wait(1)
                        LocalPlayer.Character:FindFirstChild("Crab Cage").Deploy:FireServer(v)
                        task.wait(1)
                    end
                    task.wait(420)
                    for i,v in pairs(game:GetService("Workspace").active:GetChildren()) do
                        if tostring(v) == tostring(game.Players.LocalPlayer) then
                            for i1,v1 in pairs(v:GetChildren()) do
                                if tostring(v1) == tostring("handle") then
                                    game.Players.LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame = v1.CFrame
                                    task.wait(.2)
                                    VirtualInputManager:SendKeyEvent(true,"E",false,game)
                                    task.wait(2)
                                    VirtualInputManager:SendKeyEvent(false,"E",false,game)
                                end
                            end
                        end
                    end
                end
            elseif CheckFish("Night Shrimp") and CheckFish("Spiderfish") and not Config['SellFish'] and ( not CheckFish("Twilight Eel") or not CheckFish("Fangborn Gar") or not CheckFish("Voidfin Mahi") or not CheckFish("Abyssacuda") or not CheckFish("Rubber Ducky") or not CheckFish("Isonade") ) then
                if not CheckFish("Isonade") and game:GetService("Workspace").zones:WaitForChild("fishing"):WaitForChild("Isonade") then
                    Config.FarmLEVEL = false
                    LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame =  game:GetService("Workspace").zones.fishing.Isonade.CFrame * CFrame.new(0,120,0)
                    Config["Checkpoint"] = LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame
                    Config.FarmLEVEL = true
                else
                    Config['Checkpoint'] = CFrame.new(-105.406273, -731.702026, 1207.2074, 0.999523878, -4.93017431e-08, 0.0308549777, 4.89722787e-08, 1, 1.14335865e-08, -0.0308549777, -9.91710447e-09, 0.999523878)
                    Config.FarmLEVEL = true
                end
            else
                Config['Checkpoint'] = CFrame.new(-105.406273, -731.702026, 1207.2074, 0.999523878, -4.93017431e-08, 0.0308549777, 4.89722787e-08, 1, 1.14335865e-08, -0.0308549777, -9.91710447e-09, 0.999523878)
                Config.FarmLEVEL = true
            end
        end

        task.wait(xEST_delay)
    end
end)

task.spawn(function() -- SellAllFish
    while true do
        local xEST_delay = 180
        if Config.SellAllFish and Config.FarmLEVEL then
            pcall(function()
                Config['SellFish'] = true
                LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame = CFrame.new(464.833344, 150.633499, 228.220322, 0.999603391, -5.24686827e-09, 0.0281608645, 4.82757434e-09, 1, 1.49572248e-08, -0.0281608645, -1.48153445e-08, 0.999603391)
                task.wait(3)
                VirtualInputManager:SendKeyEvent(true,"E",false,game)
                VirtualInputManager:SendKeyEvent(false,"E",false,game)
                task.wait(.5)
                workspace.world.npcs:FindFirstChild("Marc Merchant").merchant.sellall:InvokeServer()
                Config['SellFish'] = false
            end)
        end
        task.wait(xEST_delay)
    end
end)


local Teleport = Window:CreateTab("Teleport", "asterisk")
local TextTeleport = Teleport:CreateSection("Teleport")
TeleportPlayer = {
    Trident = CFrame.new(-1479.48987, -228.710632, -2391.39307, 0.0435845852, 0, 0.999049723, 0, 1, 0, -0.999049723, 0, 0.0435845852),
    Keepers = CFrame.new(1296.32007, -808.551941, -298.938171, 0.0735510588, -0, -0.997291446, 0, 1, -0, 0.997291446, 0, 0.0735510588),
    Snow = CFrame.new(2648.67578, 139.066055, 2521.29736, 0.4648332, 0, 0.885398269, 0, 1, 0, -0.885398269, 0, 0.4648332),
    Mod = CFrame.new(-29.8367615, -250.484863, 199.11615, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247),
    Merlin = CFrame.new(-949.014587, 231.533966, -985.975403, -0.342042685, 0, -0.939684391, 0, 1, 0, 0.939684391, 0, -0.342042685),
    Sunstone = CFrame.new(-933.259705, 128.143951, -1119.52063, -0.342042685, 0, -0.939684391, 0, 1, 0, 0.939684391, 0, -0.342042685),
    Moosewood = CFrame.new(383.101135, 131.240601, 243.933853, -0.457844615, 0, -0.889032245, 0, 1, 0, 0.889032245, 0, -0.457844615),
    Swamp = CFrame.new(2501.48584, 127.758324, -720.699463, 0, 0, -1, 0, 1, 0, 1, 0, 0),
    Mirrorroom = CFrame.new(259.707764, -871.393188, 4140.30273, -1, 0, 0, 0, 1, 0, 0, 0, -1),
    Vertigo = CFrame.new(-112.007278, -492.901093, 1040.32788, -1, 0, 0, 0, 1, 0, 0, 0, -1),
    Snowcap = CFrame.new(2648.67578, 139.066055, 2521.29736, 0.4648332, 0, 0.885398269, 0, 1, 0, -0.885398269, 0, 0.4648332),
    Thedepths = CFrame.new(568.15271, -701.881104, 1230.8479, -1, 0, 0, 0, 1, 0, 0, 0, -1),
    Thedepthsentrance = CFrame.new(11.4627075, -701.881104, 1230.8479, -1, 0, 0, 0, 1, 0, 0, 0, -1),
    Mushgrove = CFrame.new(2501.48584, 127.758324, -720.699463, 0, 0, -1, 0, 1, 0, 1, 0, 0),
    Wilson = CFrame.new(2938.80591, 277.474762, 2567.13379, 0.4648332, 0, 0.885398269, 0, 1, 0, -0.885398269, 0, 0.4648332),
    Birch = CFrame.new(1742.32031, 138.257874, -2502.23779, 0.596325636, 0, 0.80274266, 0, 1, 0, -0.80274266, 0, 0.596325636),
    Volcano = CFrame.new(-1888.52319, 163.847565, 329.238281, 1, 0, 0, 0, 1, 0, 0, 0, 1),
    Deepshop = CFrame.new(-979.196411, -247.910156, -2699.87207, 0.587748766, 0, 0.809043527, 0, 1, 0, -0.809043527, 0, 0.587748766),
    Roslit = CFrame.new(-1476.51147, 130.168427, 671.685303, 0, 0, -1, 0, 1, 0, 1, 0, 0),
    Spike = CFrame.new(-1254.80054, 133.885559, 1554.20215, -0.145238042, 0.0316812992, -0.988889396, -0.0855418146, 0.995342493, 0.0444515422, 0.985691965, 0.0910474434, -0.141851544),
    Altar = CFrame.new(1296.32007, -808.551941, -298.938171, 0.0735510588, -0, -0.997291446, 0, 1, -0, 0.997291446, 0, 0.0735510588),
    Statue = CFrame.new(72.883667, 138.696487, -1028.41931, 0.0735510588, -0, -0.997291446, 0, 1, -0, 0.997291446, 0, 0.0735510588),
    Enchant = CFrame.new(1296.32007, -808.551941, -298.938171, 0.0735510588, -0, -0.997291446, 0, 1, -0, 0.997291446, 0, 0.0735510588),
    Deep = CFrame.new(-1510.88672, -237.695053, -2852.90674, 0.573598742, 0.000578988635, 0.819136202, -0.000339840539, 0.999999821, -0.000468855433, -0.819136322, -9.44083149e-06, 0.573598862),
    Terrapin = CFrame.new(-143.875244, 141.167603, 1909.60706, -0.166835427, 0.0122494074, -0.985908687, 0.0336381644, 0.999411464, 0.00672492199, 0.98541075, -0.0320421979, -0.167149305),
    Thedepthsobby = CFrame.new(66.9927063, -701.881104, 1230.8479, -1, 0, 0, 0, 1, 0, 0, 0, -1),
    Brine = CFrame.new(-1794.10596, -145.849701, -3302.92358, -5.16176224e-05, 3.10316682e-06, 0.99999994, 0.119907647, 0.992785037, 3.10316682e-06, -0.992785037, 0.119907647, -5.16176224e-05),
    Thedepthsmazeexit = CFrame.new(978.142822, -686.911133, 1253.74231, -0.22495985, 0, 0.974368095, 0, 1, 0, -0.974368095, 0, -0.22495985),
    Executive = CFrame.new(-29.8367615, -250.484863, 199.11615, 0.707134247, -0, -0.707079291, 0, 1, -0, 0.707079291, 0, 0.707134247),
    Arch = CFrame.new(998.966797, 126.684937, -1237.14343, 0, 0, -1, 0, 1, 0, 1, 0, 0),
    Forsaken = CFrame.new(-2498.24585, 133.71489, 1624.8551, 1, 0, 0, 0, 1, 0, 0, 0, 1),
    Depthsmazeend = CFrame.new(1683.63269, -896.821045, 1440.54773, -1, 0, 0, 0, 1, 0, 0, 0, -1),
}

local SelectPlayerTeleport
local Dropdown = Teleport:CreateDropdown({
    Name = "Select Teleport",
    Options = {
        "Trident",
        "Keepers",
        "Snow",
        "Mod",
        "Merlin",
        "Sunstone",
        "Moosewood",
        "Swamp",
        "Mirrorroom",
        "Vertigo",
        "Snowcap",
        "Thedepths",
        "Thedepthsentrance",
        "Mushgrove",
        "Wilson",
        "Birch",
        "Volcano",
        "Deepshop",
        "Roslit",
        "Spike",
        "Altar",
        "Statue",
        "Enchant",
        "Deep",
        "Terrapin",
        "Thedepthsobby",
        "Brine",
        "Thedepthsmazeexit",
        "Executive",
        "Arch",
        "Forsaken",
        "Depthsmazeend"
    },
    CurrentOption = {""},
    MultipleOptions = false,
    Flag = "Dropdown1", -- A flag is the identifier for the configuration file, make sure every element has a different flag if you're using configuration saving to ensure no overlaps
    Callback = function(Options)
        SelectPlayerTeleport = Options[1]
    end,
})
local Button = Teleport:CreateButton({
    Name = "Teleport",
    Callback = function()
        for i,v in pairs(TeleportPlayer) do
            if tostring(SelectPlayerTeleport) == tostring(i) then
                LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame = v
            end
        end
    end,
})


local TextTeleport1 = Teleport:CreateSection("Teleport Server")
local Button = Teleport:CreateButton({
    Name = "Rejoin",
    Callback = function()
        TeleportService:TeleportToPlaceInstance(game.placeId, game.jobId, game.Players.LocalPlayer);
    end,
})
local Button = Teleport:CreateButton({
    Name = "Hop Server",
    Callback = function()
        HopServer(true)
    end,
})
local Button = Teleport:CreateButton({
    Name = "Hop Server Low",
    Callback = function()
        HopServer(false)
    end,
})

-- FPSBoost()
-- if game:GetService("Workspace").zones:WaitForChild("fishing"):WaitForChild("Isonade") then
--     LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame =  game:GetService("Workspace").zones.fishing.Isonade.CFrame * CFrame.new(0,120,0)
-- end


-- for i,v in pairs(game:GetService("Players")["testuser_z2"].PlayerGui.hud.safezone.bestiary.fish.scroll:GetChildren()) do
--     if v:IsA("Frame") then
--         test = tostring(tostring(v):gsub(' ', '')):sub(2)
--         print(test)
--     end
-- end
-- for i,v in PositionCrabCage_Vertigo do
--     LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame = v
--     task.wait(.5)
--     LocalPlayer.Character:FindFirstChild("Crab Cage").Deploy:FireServer(v)
--     task.wait(.5)
-- end
-- for i,v in pairs(game:GetService("Workspace").active:GetChildren()) do
--     if tostring(v) == tostring(game.Players.LocalPlayer) then
--         for i1,v1 in pairs(v:GetChildren()) do
--             if tostring(v1) == tostring("handle") then
--                 game.Players.LocalPlayer.Character:FindFirstChild("HumanoidRootPart").CFrame = v1.CFrame
--                 task.wait(.2)
--                 VirtualInputManager:SendKeyEvent(true,"E",false,game)
--                 task.wait(2)
--                 VirtualInputManager:SendKeyEvent(false,"E",false,game)
--             end
--         end
--     end
-- end
