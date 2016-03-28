
All icons from http://google.github.io/material-design-icons/




## From react native documentation

### Static Image Resources

As of 0.14 release, React Native provides a unified way of managing images in your iOS and Android apps. To add a static image to your app, place it somewhere in your source code tree and reference it like this:


	<Image source={require('./my-icon.png')} />


The image name is resolved the same way JS modules are resolved. In the example above the packager will look for my-icon.png in the same folder as the component that requires it. Also if you have my-icon.ios.png and my-icon.android.png, the packager will pick the file depending on the platform you are running on.

You can also use @2x, @3x, etc. suffix in the file name to provide images for different screen densities. For example, if you have the following file structure:

	.
	├── button.js
	└── img
		├── check@2x.png
		└── check@3x.png

