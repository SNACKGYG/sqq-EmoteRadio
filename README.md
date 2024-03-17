# sqq-EmoteRadio



- Warning: The animation was not created by us. We have only re-published it and attached an explanation of how to link it <br>
 تنبية لم يتم صنع الانميشن من قبلنا فقط قمنا بإعادة نشره و أرفاق شرح توضيحي لكيفية ربطه

[Discord](https://discord.gg/PWnxxHcpbr)

# Preview معاينة
 ![radioemote](https://github.com/SNACKGYG/sqq-EmoteRadio/assets/97559522/95d48589-9bcc-487f-8bed-f071eb1889a4)

[video]([https://discord.gg/PWnxxHcpbr](https://streamable.com/qforls))

### INSTALLATION التثبيت
1- In your stream animation script, add the files in the <br> في سكربت الحركات الخاص بك stream قم بأضافة الملفات الموجودة في ملف <br>

2- Add the codes below in the specified path <br> قم بأضافة الأكواد في المسار المحدد

3- **Add this to your animations file, and it will most likely be the path <br> ضيف هذا داخل ملف الحركات عندك بالأغلب سيكون المسار**

- Follow the next `qb-emotes > client.lua > AnimationList.lua` folder

```lua
	["wtr"] = {
        "ultra@walkie_talkie",
        "walkie_talkie",
        "Walkie Talkie radio",
        AnimationOptions = {
            Prop = "prop_cs_hand_radio",
            PropBone = 18905,
            PropPlacement = {
                vector3(0.140000, 0.030000, 0.030000),
                vector3(-105.877000, -10.943200, -33.721200),
				},
         EmoteLoop = true,
         EmoteMoving = true
        }
    },
```
### pma-voice التثبيت

```lua
					if FemaleHasRadio then 
						RequestAnimDict('random@arrests')
						while not HasAnimDictLoaded('random@arrests') do
							Citizen.Wait(10)
						end
						TaskPlayAnim(PlayerPedId(), "random@arrests", "generic_radio_enter", 8.0, 2.0, -1, 50, 2.0, 0, 0, 0)
					else
						RequestAnimDict('ultra@walkie_talkie')
						while not HasAnimDictLoaded('ultra@walkie_talkie') do
							Citizen.Wait(10)
						end
						newRadio()
						TaskPlayAnim(PlayerPedId(), 'ultra@walkie_talkie', 'walkie_talkie', 8.0, 2.0, -1, 50, 2.0, 0, 0, 0)
					end

```



[installation](#sqq-EmoteRadio)

