## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|STOP|FINISHED|POWERED OFF"}
1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001
    - payload
        - {"Temperature": "25.2"}
        - {"Water level": "10"}
        - {"Drain pump": "100"}
        - {"Energy efficiency": "2000"}
        - {"Position": "90"}
        - {"Low acoustic noise": "10"}
        - {"Saving water": "10"}
        - {"UV-C": "100"}
        - {"Hall": "open/close"}
        

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/app/get/1212312121/model-01/sn-001
    - payload
        - {"Determine open/close": "door"}
        - {"Touch screens": "Touch Water level"}
        - {"acoustic noise": "10"}
        - {"Voice sensors": "Voice level"}
        - {"Temperature": "10"}
        - {"Humidity": "10"}
        - {"Radar: "1"}



