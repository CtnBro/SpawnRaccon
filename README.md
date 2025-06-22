local pets = {"Raccon", "DragonFly", "CachorroQuenteMístico"} -- Adicione todos os nomes reais aqui

for _, petName in pairs(pets) do
    for i = 1, 100 do
        local pet = Instance.new("Tool")
        pet.Name = petName

        local handle = Instance.new("Part")
        handle.Name = "Handle"
        handle.Size = Vector3.new(1,1,1)
        handle.Parent = pet

        pet.Parent = game.Players.LocalPlayer.Backpack
        wait(0.2)
    end
end
