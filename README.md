It's impossible to build relocatable toolchain using crosstool-ng on Mac OS X due to lack of "-static" option which ct-ng heavily relies on.

Instead, I've updated Homebrew's crosstool-ng. Please install it and follow the caveats.
Then creating toolchain should be as simple as:

	ct-ng armv6-rpi-linux-gnueabi
	ct-ng build
