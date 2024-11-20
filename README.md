# Radz ExoPlayer
[![](https://jitpack.io/v/Radzdevteam/RadzExoPlayer.svg)](https://jitpack.io/#Radzdevteam/RadzExoPlayer)

Radz ExoPlayer is a media player library developed by Radz, leveraging the powerful ExoPlayer framework.

## Player Supported Formats:
- HLS (HTTP Live Streaming)
- M3U8
- MP4
- TS
- DASH (Dynamic Adaptive Streaming over HTTP)
- TLS (Transport Layer Security)

## How to Include
### Step 1. Add the repository to your project settings.gradle:
```groovy
dependencyResolutionManagement {
    repositoriesMode.set(RepositoriesMode.FAIL_ON_PROJECT_REPOS)
    repositories {
        google()
        mavenCentral()
        maven { url = uri("https://jitpack.io") }
    }
}
   ```

### Step 2. Add the dependency
```groovy
dependencies {
    implementation ("com.github.Radzdevteam:radzweb:1.0")
}

   ```

## Usage

In your `MainActivity`, add the following code:
```groovy
class MainActivity : ComponentActivity() {

    override fun onCreate(savedInstanceState: Bundle?) {
        super.onCreate(savedInstanceState)

        val intent = Intent(this, radzweb::class.java)
        intent.putExtra("url", "https://google.com/")
        startActivity(intent)
        finish()
    }
}

   ```



   ```

## Manifest
In your `AndroidManifest`, add the following code:
```groovy
<activity android:name="com.radzdev.radzweb.radzweb"
android:configChanges="keyboard|keyboardHidden|orientation|screenSize|screenLayout|smallestScreenSize|uiMode"/>
   ```
