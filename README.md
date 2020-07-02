# Introduce

&ensp;&ensp;This project mainly stores the weather data collected by my private meteorological station. Publicly available data can be used for research and machine learning. The meteorological station is located in China (113.87362, 23.121406). The device operation records started from February 3, 2019, including wind direction, wind speed, temperature, humidity, PM1.0, PM2.5 and PM10

# Logs
All log data is named after a time text file.

> Data before May 1, 2019 May be inaccurate due to device debugging


Record Format: 

`2020-05-18T22:21:14 A1151B180C0000D0000E0000F0013G0000H0000I0000J0000K0000L0298M716N10044,028,041,048,024,036,047,*07`

> The data before 2020-05-18 22:21:14 has no data of standard particulate matter, so the format is like this:
>
> `2019-02-03T19:02:39 A1866B045C0000D0000E0000F0003G0000H0000I0000J0000K0000L0258M608N10167*2C`

Date:`2020-05-18T22:21:14`

AD value (0-4095) was measured in real time by wind direction: `A1151`

The wind:`B180`

Real-time wind speed frequency (1Hz): `C0000`

Real-time wind speed (0.1m /S): `D0000`

Average wind speed in the 1 minute (0.1m/s): `E0000`

Maximum wind speed in the Before 5 minutes (0.1m/s): `F0013`

Real-time number of bucket rain gauges: `G0000`

Number of bucket rain gauges in the before 1 minute: `H0000`

Rainfall in the before 1 minute (0.1mm): `I0000`

Rainfall in the before 1 hours (0.1mm): `J0000`

Rainfall in the before 24 hours (0.1mm): `K0000`

Temperature (Celsius): `L0298`

Humidity (0.1) (0%-99%): `M716`

Air pressure (0.1HPa): `N10044`

Concentration of PM1.0 (CF=1, standard particulate matter, μg/m³)：`,028`

Concentration of PM2.5 (CF=1, standard particulate matter, μg/m³)：`,041`

Concentration of PM10 (CF=1, standard particulate matter, μg/m³)：`,048`

Concentration of PM1.0 (Atmospheric environment, μg/m³)：`,024`

Concentration of PM2.5 (Atmospheric environment, μg/m³)：`,036`

Concentration of PM10 (Atmospheric environment, μg/m³)：`,047`

Checksum, between A and * (excluding *) all characters xor results: `*07`
