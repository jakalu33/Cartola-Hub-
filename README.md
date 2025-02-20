--[=[
 d888b  db    db d888888b      .d888b.      db      db    db  .d8b.  
88' Y8b 88    88   `88'        VP  `8D      88      88    88 d8' `8b 
88      88    88    88            odD'      88      88    88 88ooo88 
88  ooo 88    88    88          .88'        88      88    88 88~~~88 
88. ~8~ 88b  d88   .88.        j88.         88booo. 88b  d88 88   88 
 Y888P  ~Y8888P' Y888888P      888888D      Y88888P ~Y8888P' YP   YP  CONVERTER
]=]

-- Instances: 6 | Scripts: 1 | Modules: 0
local G2L = {};

-- StarterGui.Btools
G2L["1"] = Instance.new("ScreenGui", game:GetService("Players").LocalPlayer:WaitForChild("PlayerGui"));
G2L["1"]["Name"] = [[Cartola Hub]];
G2L["1"]["ZIndexBehavior"] = Enum.ZIndexBehavior.Sibling;

-- StarterGui.Btools.Febtools
G2L["2"] = Instance.new("TextButton", G2L["1"]);
G2L["2"]["BorderSizePixel"] = 0;
G2L["2"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
G2L["2"]["TextSize"] = 14;
G2L["2"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["2"]["TextColor3"] = Color3.fromRGB(0, 0, 0);
G2L["2"]["Size"] = UDim2.new(0, 200, 0, 50);
G2L["2"]["Name"] = [[Febtools]];
G2L["2"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["2"]["Text"] = [[CARTOLA HUB]];
G2L["2"]["Position"] = UDim2.new(0.08721625059843063, 0, 0.44979920983314514, 0);

-- StarterGui.Btools.Febtools.LocalScript
G2L["3"] = Instance.new("LocalScript", G2L["2"]);


-- StarterGui.Btools.ImageButton
G2L["4"] = Instance.new("ImageButton", G2L["1"]);
G2L["4"]["BorderSizePixel"] = 0;
G2L["4"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
G2L["4"]["Image"] = [[http://www.roblox.com/asset/?id=9897155096]];
G2L["4"]["Size"] = UDim2.new(1, 100, 1, 100);
G2L["4"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["4"]["Visible"] = false;

-- StarterGui.Btools.ImageButton.Sound
G2L["5"] = Instance.new("Sound", G2L["4"]);
G2L["5"]["Volume"] = 10;
G2L["5"]["Looped"] = true;
G2L["5"]["SoundId"] = [[rbxassetid://7705506391]];
G2L["5"]["RollOffMode"] = Enum.RollOffMode.InverseTapered;

-- StarterGui.Btools.ImageButton.TextLabel
G2L["6"] = Instance.new("TextLabel", G2L["4"]);
G2L["6"]["TextWrapped"] = true;
G2L["6"]["BorderSizePixel"] = 0;
G2L["6"]["TextScaled"] = true;
G2L["6"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
G2L["6"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
G2L["6"]["TextSize"] = 100;
G2L["6"]["TextColor3"] = Color3.fromRGB(255, 0, 0);
G2L["6"]["Size"] = UDim2.new(0, 470, 0, 347);
G2L["6"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
G2L["6"]["Text"] = [[VOCÊ FOI TROLLADO KKKKKK]];
G2L["6"]["BackgroundTransparency"] = 1;
G2L["6"]["Position"] = UDim2.new(0.2486659586429596, 0, 0.24080267548561096, 0);

-- StarterGui.Btools.Febtools.LocalScript
local function C_3()
local script = G2L["3"];
	script.Parent.MouseButton1Click:Connect(function()
		script.Parent.Parent.ImageButton.Visible = true
		script.Parent.Parent.ImageButton.Sound:Play()
		
	end)
end;
task.spawn(C_3);

return G2L["1"], require;
