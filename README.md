![ezgif com-gif-maker (1)](https://user-images.githubusercontent.com/20436225/161189296-ddcf0ba9-de7b-4abf-8f66-ef8bf6ff8752.gif)


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

