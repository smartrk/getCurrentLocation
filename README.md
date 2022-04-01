![ezgif com-gif-maker (1)](https://user-images.githubusercontent.com/20436225/161188828-6c71ff44-eccf-4c60-9c8d-4c6c35948b60.mp4)


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

