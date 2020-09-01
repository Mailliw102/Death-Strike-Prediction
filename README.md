## Death Strike Prediction
Death Strike Prediction is a World of Warcraft addon for Death Knights to predict how much healing their next Death Strike will do. It keeps tracks of recent damage taken as well as active buffs and debuffs that affect self-healing to estimate how much the next Death Strike will heal. It also makes this information available via addon messages to other clients such as other copies of the addon or custom addons or WeakAuras that can consume this information.

### Features
* Estimate the healing of the next Death Strike by tracking buffs, debuffs and stats that affect self healing
* Easily add new buffs or debuffs that the addon is not aware of
* Broadcast the predicted healing via addon messages to be usable by WeakAuras or other addons
* Activate predictions for specific Death Knight specializations
* Display the healing prediction as a percentage or as an absolute value
* Maintain a history of how much Death Strike healed for compared to the predicted values (mostly used for debugging)

### Why not just a WeakAura?
There are a few WeakAuras out there that estimate Death Strike healing, but they are not taking into consideration some key effects like Necrotic in Mythic+ or other healing reduction debuffs. These weakauras are also very imprecise in their estimations when there is a lot of incoming damage. I have tested all the ones I could find and compared the estimates with the actual healing of Death Strike taken from the combat log and saw differences up to 250K. And lastly, these weakauras are very inefficient in how they use LUA tables to store the recent damage taken events. So I decided to make this addon to fix all these problems and add some extra features on top.

### How to use
The addon loads automatically when you play a Blood Death Knight. You can configure it in the settings to load as Unholy or Frost if you want, but it only loads as Blood by default. The addon will show a Death Strike icon with the healing prediction for the next Death Strike. There are some options to configure how the information is presented in the Interface -&gt; AddOns menu. You can also add buffs or debuffs that affect Death Strike healing or edit the built-in values if you feel you need to do so for whatever reason.

### Slash commands
You can perform the following actions using the /deathstrikeprediction command, or the /dsp alias:

Toggle the prediction frame

```/deathstrikeprediction```

```/dsp```

Toggle the debug frame (useful for developers or to submit a bug report)

```/deathstrikeprediction debug```

```/dsp debug```

### How to contribute
To submit translations, you can either use the [CurseForge localization](https://www.curseforge.com/wow/addons/death-strike-prediction/localization "CurseForge localization") feature, submit an [issue on GitHub](https://github.com/Mailliw102/Death-Strike-Prediction/issues/new/choose "GitHub issues"), or submit a [pull request on GitHub](https://github.com/Mailliw102/Death-Strike-Prediction/pulls "GitHub pull requests"). To submit bug reports or feature requests, you can use the [CurseForge issues](https://www.curseforge.com/wow/addons/death-strike-prediction/issues/create "CurseForge issues") system or the [GitHub issues](https://github.com/Mailliw102/Death-Strike-Prediction/issues/new/choose "GitHub issues") system.

### Support
If you like this addon and would like to show your appreciation, consider making a donation, however small it may be. This is never necessary, but always appreciated. All my stuff is completely free to use, modify and redistribute however you want. I would just appreciate to get credit if you redistribute some of my work.

[![PayPal donation](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_donations&business=KFUY9AY9BGPXW&currency_code=CAD&source=url "PayPal donation")
