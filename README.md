# Loader
```
-- List of scripts to load
local scripts = {
    'https://raw.githubusercontent.com/1337h4xx/1/main/Longneck_V_B_H.lua',
    'https://raw.githubusercontent.com/NotH4xor/LOADER-SWIMHUB/main/T_Zoom',
    'https://raw.githubusercontent.com/1337h4xx/1/main/X_3rd_Person',
    'https://raw.githubusercontent.com/1337h4xx/1/main/FreecamUD.lua',
    'https://raw.githubusercontent.com/1337h4xx/1/main/kill_notification',
    'https://raw.githubusercontent.com/1337h4xx/1/main/FullBright%20Loop%20Bypass',
    'https://raw.githubusercontent.com/NotH4xor/LOADER-SWIMHUB/main/Bighead',
    'https://raw.githubusercontent.com/NotH4xor/LOADER-SWIMHUB/main/VisibleESP',
    'https://raw.githubusercontent.com/1337h4xx/1/main/SigmaV3',
-- Removed AmongusHook
}

-- Function to create and resume a coroutine for each script
for _, url in ipairs(scripts) do
    local thread = coroutine.create(function()
        loadstring(game:HttpGet(url, true))()
    end)
    coroutine.resume(thread)
end

-- Add a new script by appending to the 'scripts' table
table.insert(scripts, "new_script_url")
```
# Swim Hub
```
getgenv().key = "60bacfd1c9810cebbab4e9ab58a907d10004986c477d720e77216acde4eabcec"
loadstring(game:HttpGet("https://swimhub.xyz/loader.lua"))()
```
