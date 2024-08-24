-- first, you need open roblox studio folder. just right click on your roblox studio .lnk file and click file location. copy all files of roblox studio folder, create folder with name what you want, my folder name is "roblox studio".
-- and delete files what containting roblox studio folders or move it in your created folder. after, you need open ExtraContent\LuaPackages. this is not a lie, LuaPackages is real corepackages, if you delete this nothing will be happen except corepackages is no longer exist in roblox studio.
-- second create .lua file in you created folder in ExtraContent/scripts/CoreScripts/ and in this you can use sublime text (sublime.com) or visual studio 2022. and in this type:
local CorePackages = game:GetService("CorePackages")
-- creating modulescript in _Index.
local v = Instance.new("ModuleScript") v.Name = "GetFFLuaFlagGetCorePackages" v.Parent = game.CorePackages.Packages._Index
-- important part dont forgot enable this and set this permissionlevelshown or capability idk rather set permissionlevelshown on game you can this with Enum.PermissionLevelShown.Game 
local Studio = game:GetService("Studio")
game.CorePackages:PermissionLevelShown = Enum.PermissionLevelShown.Game 
settings():Studio["ShowCorePackagesInExplorer"].Enabled = true
brb i add more rly
