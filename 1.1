local module = {}

local CoSe = game:GetService("CollectionService")

-- // 2D ESP // --

local function WTS(part)
    local screen = workspace.CurrentCamera:WorldToViewportPoint(part.Position)
    return Vector2.new(screen.x, screen.y)
end

local function round(n)
	return math.ceil(n - 0.5)
end

function module.Create2DESP(part, text, color)
    if CoSe:HasTag(part, "2D_ESP") then
        return warn("Object already has 3D ESP!")
    end

    local box = Drawing.new("Square")
    local name = Drawing.new("Text")
    -- // text settings // --
    name.Text = "Initializing..."
    name.Color = color
    name.Position = WTS(part)
    name.Size = 20.0
    name.Outline = true
    name.Center = true
    name.Visible = true
    -- // box settings // --
    box.Size = Vector2.new(10,10)
    --box.AnchorPoint = Vector2.new(0.5, 0.5)
    box.Position = WTS(part)
    box.Color = color
    box.Thickness = 0.5
    box.Visible = true

    CoSe:AddTag(part, "2D_ESP")

    local RdSt = game:GetService("RunService").Stepped:Connect(function()
        pcall(function()
            local Distance = (workspace.Camera.CFrame.Position - part.Position).Magnitude
            --local Distance = (game:GetService("Players").LocalPlayer.Character.Head.Position - part.Position).Magnitude
            name.Text = "["..round(Distance).."] "..text
            local destroyed = not part:IsDescendantOf(workspace)
            if destroyed and name ~= nil then
                name:Remove()
                box:Remove()
                CoSe:RemoveTag(part, "2D_ESP")
                RdSt:Disconnect()
            end
            if part ~= nil then
                name.Position = WTS(part)
                box.Position = WTS(part)
            end
            local _, screen = workspace.CurrentCamera:WorldToViewportPoint(part.Position)
            if screen then
                name.Visible = true
                box.Visible = true
            else
                name.Visible = false
                box.Visible = false
            end
        end)
    end)
end

-- // END OF 2D ESP // --

-- // 3D ESP // --

local workspace = game:GetService("Workspace")
local player = game:GetService("Players").LocalPlayer
local camera = workspace.CurrentCamera

--// Settings:
local on = true -- Use this if your making gui

local Box_Thickness = 2
local Box_Transparency = 1 -- 1 Visible, 0 Not Visible

local Autothickness = true -- Makes screen less encumbered

local function NewLine(coloror)
    local Box_Color = coloror or Color3.fromRGB(255, 0, 0)
    local line = Drawing.new("Line")
    line.Visible = false
    line.From = Vector2.new(0, 0)
    line.To = Vector2.new(1, 1)
    line.Color = Box_Color
    line.Thickness = Box_Thickness
    line.Transparency = Box_Transparency
    return line
end

--// Main Function:
--[[
    Example: 
    local Part = workspace.Part      
    ESP(Part)
]]
function module.Create3DESP(objected, text, coloror)
    if CoSe:HasTag(objected, "3D_ESP") then
        return warn("Object already has 3D ESP!")
    end
    CoSe:AddTag(objected, "3D_ESP")
    local part = objected   

    --// Lines for 3D box (12)
    local lines = {
        line1  = NewLine(coloror),
        line2  = NewLine(coloror),
        line3  = NewLine(coloror),
        line4  = NewLine(coloror),
        line5  = NewLine(coloror),
        line6  = NewLine(coloror),
        line7  = NewLine(coloror),
        line8  = NewLine(coloror),
        line9  = NewLine(coloror),
        line10 = NewLine(coloror),
        line11 = NewLine(coloror),
        line12 = NewLine(coloror)
    }

    local name = Drawing.new("Text")
    name.Text = text or "Part"
    name.Color = coloror or Color3.new(1, 1, 1)
    name.Position = WTS(part)
    name.Size = 20.0
    name.Outline = true
    name.Center = true
    name.Visible = true
    name.ZIndex = 15
