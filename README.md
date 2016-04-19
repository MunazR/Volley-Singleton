# Volley Singleton [ ![Download](https://api.bintray.com/packages/munazr/maven/volley-singleton/images/download.svg) ](https://bintray.com/munazr/maven/volley-singleton/_latestVersion)
Android library for a singleton instance of volley

## Installation
Add the following to your gradle build
```
repositories {
    maven {
        url 'https://dl.bintray.com/munazr/maven/'
    }
}

dependencies {
    compile 'com.munaz.volleysingleton:volleysingleton:1.0.0'
}
```

Or clone this repository, add it as a module in your app and add following to your gradle build
```
dependencies {
    compile project(':volleysingleton')
}
```

## Usage
To add requests to the queue, generate a volley request and tuse the following
```
VolleySingleton.getInstance(getApplicationContext()).addToRequestQueue(myRequest);
```
The context only needs to be passed in once during the application lifecycle to initialize the singleton.

For more on creating requests click [here](http://developer.android.com/training/volley/index.html).

## License

The MIT License (MIT)

Copyright (c) 2016 Munaz

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
