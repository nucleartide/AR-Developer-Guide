# ✨📱 The Developer's Guide to Augmented Reality (AR)

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
			<a href="#native-apps">Native mobile</a>
		</th>
		<td width="800">
			Good for adding AR to a standalone mobile app.<br /><br /><em>Examples: iOS, Android.</em>
		</td>
	</tr>
	<tr>
		<th width="200">
			<a href="#social">Social media</a>
		</th>
		<td width="800">
			Good if you're looking to create AR filters & effects for social media.<br /><br /><em>Examples: Facebook, Instagram, Snapchat.</em>
		</td>
	</tr>
	<tr>
		<th width="200">
			<a href="#mobile-web">Mobile web</a>
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
| [AR Kit](https://developer.apple.com/augmented-reality/) | iOS | Apple's first-party augmented reality SDK. iOS only. |
| [Unity](https://unity.com/) | Cross-platform engine | One of the two big players (the other being Unreal) in the 3D engine space. |
| [Unreal](https://www.unrealengine.com/) | Cross-platform engine | One of the two big players (the other being Unity) in the 3D engine space. |
| [Wikitude](https://www.wikitude.com/) | Cross-platform SDK | An augmented reality SDK. Requires a license. |
| [Vuforia](https://www.ptc.com/en/products/vuforia) | Cross-platform SDK | An augmented reality SDK. Requires a license. |
| [AR Foundation](https://docs.unity3d.com/Packages/com.unity.xr.arfoundation@4.1/manual/) | Cross-platform SDK | Unity's augmented reality SDK, that provides a uniform API across all XR platforms. You should use this if you're using Unity. |
| [AR Core](https://developers.google.com/ar) | Cross-platform SDK | Google's first-party augmented reality SDK. Supports iOS and Android. |
| [MRTK](https://github.com/microsoft/MixedRealityToolkit-Unity) | Cross-platform SDK | Microsoft's SDK for mixed reality applications. Unity only. |
| [ViroReact](https://viromedia.com/viroreact) | Cross-platform SDK | React Native wrapper for AR Kit and AR Core. Useful if you're using React Native. |
| [MARS](https://unity.com/products/unity-mars) | Cross-platform SDK | Unity's authoring environment for mixed reality applications. Expensive. |
| [OpenCV](https://opencv.org/) | Do-it-yourself library | The classic C++ library for computer vision. Useful if you're opting for a native, do-it-yourself approach. |
| [DLib](http://dlib.net/) | Do-it-yourself library | A C++ machine learning library. Containins image processing features that are useful if you're opting for a do-it-yourself approach. |

### Recommendation

If you're starting out, use **Unity** with **AR Foundation**.

AR Foundation delegates the actual augmented reality behavior to **AR Kit** and **AR Core**, so you're actually using Apple's and Google's tech under the hood.

To learn AR Foundation, I haven't found any good courses or tutorials. It seems most people just learn by playing with the official [arfoundation-samples](https://github.com/Unity-Technologies/arfoundation-samples) and [arfoundation-demos](https://github.com/Unity-Technologies/arfoundation-demos).

Also check out the `#augmented-reality` channel in the [Unity Discord](https://discord.com/invite/unity) for help.

<br />

## Social

### Tools

| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Technology&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Comment |
| --- | --- |
| Spark AR | Facebook's authoring tool for creating augmented reality content. Can only publish to Facebook or Instagram. |
| Lens Studio | Snapchat's authoring tool for creating augmented reality content. Can only publish to Snapchat. |
| Adobe Aero | Adobe's authoring tool for creating augmented reality content – kinda like Photoshop for AR. Unlike Spark AR or Lens Studio, exported Aero content isn't limited to a social media platform, but rather to iOS; it doesn't work on Android. |
| Reality Composer | Apple's first-party authoring tool for augmented reality content. Competitor to Adobe Aero. |

### Recommendation

If you know you want to create social media content, then choose either **Spark AR** for Facebook/Instagram, or **Lens Studio** for Snapchat.

Adobe Aero and Reality Composer are neat tools for iOS, and are worth investigating later in your AR journey – if only to learn about AR creation workflows.

<br />

## Mobile Web

### Tools

| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Technology&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Type | Comment |
| --- | --- | --- |
| Three.js | Free | The most widely known 3D library for JavaScript. |
| A-Frame | Free | A framework built atop Three.js. Has a friendlier, markup-driven approach to declaring the content of your 3D scene. |
| AR.js | Free | An augmented reality library in JavaScript. Not as feature rich as AR Core or AR Kit in native development, but still useful. |
| Mediapipe | Free | A machine learning library in JavaScript. Fills the gaps left by AR.js, and is worth a look if you need advanced AR features. |
| WebXR | Free | This is a web standard, not a specific tool. Useful to understand the concepts though. |
| Mozilla WebXR Viewer | Free | Mozilla's experimental web browser, containing a full-featured WebXR implementation. Useful for experimenting with WebXR, but not for production use. |
| [ARWT](https://github.com/ToughNutToCrack/ARWT) | Free | An open source library that allows you to author Web AR applications in Unity. |
| Babylon.js | Free | Another JavaScript-based game engine. |
| model-viewer | Free | A web component released by Google. Extremely useful if all you want is to view your 3D models in augmented reality. Uses Apple AR Quick Look and Android SceneViewer under the hood. |
| Apple AR Quick Look | Free | Apple's iOS-native method for displaying 3D models in augmented reality. |
| Android SceneViewer | Free | Google's Android-native method for displaying 3D models in augmented reality. |
| 8th Wall | Paid | The most-recommended solution for a paid Web AR SDK. Too expensive for beginning AR developers, but you should use if your job needs it. |
| Zappar | Paid | Another paid Web AR SDK. Cheaper than 8th Wall, and equally feature rich. |
| Blippar | Paid | Another paid Web AR SDK. |
| [AWE](https://awe.media/) | Paid | Another paid Web AR SDK. |
| Letsee | Paid | Another paid Web AR SDK. |
| PlayCanvas | Freemium | Another JavaScript-based game engine. |
| Sumerian | Freemium | Amazon's augmented reality offering. Useful if you want to interact heavily with AWS services. |
| Niantic Real World Platform | Early Access | Niantic's SDK offering. (Niantic is the company behind Pokemon Go.) Looks very promising, and worth checking out. Requires early access though. |

### Recommendation

The amount of choices is overwhelming here.

However, if you want to build AR content for mobile web, start with **A-Frame**. That'll give you the structure you need to start playing around.

From A-Frame, you can explore the ecosystem of JavaScript libraries (Three.js, AR.js, Mediapipe, WebXR concepts) as you need them.

On the other hand, if all you need is an AR model viewer for your e-commerce store, then look into Google's **model-viewer**, which uses **Apple AR Quick Look** and **Android SceneViewer** under the hood.

<br />

## Contribute

The AR tech landscape is constantly changing, so this list can't be exhaustive.

If I missed something, please open an issue or pull request!

<br />

## Who am I?

I'm a freelance developer focused on mobile AR. Check out my freelance portfolio at https://jasont.co/portfolio/.

If you're looking for dev help, drop me a line at `jasontu4@gmail.com`.
