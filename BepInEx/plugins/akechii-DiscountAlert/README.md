# DiscountAlert
Alerts you which items have a discount when the round begins.

## Features
- If an item's price has dropped, it will be highlighted in green.
- If an item's price has raised, it will be highlighted in red. (This *should* be compatible with mods that raise item prices)

## Customization
You can customize the mod by editing the `discount.alert.cfg` file in BepInEx/config/.
### [Alert]
- `DelayAfterLeverIsPulled` - Number of seconds to wait after the "Land ship" or "Start Game" lever is pulled before showing the alert. (Default: `4`)
- `ColorsEnabled` - Enable or disable text colors. (Default: `true`)
- `TitleText` - Alert title text. (Default: `Today\'s discounts`)
- `NoDiscountText` - Alert text when there are no discounts. (Default: `None :( \n Check back tomorrow!`)
- `AlertEnabledWhenNoDiscounts` - Show alert when there are no discounts. (Default: `true`)

### [Colors]
- `PriceUpColor` - Text color when the price goes up (currently only possible with other mods). (Default: `#990000`)
- `PriceDownColor` - Text color when the price goes down. (Default: `#008000`)
- `NoDiscountColor` -  Text color when there are no discounts. (Default: `None`)
- `TitleColor` - Text color for the alert's title (Default: `None`)

## Bug reports
If you find any bugs, please report them in the discord thread:
https://discord.com/channels/1168655651455639582/1188590750091464824

## Changes
- 1.0.0 - Initial release
- 1.1.0 - Alerts are now color coded to add compatibility with other mods
- 1.1.1 - Updated README.md
- 2.0.0 - The mod is now fully client-sided!
- 2.1.0
	- Added a delay to prevent the alert from showing up the moment the "Land ship" lever is pulled
	- Added customization options! Check the "Customization" section for more info
	- Fixed a bug where the alert would be shown twice
- 2.2.0
	- Customizations are now saved in BepInEx/config/discount.alert.cfg to make it easier to share your settings with others, they also wont be overwritten when the mod is updated
	- Added more customization options
- 2.3.0
	- Added a customization option to show the alert when there are no discounts (enabled by default)