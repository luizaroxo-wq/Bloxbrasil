-- ATENÇÃO: Script meramente ilustrativo. Não irá funcionar por si só.
-- Ele demonstra a LÓGICA usada pelos scripts reais.

-- Função principal que fica "ouvindo" o chat em busca do aviso de fruta
game:GetService("Players").LocalPlayer.PlayerGui.Chat.Frame.ChatBarParentFrame.Frame.ChildAdded:Connect(function(message)
    -- Se a mensagem do jogo for sobre a Dragon East (exemplo)
    if message.Text:find("Dragon East") then
        print("Fruta Dragon East encontrada! Teleportando...")
        -- O script REAL teria o código para achar as coordenadas e teleportar
        -- Teleportar para as coordenadas (exemplo: game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(123, 50, 456))
        
        -- Aguarda um instante para dar tempo de chegar
        task.wait(0.5)
        
        -- O script REAL teria o código para interagir com a fruta e coletá-la
        print("Fruta coletada e armazenada!")
        
        -- Código para comer a fruta (se desejado)
        -- Pressionaria a tecla de inventário, procuraria pela fruta e clicaria em "Comer"
    end
end)

-- Mantém o script rodando
while task.wait(1) do
    -- O script REAL teria código anti-AFK aqui
end
