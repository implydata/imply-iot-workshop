# Data Simulator + AWS IoT Core + Kinesis 





## Device Sensor Schema

**evSensor**

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
