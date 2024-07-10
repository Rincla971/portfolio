local block = script.Parent
local debounce = script.Debounce

local colors = {BrickColor.new("Red flip/flop"), BrickColor.new("Forest green"), BrickColor.new("Bright orange"), BrickColor.new("Yellow flip/flop")}

block.BrickColor = colors[math.random(1, #colors)]

block.Touched:Connect(function(hit)
	if not debounce.Value and hit.Parent:FindFirstChildOfClass("Humanoid") then
		debounce.Value = true
		for i = 1, 20 do
			block.Transparency = i/20
			wait(0.05)
		end
		block.CanCollide = false
		wait(2)
		block.CanCollide = true
		block.Transparency = 0
		debounce.Value = false
	end
end)
