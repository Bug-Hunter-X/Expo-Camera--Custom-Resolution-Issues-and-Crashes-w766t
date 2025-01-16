# Expo Camera Custom Resolution Bug

This repository demonstrates a bug encountered when using custom resolutions with the Expo Camera API.  Setting resolutions that don't align perfectly with the camera's sensor capabilities can result in crashes or distorted images. The `bug.js` file shows the problematic code, while `bugSolution.js` offers a solution.

## Problem

The Expo Camera API, while flexible, can be problematic when resolutions are not properly aligned with hardware constraints. This can lead to undefined behavior, including application crashes or images with unexpected distortion.

## Solution

The provided solution focuses on carefully selecting resolutions that are compatible with the camera sensor.  If the specific resolution is crucial, it is highly recommended to thoroughly test it on the target devices.  It might be also useful to handle potential errors more gracefully, providing feedback to the user in case of incompatibility.

## Reproduction Steps

1. Clone this repository.
2. Install dependencies using `npm install`.
3. Run the app using `expo start`.
4. Try capturing images with the custom resolution specified in `bug.js`. Observe the crashes or image distortion.
5. Replace `bug.js` with `bugSolution.js` to observe improved stability. 

Note: This issue is device-specific, so the effect might vary across different devices. 