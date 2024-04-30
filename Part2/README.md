# Data Simulator + AWS IoT Core + Kinesis 


![AWS Stack + Imply Polaris](https://github.com/implydata/imply-iot-workshop/blob/main/Part2/Iot%2BImply.png "AWS Stack + Imply Polaris")



## Device Sensor Schema

**evSensor**  [Sample Payload](/Part2/evSensor.json) 

colName| dataType| description  
|---|---|---|
|_type|string|type of event|  
|_event_timing|int|event occurrence observed time in seconds|   
|_seq|int|sequence number| 
|torque_available_motoring|float|ideal torque at temperature|  
|updated|bool|  |  
|torque_available_regen|float|torque regenerated|  
|tenant|string|electric vehicle make|  
|_type|string|type of sensor data emitted|  
|fleet|array|vehicle type in fleet|  
|car_ownership_id|int|owner id|  
|eventTimestamp|timestamp|event occurrence timestamp|  
|temperature_IGBT_A|float|inverter temperature type A|  
|temperature_IGBT_B|float|inverter temperature type B|  
|temperature_IGBT_C|float|inverter temperature type C|  
|motor_temperature|string|motor temperature recorded|  
|torque_achieved|string|torque achieved at the time|  
|fault_properties|complex<JSON>|fault sensor data|  
  |fault_status|bool|fault status|  
  |fault_type|array|fault code|  
|charging_properties|complex<JSON>|charging stats|  
  |charge_time|bool|total charging time|  
  |total_charge_energy_added|array|energy added, in kwH|  
  |charge_location|spatial|Lat and Long data of charging|  
|_subtype|array|subtype of sensor data emitted|  
|VIN|string|vehicle VIN|  



*Quick links :*
[Home](/README.md) - [Part 1](/Part1/README.md) - [Part 2](/Part2/README.md) - [Part 3](/Part3/README.md) - [Part 4](/Part4/README.md)
