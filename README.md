# _this is not Fe_
it works whit some **Limited Emotes**
*example:*
![MyBrother](https://github.com/user-attachments/assets/aae6899e-3783-4f2a-94fd-0edaf989c161)
& some **Kill Emotes**
*example:*
![STILL_FUNNY](https://github.com/user-attachments/assets/86dcff01-4a80-42de-ba61-b97c091c849b)

# Script:
```Luau
local v364 = game:GetService("Players")
                local v365 = game:GetService("ReplicatedStorage")
                local v366 = v364.LocalPlayer
                local v367 = v366.Character or v366.CharacterAdded:Wait()
                local v368 = v367:WaitForChild("Humanoid")
                local v369 = Instance.new("Animation")
                v369.AnimationId = "rbxassetid://emote id here"
                v368:LoadAnimation(v369):Play()
                local v370 = Instance.new("Accessory")
                v370.Name = "#EmoteHolder_" .. math.random(1, 100000)
                v370.Parent = v367
                v370:SetAttribute("EmoteProperty", true)
                require(v365.Emotes.VFX):MainFunction({
                    Character = v367,
                    vfxName = "emote name here",
                    SpecificModule = v365.Emotes.VFX,
                    AnimSent = put the same emote id here,
                    RealBind = v370
                })
```
**Some emote names that work:**
`Last Will` `Embers` `Final Stand` `Final Spark` `Ruthless` `Divine Form`
`Boss Raid` `Time Shift` `Lethal Beam` `True Aura` `Flower Bomb` `Sure Hit` `STILL FUNNY?`
