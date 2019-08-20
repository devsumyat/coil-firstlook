# coil-firstlook
This is coil first experience project.

![architecture](https://github.com/devsumyat/coil-firstlook/blob/master/38dk89.gif)

# Requirements
* AndroidX
* Min SDK 14+
* Compile SDK: 28+
* Java 8+

# Download
Gradle: 
implementation 'io.coil-kt:coil:0.6.1'

# Quick Start
* basic usage 

// in Glide
Glide.with(context)
    .load(url)
    .into(imageView)

// in Picasso
Picasso.get()
    .load(url)
    .into(imageView)

// in Coil
-> imageView.load(url)
* custom request

// in Glide
Glide.with(context)
    .load(url)
    .placeholder(placeholder)
    .fitCenter()
    .into(imageView)

// in Picasso
Picasso.get()
    .load(url)
    .placeholder(placeholder)
    .fit()
    .into(imageView)

// in Coil (autodetects the scale type)
-> imageView.load(url) {
    placeholder(placeholder)
}
