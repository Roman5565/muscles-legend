-- Gui to Lua
-- Version: 3.2

-- Instances:

local Muclelenendscript = Instance.new("ScreenGui")
local Drag = Instance.new("Frame")
local Close = Instance.new("TextButton")
local Minimize = Instance.new("TextButton")
local Frame = Instance.new("Frame")
local ScrollingFrame = Instance.new("ScrollingFrame")
local Home = Instance.new("TextButton")
local Teleports = Instance.new("TextButton")
local Removegui = Instance.new("TextButton")
local Youtube = Instance.new("TextButton")
local Hitbox = Instance.new("TextButton")
local H0 = Instance.new("Frame")
local Good = Instance.new("TextLabel")
local Name1 = Instance.new("TextLabel")
local Rejoin = Instance.new("TextButton")
local Tele = Instance.new("ScrollingFrame")
local Tinyisland = Instance.new("TextButton")
local Frostgym = Instance.new("TextButton")
local Mythicalgym = Instance.new("TextButton")
local Firegym = Instance.new("TextButton")
local Legendgym = Instance.new("TextButton")
local Muscleking = Instance.new("TextButton")
local sandisland = Instance.new("TextButton")
local Magmaring = Instance.new("TextButton")
local Desertring = Instance.new("TextButton")
local YT = Instance.new("ScrollingFrame")
local Sub = Instance.new("TextLabel")
local link = Instance.new("TextLabel")
local CC = Instance.new("TextLabel")
local Hitb = Instance.new("ScrollingFrame")
local TextHitb = Instance.new("TextBox")
local Execute = Instance.new("TextButton")
local Open = Instance.new("TextButton")

--Properties:

Muclelenendscript.Name = "Mucle lenend script"
Muclelenendscript.Parent = game.CoreGui
Muclelenendscript.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Drag.Name = "Drag"
Drag.Parent = Muclelenendscript
Drag.BackgroundColor3 = Color3.fromRGB(63, 63, 63)
Drag.BorderSizePixel = 0
Drag.Position = UDim2.new(0.173316821, 0, 0.0406249985, 0)
Drag.Size = UDim2.new(0, 355, 0, 30)
Drag.Active = true
Drag.Draggable = true
Drag.Visible = false

Close.Name = "Close"
Close.Parent = Drag
Close.BackgroundColor3 = Color3.fromRGB(63, 63, 63)
Close.BorderSizePixel = 0
Close.Position = UDim2.new(0.915493011, 0, 0, 0)
Close.Size = UDim2.new(0, 30, 0, 30)
Close.Font = Enum.Font.SourceSans
Close.Text = "X"
Close.TextColor3 = Color3.fromRGB(255, 255, 255)
Close.TextScaled = true
Close.TextSize = 14.000
Close.TextWrapped = true
Close.MouseButton1Click:Connect(function()
	Drag.Visible = false
	Open.Visible = true
end)

Minimize.Name = "Minimize"
Minimize.Parent = Drag
Minimize.BackgroundColor3 = Color3.fromRGB(63, 63, 63)
Minimize.BorderSizePixel = 0
Minimize.Position = UDim2.new(0.830985904, 0, 0, 0)
Minimize.Size = UDim2.new(0, 30, 0, 30)
Minimize.Font = Enum.Font.SourceSans
Minimize.Text = "-"
Minimize.TextColor3 = Color3.fromRGB(255, 255, 255)
Minimize.TextScaled = true
Minimize.TextSize = 14.000
Minimize.TextWrapped = true
function Mini()
	if Minimize.Text == "-" then
		Minimize.Text = "+"
		Frame.Visible = false
	elseif Minimize.Text == "+" then
		Minimize.Text = "-"
		Frame.Visible = true
	end
end
Minimize.MouseButton1Click:Connect(Mini)

Frame.Parent = Drag
Frame.BackgroundColor3 = Color3.fromRGB(63, 63, 63)
Frame.BorderSizePixel = 0
Frame.Position = UDim2.new(0, 0, 2, 0)
Frame.Size = UDim2.new(0, 355, 0, 223)

ScrollingFrame.Parent = Frame
ScrollingFrame.Active = true
ScrollingFrame.BackgroundColor3 = Color3.fromRGB(95, 95, 95)
ScrollingFrame.BorderSizePixel = 0
ScrollingFrame.Size = UDim2.new(0, 75, 0, 223)
ScrollingFrame.ScrollBarThickness = 0

Home.Name = "Home"
Home.Parent = ScrollingFrame
Home.BackgroundColor3 = Color3.fromRGB(139, 139, 139)
Home.BorderSizePixel = 2
Home.Size = UDim2.new(0, 75, 0, 35)
Home.Font = Enum.Font.SourceSans
Home.Text = "Home"
Home.TextColor3 = Color3.fromRGB(255, 255, 255)
Home.TextScaled = true
Home.TextSize = 14.000
Home.TextWrapped = true
Home.MouseButton1Click:Connect(function()
	YT.Visible = false
	Hitb.Visible = false
	Tele.Visible = false
	H0.Visible = true
end)

Teleports.Name = "Teleports"
Teleports.Parent = ScrollingFrame
Teleports.BackgroundColor3 = Color3.fromRGB(139, 139, 139)
Teleports.BorderSizePixel = 2
Teleports.Position = UDim2.new(0, 0, 0.0784753338, 0)
Teleports.Size = UDim2.new(0, 75, 0, 35)
Teleports.Font = Enum.Font.SourceSans
Teleports.Text = "Teleports"
Teleports.TextColor3 = Color3.fromRGB(255, 255, 255)
Teleports.TextScaled = true
Teleports.TextSize = 14.000
Teleports.TextWrapped = true
Teleports.MouseButton1Click:Connect(function()
	YT.Visible = false
	Hitb.Visible = false
	Tele.Visible = true
	H0.Visible = false
end)

Removegui.Name = "Remove gui"
Removegui.Parent = ScrollingFrame
Removegui.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
Removegui.BorderSizePixel = 2
Removegui.Position = UDim2.new(0, 0, 0.327354252, 0)
Removegui.Size = UDim2.new(0, 75, 0, 35)
Removegui.Font = Enum.Font.SourceSans
Removegui.Text = "Remove gui"
Removegui.TextColor3 = Color3.fromRGB(0, 0, 0)
Removegui.TextScaled = true
Removegui.TextSize = 14.000
Removegui.TextWrapped = true
Removegui.MouseButton1Click:Connect(function()
	Muclelenendscript:Destroy()
end)

Youtube.Name = "Youtube"
Youtube.Parent = ScrollingFrame
Youtube.BackgroundColor3 = Color3.fromRGB(139, 139, 139)
Youtube.BorderSizePixel = 2
Youtube.Position = UDim2.new(0, 0, 0.242152452, 0)
Youtube.Size = UDim2.new(0, 75, 0, 35)
Youtube.Font = Enum.Font.SourceSans
Youtube.Text = "Youtube"
Youtube.TextColor3 = Color3.fromRGB(255, 255, 255)
Youtube.TextScaled = true
Youtube.TextSize = 14.000
Youtube.TextWrapped = true
Youtube.MouseButton1Click:Connect(function()
	YT.Visible = true
	Hitb.Visible = false
	Tele.Visible = false
	H0.Visible = false
end)

Hitbox.Name = "Hitbox"
Hitbox.Parent = ScrollingFrame
Hitbox.BackgroundColor3 = Color3.fromRGB(139, 139, 139)
Hitbox.BorderSizePixel = 2
Hitbox.Position = UDim2.new(0, 0, 0.157000005, 0)
Hitbox.Size = UDim2.new(0, 75, 0, 35)
Hitbox.Font = Enum.Font.SourceSans
Hitbox.Text = "Hitbox"
Hitbox.TextColor3 = Color3.fromRGB(255, 255, 255)
Hitbox.TextScaled = true
Hitbox.TextSize = 14.000
Hitbox.TextWrapped = true
Hitbox.MouseButton1Click:Connect(function()
	YT.Visible = false
	Hitb.Visible = true
	Tele.Visible = false
	H0.Visible = false
end)

H0.Name = "H0"
H0.Parent = Frame
H0.BackgroundColor3 = Color3.fromRGB(95, 95, 95)
H0.Position = UDim2.new(0.239436626, 0, 0.0493273549, 0)
H0.Size = UDim2.new(0, 262, 0, 201)

Good.Name = "Good"
Good.Parent = H0
Good.BackgroundColor3 = Color3.fromRGB(95, 95, 95)
Good.BorderSizePixel = 0
Good.Size = UDim2.new(0, 262, 0, 71)
Good.Font = Enum.Font.SourceSans
Good.Text = "Thanks for using Muscle legend gui  V1"
Good.TextColor3 = Color3.fromRGB(255, 255, 255)
Good.TextScaled = true
Good.TextSize = 14.000
Good.TextWrapped = true

Name1.Name = "Name1"
Name1.Parent = H0
Name1.BackgroundColor3 = Color3.fromRGB(95, 95, 95)
Name1.BorderSizePixel = 0
Name1.Position = UDim2.new(0, 0, 0.378109455, 0)
Name1.Size = UDim2.new(0, 262, 0, 71)
Name1.Font = Enum.Font.SourceSans
Name1.Text = ""
Name1.TextColor3 = Color3.fromRGB(255, 255, 255)
Name1.TextScaled = true
Name1.TextSize = 14.000
Name1.TextWrapped = true
pcall(function()
	Name1.Text = game.Players:GetPlayerFromCharacter(game.Workspace.CurrentCamera.CameraSubject.Parent).Name
end)

Rejoin.Name = "Rejoin"
Rejoin.Parent = H0
Rejoin.BackgroundColor3 = Color3.fromRGB(95, 95, 95)
Rejoin.BorderSizePixel = 0
Rejoin.Position = UDim2.new(0, 0, 0.731343269, 0)
Rejoin.Size = UDim2.new(0, 262, 0, 50)
Rejoin.Font = Enum.Font.SourceSans
Rejoin.Text = "Rejoin"
Rejoin.TextColor3 = Color3.fromRGB(255, 255, 255)
Rejoin.TextScaled = true
Rejoin.TextSize = 100.000
Rejoin.TextWrapped = true
Rejoin.MouseButton1Click:Connect(function()
	game:GetService("TeleportService"):Teleport(game.PlaceId)
end)


Tele.Name = "Tele"
Tele.Parent = Frame
Tele.Active = true
Tele.BackgroundColor3 = Color3.fromRGB(95, 95, 95)
Tele.BorderSizePixel = 0
Tele.Position = UDim2.new(0.238999993, 0, 0.0489999987, 0)
Tele.Size = UDim2.new(0, 262, 0, 201)
Tele.Visible = false
Tele.CanvasSize = UDim2.new(0, 0, 2.20000005, 0)
Tele.ScrollBarThickness = 0

Tinyisland.Name = "Tiny island"
Tinyisland.Parent = Tele
Tinyisland.BackgroundColor3 = Color3.fromRGB(193, 0, 0)
Tinyisland.BorderSizePixel = 0
Tinyisland.Size = UDim2.new(0, 262, 0, 50)
Tinyisland.Font = Enum.Font.SourceSans
Tinyisland.Text = "Tiny island"
Tinyisland.TextColor3 = Color3.fromRGB(0, 0, 0)
Tinyisland.TextScaled = true
Tinyisland.TextSize = 14.000
Tinyisland.TextWrapped = true
Tinyisland.MouseButton1Click:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-39, 4, 1876)
end)

Frostgym.Name = "Frost gym"
Frostgym.Parent = Tele
Frostgym.BackgroundColor3 = Color3.fromRGB(193, 0, 0)
Frostgym.BorderSizePixel = 0
Frostgym.Position = UDim2.new(0, 0, 0.11210762, 0)
Frostgym.Size = UDim2.new(0, 262, 0, 50)
Frostgym.Font = Enum.Font.SourceSans
Frostgym.Text = "Frost gym"
Frostgym.TextColor3 = Color3.fromRGB(0, 0, 0)
Frostgym.TextScaled = true
Frostgym.TextSize = 14.000
Frostgym.TextWrapped = true
Frostgym.MouseButton1Click:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-2590, 4, -409)
end)

Mythicalgym.Name = "Mythical gym"
Mythicalgym.Parent = Tele
Mythicalgym.BackgroundColor3 = Color3.fromRGB(193, 0, 0)
Mythicalgym.BorderSizePixel = 0
Mythicalgym.Position = UDim2.new(0, 0, 0.224215239, 0)
Mythicalgym.Size = UDim2.new(0, 262, 0, 50)
Mythicalgym.Font = Enum.Font.SourceSans
Mythicalgym.Text = "Mythical gym"
Mythicalgym.TextColor3 = Color3.fromRGB(0, 0, 0)
Mythicalgym.TextScaled = true
Mythicalgym.TextSize = 14.000
Mythicalgym.TextWrapped = true
Mythicalgym.MouseButton1Click:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(2224, 4, 1072)
end)

Firegym.Name = "Fire gym"
Firegym.Parent = Tele
Firegym.BackgroundColor3 = Color3.fromRGB(193, 0, 0)
Firegym.BorderSizePixel = 0
Firegym.Position = UDim2.new(0, 0, 0.336322844, 0)
Firegym.Size = UDim2.new(0, 262, 0, 50)
Firegym.Font = Enum.Font.SourceSans
Firegym.Text = "Fire gym"
Firegym.TextColor3 = Color3.fromRGB(0, 0, 0)
Firegym.TextScaled = true
Firegym.TextSize = 14.000
Firegym.TextWrapped = true
Firegym.MouseButton1Click:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-6733, 4, -1283)
end)

Legendgym.Name = "Legend gym"
Legendgym.Parent = Tele
Legendgym.BackgroundColor3 = Color3.fromRGB(193, 0, 0)
Legendgym.BorderSizePixel = 0
Legendgym.Position = UDim2.new(0, 0, 0.448430479, 0)
Legendgym.Size = UDim2.new(0, 262, 0, 50)
Legendgym.Font = Enum.Font.SourceSans
Legendgym.Text = "Legend gym"
Legendgym.TextColor3 = Color3.fromRGB(0, 0, 0)
Legendgym.TextScaled = true
Legendgym.TextSize = 14.000
Legendgym.TextWrapped = true
Legendgym.MouseButton1Click:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(4632, 988, -3897)
end)

Muscleking.Name = "Muscle king"
Muscleking.Parent = Tele
Muscleking.BackgroundColor3 = Color3.fromRGB(0, 209, 255)
Muscleking.BorderSizePixel = 0
Muscleking.Position = UDim2.new(0, 0, 0.560538113, 0)
Muscleking.Size = UDim2.new(0, 262, 0, 50)
Muscleking.Font = Enum.Font.SourceSans
Muscleking.Text = "Muscle island"
Muscleking.TextColor3 = Color3.fromRGB(0, 0, 0)
Muscleking.TextScaled = true
Muscleking.TextSize = 14.000
Muscleking.TextWrapped = true
Muscleking.MouseButton1Click:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-8582, 14, -5676)
end)

sandisland.Name = "sand island"
sandisland.Parent = Tele
sandisland.BackgroundColor3 = Color3.fromRGB(34, 255, 0)
sandisland.BorderSizePixel = 0
sandisland.Position = UDim2.new(0, 0, 0.672645748, 0)
sandisland.Size = UDim2.new(0, 262, 0, 50)
sandisland.Font = Enum.Font.SourceSans
sandisland.Text = "sand island"
sandisland.TextColor3 = Color3.fromRGB(0, 0, 0)
sandisland.TextScaled = true
sandisland.TextSize = 14.000
sandisland.TextWrapped = true
sandisland.MouseButton1Click:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-31, 4, -282)
end)

Magmaring.Name = "Magma ring"
Magmaring.Parent = Tele
Magmaring.BackgroundColor3 = Color3.fromRGB(0, 25, 255)
Magmaring.BorderSizePixel = 0
Magmaring.Position = UDim2.new(0, 0, 0.784753382, 0)
Magmaring.Size = UDim2.new(0, 262, 0, 50)
Magmaring.Font = Enum.Font.SourceSans
Magmaring.Text = "Magma ring"
Magmaring.TextColor3 = Color3.fromRGB(0, 0, 0)
Magmaring.TextScaled = true
Magmaring.TextSize = 14.000
Magmaring.TextWrapped = true
Magmaring.MouseButton1Click:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(4491, 128, -8431)
end)

Desertring.Name = "Desert ring"
Desertring.Parent = Tele
Desertring.BackgroundColor3 = Color3.fromRGB(0, 25, 255)
Desertring.BorderSizePixel = 0
Desertring.Position = UDim2.new(0, 0, 0.896861017, 0)
Desertring.Size = UDim2.new(0, 262, 0, 50)
Desertring.Font = Enum.Font.SourceSans
Desertring.Text = "Desert ring"
Desertring.TextColor3 = Color3.fromRGB(0, 0, 0)
Desertring.TextScaled = true
Desertring.TextSize = 14.000
Desertring.TextWrapped = true
Desertring.MouseButton1Click:Connect(function()
	game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(1007, 154, -7007)
end)

YT.Name = "YT"
YT.Parent = Frame
YT.Active = true
YT.BackgroundColor3 = Color3.fromRGB(95, 95, 95)
YT.Position = UDim2.new(0.238999993, 0, 0.0489999987, 0)
YT.Size = UDim2.new(0, 262, 0, 201)
YT.Visible = false
YT.ScrollBarThickness = 0

Sub.Name = "Sub"
Sub.Parent = YT
Sub.BackgroundColor3 = Color3.fromRGB(95, 95, 95)
Sub.BorderSizePixel = 0
Sub.Size = UDim2.new(0, 262, 0, 47)
Sub.Font = Enum.Font.SourceSans
Sub.Text = "Subscribe to WarriorRoberr"
Sub.TextColor3 = Color3.fromRGB(255, 255, 255)
Sub.TextScaled = true
Sub.TextSize = 14.000
Sub.TextWrapped = true

link.Name = "link"
link.Parent = YT
link.BackgroundColor3 = Color3.fromRGB(95, 95, 95)
link.BorderSizePixel = 0
link.Position = UDim2.new(0, 0, 0.132286996, 0)
link.Size = UDim2.new(0, 262, 0, 47)
link.Font = Enum.Font.SourceSans
link.Text = "link: https://Youtube.com/c/WarriorRoberr"
link.TextColor3 = Color3.fromRGB(255, 255, 255)
link.TextScaled = true
link.TextSize = 14.000
link.TextWrapped = true

CC.Name = "CC"
CC.Parent = Frame
CC.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
CC.BorderSizePixel = 0
CC.Position = UDim2.new(0, 0, -0.134529114, 0)
CC.Size = UDim2.new(0, 355, 0, 30)
CC.Font = Enum.Font.SourceSans
CC.Text = "Script Made by WarriorRoberr"
CC.TextColor3 = Color3.fromRGB(0, 0, 0)
CC.TextScaled = true
CC.TextSize = 14.000
CC.TextWrapped = true

Hitb.Name = "Hitb"
Hitb.Parent = Frame
Hitb.Active = true
Hitb.BackgroundColor3 = Color3.fromRGB(95, 95, 95)
Hitb.BorderSizePixel = 0
Hitb.Position = UDim2.new(0.238999993, 0, 0.0489999987, 0)
Hitb.Size = UDim2.new(0, 262, 0, 201)
Hitb.Visible = false
Hitb.ScrollBarThickness = 0

TextHitb.Name = "TextHitb"
TextHitb.Parent = Hitb
TextHitb.BackgroundColor3 = Color3.fromRGB(255, 0, 4)
TextHitb.Position = UDim2.new(0, 0, 0.0538116582, 0)
TextHitb.Size = UDim2.new(0, 262, 0, 50)
TextHitb.Font = Enum.Font.SourceSans
TextHitb.PlaceholderColor3 = Color3.fromRGB(0, 0, 0)
TextHitb.PlaceholderText = "Size"
TextHitb.Text = ""
TextHitb.TextColor3 = Color3.fromRGB(0, 0, 0)
TextHitb.TextScaled = true
TextHitb.TextSize = 14.000
TextHitb.TextWrapped = true

Execute.Name = "Execute"
Execute.Parent = Hitb
Execute.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Execute.Position = UDim2.new(0.652671754, 0, 0.28699553, 0)
Execute.Size = UDim2.new(0, 69, 0, 50)
Execute.Font = Enum.Font.SourceSans
Execute.Text = "Execute"
Execute.TextColor3 = Color3.fromRGB(249, 249, 249)
Execute.TextScaled = true
Execute.TextSize = 14.000
Execute.TextWrapped = true
Execute.MouseButton1Click:Connect(function()
	_G.HeadSize = TextHitb.Text
	_G.Disabled = true

	game:GetService('RunService').RenderStepped:connect(function()
		if _G.Disabled then
			for i,v in next, game:GetService('Players'):GetPlayers() do
				if v.Name ~= game:GetService('Players').LocalPlayer.Name then
					pcall(function()
						v.Character.HumanoidRootPart.Size = Vector3.new(_G.HeadSize,_G.HeadSize,_G.HeadSize)
						v.Character.HumanoidRootPart.Transparency = 0.9
						v.Character.HumanoidRootPart.Color = Color3.new(1, 0, 0)
						v.Character.HumanoidRootPart.Material = "Neon"
						v.Character.HumanoidRootPart.CanCollide = false
					end)
				end
			end
		end
	end)
end)

Open.Name = "Open"
Open.Parent = Muclelenendscript
Open.BackgroundColor3 = Color3.fromRGB(63, 63, 63)
Open.Position = UDim2.new(0, 0, 0.421875, 0)
Open.Size = UDim2.new(0, 84, 0, 50)
Open.Font = Enum.Font.SourceSans
Open.Text = "Open"
Open.TextColor3 = Color3.fromRGB(255, 255, 255)
Open.TextScaled = true
Open.TextSize = 14.000
Open.TextWrapped = true
Open.MouseButton1Click:Connect(function()
	Open.Visible = false
	Drag.Visible = true
end)
