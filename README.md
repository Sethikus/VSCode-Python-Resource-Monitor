# Python Resource Monitor

Until now, resource and performance monitor extensions in VS Code only displayed current global resource consumption data via lists and text. Likewise, it is very awkward to use third-party tools to find the process you want to monitor.

However, this extension provides an easier, graphical solution that can show data specific to the process being used by the Python debugger! *Yeah, so I made this because searching for the right python process in task manager was annoying*

## Features
Provides a resource monitor that is opened when debugging Python, including process memory and cpu usage. Automatically launches (or reuses existing tab) upon debugging with Python.

![usage](images/usage.gif)

*Test program storing strings of random sizes in memory*

| Command | Usage |
| ------- | ----- |
| `PyRSM: Length` | Set the maximum log length in milliseconds of the resource monitor. Set to `0` to allow unlimited length (time display will scale). |
| `PyRSM: Polling Interval` | Set the time between datapoints in milliseconds. |

## Known Issues and Future Updates

- Hopefully, this will one day work for many languages and debuggers!
- Not tested on MacOS.
- I don't think it will work with the Python multiprocessing module quite yet.

## Recent Major Updates
### 0.0.1
First Release! All the basics seem to work.

### 0.0.2
Added icon and more details.

### 0.1.0
Millisecond-accuracy for CPU usage. When writing the module, tested with Linux.