# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.1.0] - 2018-11-14

### Added
- Allows the polling interval to be configured.
- Exposes the `ConnectivityDidChange` notification name as part of the public interface.

### Changed
- Enforces SSL by default.

## [1.0.0] - 2018-09-20
### Changed
- Updated for Xcode 10 and Swift 4.2.

## [0.0.4] - 2018-08-18
### Changed
- Fixed an issue whereby the callback could be invoked more frequently than necessary if using the polling option.

## [0.0.3] - 2018-08-18
### Added
- Adds a sample application to demonstrate how to use Connectivity.
### Changed
- Improvements to code structure and an early exit mechanism such that once the required number of successful connectivity checks has been met any pending checks will be cancelled as they will no longer affect the result.

## [0.0.2] - 2018-08-07
### Changed
- This release introduces support for Swift 4 and integration using the Carthage dependency manager. In order to integrate Connectivity into your project via Carthage, add the following line to your project's Cartfile:

	```
	github "rwbutler/Connectivity"
	```

## [0.0.1] - 2018-07-27
### Added
- Connectivity is a framework which improves on Reachability by allowing developers to detect whether true Internet connectivity is available or whether a captive portal is blocking Internet traffic.