# GarminFileConvert

load Garmin TCX/GPX/CSV files and save as Golden Cheetah json.

## File Formats
### TCX
<Activities>
    <Activity Sport="Biking">
      <Id>2017-02-19T11:14:46.000Z</Id>
      <Lap StartTime="2017-02-19T11:14:46.000Z">
        <TotalTimeSeconds>637.0</TotalTimeSeconds>
        <DistanceMeters>5000.0</DistanceMeters>
        <MaximumSpeed>9.069000244140625</MaximumSpeed>
        <Calories>116</Calories>
        <AverageHeartRateBpm>
          <Value>150</Value>
        </AverageHeartRateBpm>
        <MaximumHeartRateBpm>
          <Value>168</Value>
        </MaximumHeartRateBpm>
        <Intensity>Active</Intensity>
        <Cadence>101</Cadence>
        <TriggerMethod>Manual</TriggerMethod>
        <Track>
          <Trackpoint>
            <Time>2017-02-19T11:14:46.000Z</Time>
            <AltitudeMeters>508.79998779296875</AltitudeMeters>
            <DistanceMeters>5.539999961853027</DistanceMeters>
            <HeartRateBpm>
              <Value>103</Value>
            </HeartRateBpm>
            <Cadence>78</Cadence>
            <Extensions>
              <ns3:TPX>
                <ns3:Speed>5.541999816894531</ns3:Speed>
              </ns3:TPX>
            </Extensions>
          </Trackpoint>
          <Trackpoint>
            <Time>2017-02-19T11:14:47.000Z</Time>
            <AltitudeMeters>508.79998779296875</AltitudeMeters>
            <DistanceMeters>11.170000076293945</DistanceMeters>
            <HeartRateBpm>
              <Value>105</Value>
            </HeartRateBpm>
            <Cadence>78</Cadence>
            <Extensions>
              <ns3:TPX>
                <ns3:Speed>5.625999927520752</ns3:Speed>
              </ns3:TPX>
            </Extensions>
          </Trackpoint>
          ...
          ...
        <Creator xsi:type="Device_t">
        <Name>fenix 3</Name>
        <UnitId>ID</UnitId>
        <ProductID>2050</ProductID>
        <Version>
          <VersionMajor>8</VersionMajor>
          <VersionMinor>8</VersionMinor>
          <BuildMajor>0</BuildMajor>
          <BuildMinor>0</BuildMinor>
        </Version>
      </Creator>
    </Activity>
  </Activities>
  <Author xsi:type="Application_t">
    <Name>Garmin Connect API</Name>
    <Build>
      <Version>
        <VersionMajor>17</VersionMajor>
        <VersionMinor>4</VersionMinor>
        <BuildMajor>0</BuildMajor>
        <BuildMinor>0</BuildMinor>
      </Version>
    </Build>
    <LangID>en</LangID>
    <PartNumber>xxxxxxx</PartNumber>
  </Author>
</TrainingCenterDatabase>

### CSV


### JSON

{
	"RIDE":{
		"STARTTIME":"2016\/02\/05 22:13:03 UTC ",
		"RECINTSECS":1,
		"DEVICETYPE":"GoldenCheetah ",
		"IDENTIFIER":" ",
		"TAGS":{
			"Athlete":"Athlete Name ",
			"Calendar Text":"\nIndoor\n\n\n\n\n\n ",
			"Change History":"Changes on Sun Jun 26 12:01:58 2016:\n ",
			"Data":"TDSPHC-----E--- ",
			"Device":"GoldenCheetah ",
			"File Format":" ",
			"Filename":"2016_02_05_23_13_03.json ",
			"Month":"February ",
			"Source Filename":"2016_02_05_23_12_58_2016_02_05_23_13_03.csv ",
			"Weekday":"Fri ",
			"Workout Code":"Indoor ",
			"Year":"2016 "
		},
		"SAMPLES":[
			{ "SECS":0, "KM":0, "WATTS":0, "CAD":0, "KPH":0, "HR":0, "TEMP":0 },
			...
            { "SECS":15, "KM":1.39933e-05, "WATTS":0, "CAD":0, "KPH":0.25188, "HR":78, "TEMP":0 },
			{ "SECS":16, "KM":5.59733e-05, "WATTS":21, "CAD":0, "KPH":6.17106, "HR":81, "TEMP":0 },
			{ "SECS":17, "KM":0.00177016, "WATTS":26, "CAD":0, "KPH":7.43046, "HR":82, "TEMP":0 },
			{ "SECS":18, "KM":0.00389714, "WATTS":30, "CAD":0, "KPH":8.56392, "HR":85, "TEMP":0 },
            ...
		]
	}
}

