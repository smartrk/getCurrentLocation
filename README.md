![ezgif com-gif-maker (1)](https://user-images.githubusercontent.com/20436225/161189495-c4b0bbc7-621a-4caa-af53-b83d54e277c8.gif)


# Android Location Manager
## 
# Get Current location with one tap
- Auto handle location permissions
- Auto handle gps permision


## Code Sample 
 ```sh
   LocationUtils.init(this)
   
      LocationUtils.getCurrentLocation(object : LocationCallBack {
                override fun callBack(location: Location) {
                    // location updates
                }

                override fun gpsRequestDeniedCallBack() {
		   // do something
                }

                override fun permissionRequestDeniedCallBack() {
                  // do something
		}
            })
```





## Gradle dependency

```sh
allprojects {
		repositories {
			maven { url 'https://jitpack.io' }
		}
	}
```

```sh
dependencies { 
        implementation 'com.github.smartrk:getCurrentLocation:1.0.0' 
}
```

