# signalk-speed-wind-averaging
SignalK plugin to calculate average boat speed and wind speed over a defined period.  The plugin receives boat speed and wind speed deltas every seconds and calculates running averages from that data.

The plugin calculates the following values:

- The running average boat speed
- The boat speed averaged over the last 10 seconds
- The maximum 10 second boat speed recorded
- The running average wind speed
- The wind speed averaged over the last 10 seconds
- The maximum 10 second wind speed recorded

The following properties can be set in the plugin's configuration screen:

- The period over which to average (10 seconds by default)
- The SignalK paths from which to read the current boat speed and wind speed
- The SignalK paths which are written to with the calculated values

To reset the running averages for boat speed and wind speed you can call the following handler:

`/self/reset`