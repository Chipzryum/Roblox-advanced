local tools = game.StarterPack.Pickaxes
local player = game.Players.LocalPlayer


script.Parent.ClickDetector.MouseClick:Connect(function(player)
	-- Ensure the pickaxe exists in the StarterPack
	if tools:FindFirstChild("WoodenPickaxe") then
		local pickaxe = tools.WoodenPickaxe:Clone()
		pickaxe.Parent = player.Backpack
	else
		warn("WoodenPickaxe not found in StarterPack")
	end
end)
