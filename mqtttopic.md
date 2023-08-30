## How do you design MQTT topics and payloads for smart washing machine

1. สถานะเครื่องซักผ้า
    - topic:v1cdti/hw/get/6310301021/model-01/sn-001/
    - payload
        - {"STATUS": "POWER ON|START|WASHING|DRYING|STOP|FINISHED|STANDBY|POWERED OFF"}
1. เซนเซอร์ภายในเครื่องซักผ้า
    - topic:v1cdti/hw/get/6310301021/model-01/sn-001
    - payload
        - {"temperature": "25.2"}
        - {"humidity": "50"}
        - {"lid-status": "open|close|lock"}
        - {"current-measure": "120"}
        - {"vibration": "10"}
        - {"imbalance": "yes|no"}
        - {"air-flow": "30.5"}
        - {"pressure": "1.2"}
        - {"UV-C": "on|off"}
        - {"hall-speed": "value"}
        - {"motor-sound": "20"}
        - {"speed": "136.2"}
        - {"direction": "clockwise|counter-clockwise"}
        - {"weight": "15"}
        - {"detergent-level": "0.3"} 
        - {"foam-level": "50"} 
        - {"water-level": "10"}
        - {"inlet-valve": "0|0.6|1.3"}
        - {"drain-valve": "0|0.5|1"}
        - {"material": "fabric"}
        - {"air-quality": "10"}
        - {"CO2": "15"}
        

 1. เซนเซอร์ภายนอกเครื่องซักผ้า
    - topic:v1cdti/hw/get/6310301021/model-01/sn-001
    - payload
        - {"human-presence": "yes|no"}
        - {"gesture": "hand-show|press|hover|slice-left|slice-right|slice-up|slice-down|pull-bar"}
        - {"user": "adult|children"}
        - {"animal-presence": "yes|no"}
        - {"voice-detection": "10"} // value of signal
        - {"people-count": "2"}
        - {"temp-outdoor": "15"}
        - {"humid-outdoor": "60"}
        - {"pressure-outdoor": "1"}
        - {"weather-predict": "good"}


