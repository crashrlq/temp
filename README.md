local p, lp = game:GetService("Players"), game.Players.LocalPlayer

for _, v in ipairs(p:GetPlayers()) do
    local algema = v ~= lp and v.Backpack and v.Backpack:FindFirstChild("Dumbell")
    if algema then
        algema.Parent = lp.Backpack
        break
    end
end
