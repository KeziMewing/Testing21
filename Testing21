local CurrentVersion = "Kezi Hub V1"

    -- Call Library
    local GUI = loadstring(game:HttpGet('https://sirius.menu/rayfield'))()

    -- Main Frame
    local Window = GUI:CreateWindow({
        Name = "CurrentVersion",
        LoadingTitle = "KeziHub Suite",
        LoadingSubtitle = "by KezHub Team",
        Theme = "Default", -- Check https://docs.sirius.menu/rayfield/configuration/themes
     
        DisableRayfieldPrompts = false,
     
        ConfigurationSaving = {
           Enabled = true,
           FolderName = nil, -- Create a custom folder for your hub/game
           FileName = "KeziHub"
        },
     
        Discord = {
           Enabled = false, -- Prompt the user to join your Discord server if their executor supports it
           Invite = "https://discord.gg/9CnjzkGeVp", -- The Discord invite code, do not include discord.gg/. E.g. discord.gg/ABCD would be ABCD
           RememberJoins = true -- Set this to false to make them join the discord every time they load it up
        },
     })


    -- Local Ver
    local TruckAutoFarms = false

    -- AutoFarm Creation
    local Tab = Window:MakeTab({
        Name = "Tab 1",
        Icon = "rbxassetid://136244553696277",
        TestersOnly = false
    })
    
    --[[
    Name = <string> - The name of the tab.
    Icon = <string> - The icon of the tab.
    TestersOnly = <bool> - Makes the tab not accessible to players.
    ]]

    local Section = Tab:AddSection({
        Name = "AutoFarm"
    })
    
    --[[
    Name = <string> - The name of the section.
    ]]


    Tab:AddButton({
        Name = "Truck AutoFarm",
        Callback = function()
                  print("button pressed")
                  while TruckAutoFarms do
                    local args = {
                        [1] = "Truck"
                    }
                    
                    game:GetService("ReplicatedStorage"):WaitForChild("NetworkContainer"):WaitForChild("RemoteEvents"):WaitForChild("Job"):FireServer(unpack(args))
                    
                    wait()

                    local args = {
                        [1] = "Cirebon"
                    }
                    
                    game:GetService("ReplicatedStorage"):WaitForChild("NetworkContainer"):WaitForChild("RemoteEvents"):WaitForChild("TransEvent"):FireServer(unpack(args))

          end    
    })
    
    --[[
    Name = <string> - The name of the button.
    Callback = <function> - The function of the button.
    ]]








end
