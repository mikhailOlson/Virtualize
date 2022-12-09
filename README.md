-- Virtualize Into Roblox Studio --

-- The Commands
-- Hyperlinks in Hypersky
-- Guidebooks in Google Drive
-- Kickstarter Campaign
-- Open Cloud Permissions
-- Team Create Policy

-- LuaU
-- Free download.zip tutorial and demonstration
-- YouTube Channel
-- Twitter Updates
-- Discord Server

--[[

CommandBar

-- Let's make this automated.

-- Current method uses a for loop to find and display a text based elements inside a 3D environment.

-- Use these commands in the Command Bar to execute these two commands to make your mind visible for your benefit.

-- Insert Billboard Gui
-- Start Copy

local Selection = game:GetService("Selection")

for _, object in pairs(Selection:Get()) do
	if object:IsA("BasePart") then
		local billboard = game.ServerStorage.Billboard:Clone()
		billboard.Parent = object
		billboard.Name = object.Name
		billboard.Text.Text = object.Name
		billboard.Size = UDim2.new(object.Size.Y, 0, object.Size.Y, 0)
	end
end

-- Stop Copy

-- SurfaceText

-- Change text of a SurfaceGui
-- Start Copy

local Selection = game:GetService("Selection")

for _, object in pairs(Selection:Get()) do
	if object:IsA("BasePart") then
		local surfaceGui = object.SurfaceGui
		surfaceGui.TextLabel.Text = object.Name
	end
end

-- Stop Copy

--]]
