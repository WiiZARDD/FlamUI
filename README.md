<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/yg2mU20.png" />
		</td>
	</tr>
	<tr>

<p align="center">
Flam UI LIb is a stabilized fork of Mercury by @WiiZARDD. If you have any questions, contact me Via discord.

<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/UG1oOC9.png" />
		</td>
	</tr>
	<tr>
	
> `loadstring(game:HttpGet("https://raw.githubusercontent.com/WiiZARDD/FlamUI/main/src.lua"))()`
		
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/7PyqLOY.png" />
		</td>
	</tr>
	<tr>
	
```
    local GUI= Mercury:Create{
    Name = "Mercury",
    Size = UDim2.fromOffset(600, 400),
    Theme = Mercury.Themes.Dark,
    Link = "https://github.com/deeeity/mercury-lib"
} 
```

<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/5O11sal.png" />
		</td>
	</tr>
	<tr>
	
```
local Tab = GUI:Tab{
	Name = "New Tab",
	Icon = "rbxassetid://8569322835"
}
```
		
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/tfRbyZS.png" />
		</td>
	</tr>
	<tr>
	
```
Tab:Button{
	Name = "Button",
	Description = nil,
	Callback = function() end
}
```
		
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/QHksuZE.png" />
		</td>
	</tr>
	<tr>
	
```
Tab:Toggle{
	Name = "Toggle",
	StartingState = false,
	Description = nil,
	Callback = function(state) end
}
```
		
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/VN6Mfbn.png" />
		</td>
	</tr>
	<tr>
	
```
Tab:Textbox{
	Name = "Textbox",
	Callback = function(text) end
}
```
		
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/qySzL5D.png" />
		</td>
	</tr>
	<tr>
	
```
local MyDropdown = Tab:Dropdown{
	Name = "Dropdown",
	StartingText = "Select...",
	Description = nil,
	Items = {
		{"Hello", 1}, 		-- {name, value}
		12,			-- or just value, which is also automatically taken as name
		{"Test", "bump the thread pls"}
	},
	Callback = function(item) return end
}

MyDropdown:AddItems({
	{"NewItem", 12},		-- {name, value}
	400				-- or just value, which is also automatically taken as name
})

MyDropdown:RemoveItems({
	"NewItem", "Hello"		-- just the names to get removed (upper/lower case ignored)
})

MyDropdown:Clear()
```
		
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/tlJB6fi.png" />
		</td>
	</tr>
	<tr>
	
```
Tab:Slider{
	Name = "Slider",
	Default = 50,
	Min = 0,
	Max = 100,
	Callback = function() end
}
```
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/V9yXXby.png" />
		</td>
	</tr>
	<tr>
	
```
Tab:Keybind{
	Name = "Keybind",
	Keybind = nil,
	Description = nil
}
```
		
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/ToYPfh4.png" />
		</td>
	</tr>
	<tr>
	
```
GUI:Prompt{
	Followup = false,
	Title = "Prompt",
	Text = "Prompts are cool",
	Buttons = {
		ok = function()
			return true
		end
		no = function()
			return false
		end
	}
}
```
		
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/drbjY97.png" />
		</td>
	</tr>
	<tr>
	
```
GUI:Notification{
	Title = "Alert",
	Text = "You shall bump the thread on V3rmillion!",
	Duration = 3,
	Callback = function() end
}
```
		
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/lKFUmBG.png" />
		</td>
	</tr>
	<tr>
	
```
Tab:ColorPicker{
	Style = Mercury.ColorPickerStyles.Legacy,
	Callback = function(color) end
}
```
		
<p align="center">
	<tr>
		<td align="center" style="padding=0;width=50%;">
			<img src="https://i.imgur.com/IknAuK2.png" />
		</td>
	</tr>
	<tr>
	
```
GUI:Credit{
	Name = "Creditor's name",
	Description = "Helped with the script",
	V3rm = "link/name",
	Discord = "helo#1234"
}
```
