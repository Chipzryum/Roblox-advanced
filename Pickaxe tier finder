local pickaxes = game.StarterPack.Pickaxes -- this is a folder
local player = game.Players.LocalPlayer

script.Parent.MouseButton1Down:Connect(function()
	local highestTierPickaxe = nil

	for _, item in ipairs(player.Backpack:GetChildren()) do
		-- Check if the item is a pickaxe and has a child named "Damage"
		if item:IsA("Tool") and item:FindFirstChild("Damage") then
			local damageValue = item.Damage.Value

			-- Update the highest tier pickaxe if the damage value is higher
			if highestTierPickaxe == nil or damageValue > highestTierPickaxe.Damage.Value then
				highestTierPickaxe = item
			end
		end
	end

	-- Print the name of the highest tier pickaxe
	if highestTierPickaxe then
		print("Highest Tier Pickaxe: " .. highestTierPickaxe.Name)
	-- invoke server to save pickaxe later
	else
		print("No Pickaxe Found")
	end
end)
