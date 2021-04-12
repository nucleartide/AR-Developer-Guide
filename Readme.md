# ✨📱 The Developer's Guide to Augmented Reality (AR) 📱✨

The AR ecosystem can be extremely intimidating for a beginner.

> _"There are so many tools... how do I choose? Where do I start?"_

☝️ If you've felt that way, then read on. This document is for you.

<br />

## First things first

Decide the platform that you want to develop for. Currently, there are 4:

<table>
	<tr>
		<th width="200">
			Platform
		</th>
		<th width="800">
			Notes
		</th>
	</tr>
	<tr>
		<th width="200">
			Native mobile
		</th>
		<td width="800">
			Good for adding AR to a standalone mobile app.<br /><br /><em>Examples: iOS, Android.</em>
		</td>
	</tr>
	<tr>
		<th width="200">
			Social media
		</th>
		<td width="800">
			Good if you're looking to create AR filters & effects for social media.<br /><br /><em>Examples: Facebook, Instagram, Snapchat.</em>
		</td>
	</tr>
	<tr>
		<th width="200">
			Mobile web
		</th>
		<td width="800">
			Good if you'd like your AR experience to be easily accessible, by not requiring an app install.
		</td>
	</tr>
	<tr>
		<th width="200">
			Wearables
		</th>
		<td width="800">
			Generally way too expensive, but good if you have an "enterprise" use case.<br /><br /><em>Examples: Magic Leap, Holo Lens.</em>
		</td>
	</tr>
</table>

The rest of this document will discuss tools and recommendations for the platforms above.

It will not discuss wearables, as I believe most beginning AR developers don't want to plop hundreds of dollars on an AR headset.

<br />

## Native apps

### Tools

| &nbsp;&nbsp;&nbsp;Technology&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Type&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Comment
| --- | --- | --- |
| AR Kit | iOS | Apple's first-party augmented reality SDK. iOS only. |
| Unity | Cross-platform engine | One of the two big players (the other being Unreal) in the 3D engine space. |
| Unreal | Cross-platform engine | One of the two big players (the other being Unity) in the 3D engine space. |
| Wikitude | Cross-platform SDK | An augmented reality SDK. Requires a license. |
| Vuforia | Cross-platform SDK | An augmented reality SDK. Requires a license. |
| AR Foundation | Cross-platform SDK | Unity's augmented reality SDK, that provides a uniform API across all XR platforms. You should use this if you're using Unity. |
| AR Core | Cross-platform SDK | Google's first-party augmented reality SDK. Supports iOS and Android. |
| MRTK | Cross-platform SDK | Microsoft's SDK for mixed reality applications. Unity only. |
| ViroReact | Cross-platform SDK | React Native wrapper for AR Kit and AR Core. Useful if you're using React Native. |
| MARS | Cross-platform SDK | Unity's authoring environment for mixed reality applications. Expensive. |
| OpenCV | Do-it-yourself library | The classic C++ library for computer vision. Useful if you're opting for a native, do-it-yourself approach. |
| DLib | Do-it-yourself library | A C++ machine learning library. Containins image processing features that are useful if you're opting for a do-it-yourself approach. |

### Recommendation

If you're starting out, use **Unity** with **AR Foundation**.

AR Foundation delegates the actual augmented reality behavior to **AR Kit** and **AR Core**, so you're actually using Apple's and Google's tech under the hood.

To learn AR Foundation, I haven't found any good courses or tutorials. It seems most people just learn by playing with the official [arfoundation-samples](https://github.com/Unity-Technologies/arfoundation-samples) and [arfoundation-demos](https://github.com/Unity-Technologies/arfoundation-demos).

Also check out the #augmented-reality channel in the [Unity Discord](https://discord.com/invite/unity) for help.

<br />

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
