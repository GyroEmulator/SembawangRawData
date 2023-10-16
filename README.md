# SembawangRawData
Pertainent data to a gravitaitonal survey, performed in Sembawang, Singapore.

The absolute gravimeter readings are in the files with the naming convention FluorescentRatio_XYZ... : the timestamp is the beggining of the data capturing.
Each gravity measurement is a sequence of 100 points:
i) The timestep between each data point is 2.5s.
ii) Even numbered points are subject to -k polarization, odd numbered points to +k polarization. 
ii) The intial fringe frequency is f0 = 25.0706916 MHz, and increases by df=1.52Hz every 2 data points.

The relative gravity data is found in "CG445-day1.txt" and "CG445-day2.txt". Columns 2-3 indicate the date and time of the measurement, column 4 indicates the raw gravity value, columns 11-14 indicate internal gravity corrections (tide, tilt, temperature, drift). The relative GPS files include nmea messages (GGA and GST).

Lastly, the file "TidalCorrections" is generated through software to more accurately filter out tidal phenomena. Thus, the internal tidal corrections indicated by the CG445 are subtracted, and the improved corrections from the software are added.
