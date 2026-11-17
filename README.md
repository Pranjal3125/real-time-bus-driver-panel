<div align="center">

# Real-Time Bus Driver Panel

### Android driver app concept for GPS-based bus tracking

An Android application project exploring driver workflows, location updates, motion-based trip detection, and cloud-connected transport tracking.

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white) ![Android](https://img.shields.io/badge/Platform-Android-3DDC84?logo=android&logoColor=white) ![Jetpack Compose](https://img.shields.io/badge/UI-Jetpack%20Compose-4285F4?logo=jetpackcompose&logoColor=white)

[Source](https://github.com/Pranjal3125/real-time-bus-driver-panel) · [Issues](https://github.com/Pranjal3125/real-time-bus-driver-panel/issues)

</div>

> **Project note:** This repository contains an Android application and example AWS backend integration. A deployed production backend, security review, and real-world transport pilot are not established by this repository alone.

## Features described by the project

- Driver sign-in using an assigned Bus ID
- GPS-based location updates while tracking
- Motion-sensor-assisted trip start/stop detection
- Foreground service for background tracking
- Offline/demo workflow for development
- Cloud integration example using API Gateway, Lambda, and DynamoDB
- Material Design 3 interface built with Jetpack Compose

## Technology

| Area | Technologies |
|---|---|
| Android | Kotlin, Jetpack Compose, Android SDK |
| Location | Google Location APIs, Activity Recognition |
| Background work | Foreground Services |
| Networking | Retrofit, OkHttp |
| Local preferences | SharedPreferences (Room is noted as planned) |
| Example backend | AWS API Gateway, Lambda, DynamoDB |
| Authentication concept | JWT / Cognito |

## Getting started

1. Clone the repository.
2. Open the project in Android Studio.
3. Sync Gradle dependencies.
4. Configure a test API endpoint if connecting a backend.
5. Run on a compatible Android device with Google Play services.

```bash
git clone https://github.com/Pranjal3125/real-time-bus-driver-panel.git
cd real-time-bus-driver-panel
./gradlew assembleDebug
```

On Windows, use `gradlew.bat assembleDebug`.

## Backend configuration

The repository includes an example Lambda function and documents an AWS architecture using API Gateway and DynamoDB. Before connecting a real environment, deploy and test the backend independently, configure your own endpoint, use least-privilege IAM permissions, and configure authentication, authorization, validation, and monitoring. Never commit credentials, tokens, private endpoints, or personal location data.

Example API payloads are illustrative and do not establish a live backend deployment.

## Permissions and privacy

Location and activity-recognition permissions are sensitive. Request them only when needed, explain their purpose, and provide a way to stop tracking. Test background behavior and permission-denied paths on supported Android versions.

## Testing checklist

- Permission grant and denial flows
- Driver sign-in validation
- GPS accuracy and update behavior
- Background tracking and foreground notification
- Offline/online transitions
- API failures and retry behavior
- Battery usage and stop-tracking behavior

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Include device/Android version, reproduction steps, and relevant logs with bug reports.

## License

No license is currently declared. All rights are reserved by default; ask the repository owner before reusing or redistributing the code.
