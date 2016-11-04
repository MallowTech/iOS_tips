---
title: Checking whether app is running on simulator or ios device.
tip-number: 05
tip-username: karthironald
tip-username-profile: https://github.com/karthironald
tip-description: The camera and mail like app in ios will not run in simulator, if you try to run in simulator means then it will get crash. So this tip will help you to find whether the app is running in **simulator** or **ios device** to save your valuable developing time.


---

####CODE:
Add this following code in your project to find whether the app is running simulator or ios device,

	#if (arch(i386) || arch(x86_64)) && os(iOS)
		let IS_SIMULATOR = true
	#else
		let IS_SIMULATOR = false
	#endif 	