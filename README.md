-- Criação da interface
local ScreenGui = Instance.new("ScreenGui")
local MainFrame = Instance.new("Frame")
local TitleLabel = Instance.new("TextLabel")
local MinimizeButton = Instance.new("TextButton")
local PlayButton = Instance.new("TextButton")

local OptionsFrame = Instance.new("Frame")
local ReachButton = Instance.new("TextButton")
local AirHelperButton = Instance.new("TextButton")
local BackButton = Instance.new("TextButton")

local ReachOptionsFrame = Instance.new("Frame")
local ReachLabel = Instance.new("TextLabel")
local ReachInput = Instance.new("TextBox")
local ReachConfirmButton = Instance.new("TextButton")

local AirHelperFrame = Instance.new("Frame")
local AirHelperLabel = Instance.new("TextLabel")
local AirHelperInput = Instance.new("TextBox")
local AirHelperConfirmButton = Instance.new("TextButton")

-- Configurações da Tela Principal
ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

MainFrame.Parent = ScreenGui
MainFrame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
MainFrame.Size = UDim2.new(0.5, 0, 0.5, 0)
MainFrame.Position = UDim2.new(0.25, 0, 0.25, 0)

TitleLabel.Parent = MainFrame
TitleLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
TitleLabel.Size = UDim2.new(1, 0, 0.2, 0)
TitleLabel.Text = "Nickk Hub"
TitleLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
TitleLabel.TextScaled = true

MinimizeButton.Parent = MainFrame
MinimizeButton.BackgroundColor3 = Color3.fromRGB(100, 100, 100)
MinimizeButton.Size = UDim2.new(0.5, 0, 0.2, 0)
MinimizeButton.Position = UDim2.new(0, 0, 0.2, 0)
MinimizeButton.Text = "Minimizar"
MinimizeButton.TextScaled = true

PlayButton.Parent = MainFrame
PlayButton.BackgroundColor3 = Color3.fromRGB(0, 200, 0)
PlayButton.Size = UDim2.new(0.5, 0, 0.2, 0)
PlayButton.Position = UDim2.new(0.5, 0, 0.2, 0)
PlayButton.Text = "Jogar"
PlayButton.TextScaled = true

-- Configurações da Tela de Opções
OptionsFrame.Parent = ScreenGui
OptionsFrame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
OptionsFrame.Size = UDim2.new(0.5, 0, 0.5, 0)
OptionsFrame.Position = UDim2.new(0.25, 0, 0.25, 0)
OptionsFrame.Visible = false

ReachButton.Parent = OptionsFrame
ReachButton.BackgroundColor3 = Color3.fromRGB(0, 200, 0)
ReachButton.Size = UDim2.new(1, 0, 0.2, 0)
ReachButton.Position = UDim2.new(0, 0, 0.2, 0)
ReachButton.Text = "Reach"
ReachButton.TextScaled = true

AirHelperButton.Parent = OptionsFrame
AirHelperButton.BackgroundColor3 = Color3.fromRGB(0, 200, 0)
AirHelperButton.Size = UDim2.new(1, 0, 0.2, 0)
AirHelperButton.Position = UDim2.new(0, 0, 0.4, 0)
AirHelperButton.Text = "Air Helper"
AirHelperButton.TextScaled = true

BackButton.Parent = OptionsFrame
BackButton.BackgroundColor3 = Color3.fromRGB(100, 100, 100)
BackButton.Size = UDim2.new(1, 0, 0.2, 0)
BackButton.Position = UDim2.new(0, 0, 0.6, 0)
BackButton.Text = "Voltar"
BackButton.TextScaled = true

-- Configurações da Tela de Opções de Reach
ReachOptionsFrame.Parent = ScreenGui
ReachOptionsFrame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
ReachOptionsFrame.Size = UDim2.new(0.5, 0, 0.5, 0)
ReachOptionsFrame.Position = UDim2.new(0.25, 0, 0.25, 0)
ReachOptionsFrame.Visible = false

ReachLabel.Parent = ReachOptionsFrame
ReachLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ReachLabel.Size = UDim2.new(1, 0, 0.2, 0)
ReachLabel.Text = "Escolha a distância (1-10):"
ReachLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
ReachLabel.TextScaled = true

ReachInput.Parent = ReachOptionsFrame
ReachInput.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
ReachInput.Size = UDim2.new(1, 0, 0.2, 0)
ReachInput.Position = UDim2.new(0, 0, 0.2, 0)

ReachConfirmButton.Parent = ReachOptionsFrame
ReachConfirmButton.BackgroundColor3 = Color3.fromRGB(0, 200, 0)
ReachConfirmButton.Size = UDim2.new(1, 0, 0.2, 0)
ReachConfirmButton.Position = UDim2.new(0, 0, 0.4, 0)
ReachConfirmButton.Text = "Confirmar"
ReachConfirmButton.TextScaled = true

-- Configurações da Tela de Air Helper
AirHelperFrame.Parent = ScreenGui
AirHelperFrame.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
AirHelperFrame.Size = UDim2.new(0.5, 0, 0.5, 0)
AirHelperFrame.Position = UDim2.new(0.25, 0, 0.25, 0)
AirHelperFrame.Visible = false

AirHelperLabel.Parent = AirHelperFrame
AirHelperLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
AirHelperLabel.Size = UDim2.new(1, 0, 0.2, 0)
AirHelperLabel.Text = "Digite a altura:"
AirHelperLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
AirHelperLabel.TextScaled = true

AirHelperInput.Parent = AirHelperFrame
AirHelperInput.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
AirHelperInput.Size = UDim2.new(1, 0, 0.2, 0)
AirHelperInput.Position = UDim2.new(0, 0, 0.2, 0)

AirHelperConfirmButton.Parent = AirHelperFrame
AirHelperConfirmButton.BackgroundColor3 = Color3.fromRGB(0, 200, 0)
AirHelperConfirmButton.Size = UDim2.new(1, 0, 0.2, 0)
AirHelperConfirmButton.Position = UDim2.new(0, 0, 0.4, 0)
AirHelperConfirmButton.Text = "Confirmar"
AirHelperConfirmButton.TextScaled = true

-- Funções dos Botões
MinimizeButton.MouseButton1Click:Connect(function()
    MainFrame.Visible = false
end)

PlayButton.MouseButton1Click:Connect(function()
    MainFrame.Visible = false
    OptionsFrame.Visible = true
end)

BackButton.MouseButton1Click:Connect(function()
    OptionsFrame.Visible = false
    MainFrame.Visible = true
end)

ReachButton.MouseButton1Click:Connect(function()
    OptionsFrame.Visible = false
    ReachOptionsFrame.Visible = true
end)

AirHelperButton.MouseButton1Click:Connect(function()
    OptionsFrame.Visible = false
    AirHelperFrame.Visible = true
end)

ReachConfirmButton.MouseButton1Click:Connect(function()
    local reachValue = tonumber(ReachInput.Text)
    if reachValue and reachValue >= 1 and reachValue <= 10 then
        print("Reach configurado para: " .. reachValue)
        -- Aqui você pode adicionar a lógica para aplicar a distância no jogo
        ReachOptionsFrame.Visible = false
        OptionsFrame.Visible = true
    else
        print("Por favor, insira um valor válido entre 1 e 10.")
    end
end)

AirHelperConfirmButton.MouseButton1Click:Connect(function()
    local airHeight = tonumber(AirHelperInput.Text)
    if airHeight then
        print("Air Helper configurado para: " .. airHeight)
        -- Aqui você pode adicionar a lógica para aplicar a altura no jogo
        AirHelperFrame.Visible = false
        OptionsFrame.Visible = true
    else
        print("Por favor, insira um valor válido para a altura.")
    end
end)
