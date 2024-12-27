-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local _90FOV = Instance.new("TextButton")
local _100FOV = Instance.new("TextButton")
local _80FOV = Instance.new("TextButton")
local _120FOV = Instance.new("TextButton")
local _70FOV = Instance.new("TextButton")
local TextLabel = Instance.new("TextLabel")
local TextLabel_2 = Instance.new("TextLabel")

--Properties:

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(5, 5, 5)
Frame.BorderColor3 = Color3.fromRGB(0, 0, 0)
Frame.BorderSizePixel = 0
Frame.Position = UDim2.new(0.377557755, 0, 0.520045817, 0)
Frame.Size = UDim2.new(0, 402, 0, 231)

_90FOV.Name = "90FOV"
_90FOV.Parent = Frame
_90FOV.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
_90FOV.BorderColor3 = Color3.fromRGB(0, 0, 0)
_90FOV.BorderSizePixel = 0
_90FOV.Position = UDim2.new(0.587064683, 0, 0.608340621, 0)
_90FOV.Size = UDim2.new(0, 148, 0, 36)
_90FOV.Font = Enum.Font.SourceSans
_90FOV.Text = "90 FOV"
_90FOV.TextColor3 = Color3.fromRGB(0, 0, 0)
_90FOV.TextSize = 14.000

_100FOV.Name = "100FOV"
_100FOV.Parent = Frame
_100FOV.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
_100FOV.BorderColor3 = Color3.fromRGB(0, 0, 0)
_100FOV.BorderSizePixel = 0
_100FOV.Position = UDim2.new(0.0273631848, 0, 0.808841646, 0)
_100FOV.Size = UDim2.new(0, 148, 0, 36)
_100FOV.Font = Enum.Font.SourceSans
_100FOV.Text = "100 FOV"
_100FOV.TextColor3 = Color3.fromRGB(0, 0, 0)
_100FOV.TextSize = 14.000

_80FOV.Name = "80FOV"
_80FOV.Parent = Frame
_80FOV.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
_80FOV.BorderColor3 = Color3.fromRGB(0, 0, 0)
_80FOV.BorderSizePixel = 0
_80FOV.Position = UDim2.new(0.587064683, 0, 0.808446288, 0)
_80FOV.Size = UDim2.new(0, 148, 0, 36)
_80FOV.Font = Enum.Font.SourceSans
_80FOV.Text = "80 FOV"
_80FOV.TextColor3 = Color3.fromRGB(0, 0, 0)
_80FOV.TextSize = 14.000

_120FOV.Name = "120FOV"
_120FOV.Parent = Frame
_120FOV.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
_120FOV.BorderColor3 = Color3.fromRGB(0, 0, 0)
_120FOV.BorderSizePixel = 0
_120FOV.Position = UDim2.new(0.0273631848, 0, 0.610645652, 0)
_120FOV.Size = UDim2.new(0, 148, 0, 36)
_120FOV.Font = Enum.Font.SourceSans
_120FOV.Text = "120 [MAX]"
_120FOV.TextColor3 = Color3.fromRGB(0, 0, 0)
_120FOV.TextSize = 14.000

_70FOV.Name = "70FOV"
_70FOV.Parent = Frame
_70FOV.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
_70FOV.BorderColor3 = Color3.fromRGB(0, 0, 0)
_70FOV.BorderSizePixel = 0
_70FOV.Position = UDim2.new(0.315920413, 0, 0.34824878, 0)
_70FOV.Size = UDim2.new(0, 148, 0, 36)
_70FOV.Font = Enum.Font.SourceSans
_70FOV.Text = "Reset FOV [70]"
_70FOV.TextColor3 = Color3.fromRGB(0, 0, 0)
_70FOV.TextSize = 14.000

TextLabel.Parent = Frame
TextLabel.BackgroundColor3 = Color3.fromRGB(5, 5, 5)
TextLabel.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.BorderSizePixel = 0
TextLabel.Position = UDim2.new(0.0597014911, 0, 0.0429592989, 0)
TextLabel.Size = UDim2.new(0, 121, 0, 29)
TextLabel.Font = Enum.Font.SourceSansBold
TextLabel.Text = "FOV MOD v1.0"
TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel.TextSize = 22.000

TextLabel_2.Parent = Frame
TextLabel_2.BackgroundColor3 = Color3.fromRGB(5, 5, 5)
TextLabel_2.BorderColor3 = Color3.fromRGB(0, 0, 0)
TextLabel_2.BorderSizePixel = 0
TextLabel_2.Position = UDim2.new(0.601990044, 0, 0.0429592989, 0)
TextLabel_2.Size = UDim2.new(0, 142, 0, 29)
TextLabel_2.Font = Enum.Font.SourceSansBold
TextLabel_2.Text = "Press Tab to hide"
TextLabel_2.TextColor3 = Color3.fromRGB(255, 255, 255)
TextLabel_2.TextSize = 22.000

-- Scripts:

local function PIXN_fake_script() -- _90FOV.LocalScript 
	local script = Instance.new('LocalScript', _90FOV)

	local button = script.Parent
	local camera = game.Workspace.CurrentCamera
	local newFOV = 90
	
	local function setFOV()
		camera.FieldOfView = newFOV
	end
	
	button.MouseButton1Click:Connect(setFOV)
end
coroutine.wrap(PIXN_fake_script)()
local function UVGF_fake_script() -- _100FOV.LocalScript 
	local script = Instance.new('LocalScript', _100FOV)

	local button = script.Parent
	local camera = game.Workspace.CurrentCamera
	local newFOV = 100
	
	local function setFOV()
		camera.FieldOfView = newFOV
	end
	
	button.MouseButton1Click:Connect(setFOV)
end
coroutine.wrap(UVGF_fake_script)()
local function DHYKEUG_fake_script() -- _80FOV.LocalScript 
	local script = Instance.new('LocalScript', _80FOV)

	local button = script.Parent
	local camera = game.Workspace.CurrentCamera
	local newFOV = 80
	
	local function setFOV()
		camera.FieldOfView = newFOV
	end
	
	button.MouseButton1Click:Connect(setFOV)
end
coroutine.wrap(DHYKEUG_fake_script)()
local function CBPSBS_fake_script() -- _120FOV.LocalScript 
	local script = Instance.new('LocalScript', _120FOV)

	local button = script.Parent
	local camera = game.Workspace.CurrentCamera
	local newFOV = 120
	
	local function setFOV()
		camera.FieldOfView = newFOV
	end
	
	button.MouseButton1Click:Connect(setFOV)
end
coroutine.wrap(CBPSBS_fake_script)()
local function TCWZZRG_fake_script() -- _70FOV.LocalScript 
	local script = Instance.new('LocalScript', _70FOV)

	local button = script.Parent
	local camera = game.Workspace.CurrentCamera
	local newFOV = 70
	
	local function setFOV()
		camera.FieldOfView = newFOV
	end
	
	button.MouseButton1Click:Connect(setFOV)
end
coroutine.wrap(TCWZZRG_fake_script)()
local function NWBIQW_fake_script() -- Frame.LocalScript 
	local script = Instance.new('LocalScript', Frame)

	local ui = script.Parent
	local dragging = false
	local dragInput
	local dragStart = Vector3.zero
	local startOffset = Vector3.zero
	
	ui.InputBegan:Connect(function(input)
		if input.UserInputType == Enum.UserInputType.MouseButton1 then
			dragging = true
			dragInput = input
			dragStart = input.Position
			startOffset = Vector3.new(ui.Position.X.Offset, ui.Position.Y.Offset)
		end
	end)
	
	ui.InputChanged:Connect(function(input)
		if dragging and input.UserInputType == Enum.UserInputType.MouseMovement then
			local delta = input.Position - dragStart
			ui.Position = UDim2.new(0, startOffset.X + delta.X, 0, startOffset.Y + delta.Y)
		end
	end)
	
	ui.InputEnded:Connect(function(input)
		if input.UserInputType == Enum.UserInputType.MouseButton1 then
			dragging = false
			dragInput = nil
		end
	end)
end
coroutine.wrap(NWBIQW_fake_script)()
local function YCQN_fake_script() -- ScreenGui.LocalScript 
	local script = Instance.new('LocalScript', ScreenGui)

	local ui = script.Parent
	local userInputService = game:GetService("UserInputService")
	
	userInputService.InputBegan:Connect(function(input)
		if input.KeyCode == Enum.KeyCode.Tab then
			ui.Enabled = not ui.Enabled
		end
	end)
end
coroutine.wrap(YCQN_fake_script)()
