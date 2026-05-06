This is a Kotlin Multiplatform project targeting Web.

/composeApp is for code that will be shared across your Compose Multiplatform applications. It contains several subfolders:
commonMain is for code that’s common for all targets.
Other folders are for Kotlin code that will be compiled for only the platform indicated in the folder name. For example, if you want to use Apple’s CoreCrypto for the iOS part of your Kotlin app, the iosMain folder would be the right place for such calls. Similarly, if you want to edit the Desktop (JVM) specific part, the jvmMain folder is the appropriate location.
Build and Run Web Application
To build and run the development version of the web app, use the run configuration from the run widget in your IDE's toolbar or run it directly from the terminal:

for the Wasm target (faster, modern browsers):
on macOS/Linux
./gradlew :composeApp:wasmJsBrowserDevelopmentRun
on Windows
.\gradlew.bat :composeApp:wasmJsBrowserDevelopmentRun
for the JS target (slower, supports older browsers):
on macOS/Linux
./gradlew :composeApp:jsBrowserDevelopmentRun
on Windows
.\gradlew.bat :composeApp:jsBrowserDevelopmentRun
Learn more about Kotlin Multiplatform, Compose Multiplatform, Kotlin/Wasm…

We would appreciate your feedback on Compose/Web and Kotlin/Wasm in the public Slack channel #compose-web. If you face any issues, please report them on YouTrack.