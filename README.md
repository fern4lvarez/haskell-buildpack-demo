# Haskell Buildpack Demo

This demo is live on cloudControl:

http://haskelldemo.cloudcontrolled.com

It uses the Haskell Buildpack:

https://github.com/fern4lvarez/buildpack-haskell

## Pushing & deploying to cloudControl

Clone this repository:

    git clone https://github.com/fern4lvarez/haskell-buildpack-demo.git

Create a new cloudControl application:

    cctrlapp APP_NAME create custom --buildpack https://github.com/fern4lvarez/buildpack-haskell.git

Ship it!

    cctrlapp APP_NAME/default push --ship

*Note*: the push will take some time to install dependencies and might
not show any output for quite a while. It will also show a lot of
warnings.
