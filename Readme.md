# ✨📱 The Developer's Guide to Augmented Reality (AR) 📱✨

The AR ecosystem can be extremely intimidating for a beginner.

> _"There are so many tools... how do I choose? Where do I start?"_

☝️ If you've felt that way, then read on. This document is for you.

<br />

## First things first

<table>
	<tr>
	<td width="200">
	foo
	</td>
	<td width="500">
	bar
	</td>
	</tr>
</table>

Decide the platform that you want to develop for. Currently, there are 4:

| Platform                                                         | Notes |
| ---                                                              | --- |
| Native mobile                            | Good for adding AR to a standalone mobile app.<br />*Examples: iOS, Android.* |
| Social media            | Good if you're looking to create AR filters & effects for social media. *Examples: Facebook, Instagram, Snapchat.* |
| Mobile web                                                   | Good if you'd like your AR experience to be easily accessible, by not requiring an app install. |
| Wearables                       | Generally way too expensive, but good if you have an "enterprise" use case. *Examples: Magic Leap, Holo Lens.* |

The rest of this document will discuss tools and recommendations for the platforms above.

It will not discuss wearables, as I believe most beginning AR developers don't want to plop hundreds of dollars on an AR headset.

<br />

## Native apps

| Technology | Type | Comment
| --- | --- | --- |
| AR Kit | iOS | --- |
| AR Core | Android | --- |
| Unity | Cross-platform engine | --- |
| Unreal | Cross-platform engine | --- |
| React Native | Cross-platform engine | --- |
| Wikitude | Cross-platform SDK | --- |
| Vuforia | Cross-platform SDK | --- |
| AR Foundation | Cross-platform SDK | --- |
| MRTK | Cross-platform SDK | --- |
| ViroReact | Cross-platform SDK | --- |
| MARS | Cross-platform SDK | --- |
| OpenCV | Do-it-yourself library | --- |
| DLib | Do-it-yourself library | --- |

Recommendation: Use Unity with AR Foundation.

# Social

Recommendation: Choose your preferred platform if you want to make augmented reality content for Facebook, SNapchat, or Instagram.

- o Spark AR
- x Lens Studio
- x Adobe Aero - AR authoring tool. seems useful for artists.

# Web (free)

Recommendation: Start with A-Frame. Explore libraries (Three.js, AR.js, Mediapipe, WebXR, model-viewer) as you need them.

- Free
	- x A-Frame
		- x Three.js - library underlying a-frame.
		- x AR.js - more limited than native
		- x Mediapipe - augmented features.
		- x WebXR - this is a spec underlying frameworks, not the framework
	- x Mozilla WebXR Viewer - interesting for experimenting with webxr, but not for production use: https://immersive-technology.com/mixedreality/ios-gets-mozillas-firefox-based-webxr-viewer-app/
	- x ARWT (author in Unity) - looks promising, but prefer something more popular.
	- x Babylon.js - prefer aframe
	- model-viewer - used for simple model viewing on a website.
		- iOS: Apple AR Quick Look
		- Android: SceneViewer
- Paid, Freemium, Proprietary
	- x Zappar
	- x 8th Wall
	- x Blippar
	- x PlayCanvas (free tier)
	- x https://awe.media/
	- x Letsee
	- x Sumerian
	- x Niantic Real World Platform - if you want to make Geomobile
