---
title: How to Use NSDateFormatter and NSNumberFormatter when we our app does not support localisation
tip-number: 03
tip-username: yogesh
tip-username-profile: https://github.com/Yogesh-MV
tip-description: When our app support does not support localisation (Consider our app support only in english). Then we have to set localeIdentifier for NSDateFormatter and NSNumberFormatter. Otherwise the formatted string will be display in device locale language. This will cause some failure in our app.

#####To set english as a default for your app use the below code:
`NSLocale *locale = [NSLocale localeWithLocaleIdentifier:@"en"];`

---
#### Test Force Tocuh by using -[SBShortcutMenuSimulator](https://github.com/DeskConnect/SBShortcutMenuSimulator)

####Note:
If the testing is not working fine in simulator. Try resetting the simulator.
