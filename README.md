<div align="center">

# Real-Time Bus Driver Panel

### Android Driver App for GPS-Based Public Transport Tracking

An Android application built with Kotlin and Jetpack Compose for bus driver workflows, real-time GPS location updates, motion-assisted trip detection, and AWS cloud integration.

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Platform-Android-3DDC84?logo=android&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/UI-Jetpack%20Compose-4285F4?logo=jetpackcompose&logoColor=white)
![AWS](https://img.shields.io/badge/Backend-AWS-232F3E?logo=amazonwebservices&logoColor=white)

[Source](https://github.com/Pranjal3125/real-time-bus-driver-panel) · [Issues](https://github.com/Pranjal3125/real-time-bus-driver-panel/issues)

</div>

> **Note:** Includes the Android client application and an example AWS serverless backend architecture (API Gateway, Lambda, DynamoDB) for development and testing.

## Features

- Driver sign-in using an assigned Bus ID
- Real-time GPS location updates while tracking
- Motion-sensor-assisted trip start/stop detection
- Foreground service for reliable background location tracking
- Offline/demo workflow for local development
- Example cloud backend using AWS API Gateway, Lambda, and DynamoDB
- Material Design 3 interface built with Jetpack Compose

## Tech Stack

| Area | Technologies |
|---|---|
| Android | Kotlin, Jetpack Compose, Android SDK |
| Location | Google Location APIs, Activity Recognition |
| Background Work | Foreground Services |
| Networking | Retrofit, OkHttp |
| Local Storage | SharedPreferences *(Room planned)* |
| Example Backend | AWS API Gateway, Lambda, DynamoDB |
| Auth Concept | JWT / Amazon Cognito |

## Getting Started

1. Clone the repository and open it in **Android Studio**.
2. Sync Gradle dependencies.
3. Configure a test API endpoint if connecting to a backend.
4. Run on an Android device with Google Play Services.

```bash
git clone https://github.com/Pranjal3125/real-time-bus-driver-panel.git
cd real-time-bus-driver-panel
./gradlew assembleDebug
```

On Windows, run `gradlew.bat assembleDebug`.

## Backend Configuration

This repository includes an example Lambda function and AWS architecture using API Gateway and DynamoDB. Before connecting a live environment:

- Deploy and test your backend independently and configure your own API endpoint.
- Use least-privilege IAM permissions, authentication/authorization, input validation, and monitoring.
- Never commit credentials, tokens, private endpoints, or personal location data.

## Permissions & Privacy

Location and activity-recognition permissions are sensitive. Request them only when needed, explain their purpose clearly to drivers, and provide an explicit control to stop tracking.

## Testing Checklist

- [ ] Permission grant and denial flows
- [ ] Driver sign-in validation
- [ ] GPS accuracy and update intervals
- [ ] Background tracking and foreground notification
- [ ] Offline/online network transitions
- [ ] API failures and retry behavior
- [ ] Battery usage and stop-tracking cleanup

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md). Include device model, Android version, reproduction steps, and logs with bug reports.

## License

All rights reserved. Contact the repository owner before reusing or redistributing this code.
