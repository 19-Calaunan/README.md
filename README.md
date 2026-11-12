Vernice Ilithyia N. Calaunan
9-Arayat

Sample Codes:
https://github.com/19-Calaunan/-CS3-Code-Portfolio/blob/main/q1/Tusok-tusok
https://github.com/19-Calaunan/-CS3-Code-Portfolio/blob/main/q1/q1_2030_arayat_calaunan.py

FAS:

https://github.com/19-Calaunan/-CS3-Code-Portfolio/blob/main/q1/q1_sq2_a1.md

https://github.com/19-Calaunan/-CS3-Code-Portfolio/blob/main/q1/q1_sg2_a2.md

https://github.com/19-Calaunan/-CS3-Code-Portfolio/blob/main/q1/q1_sg2_a3.py

https://github.com/19-Calaunan/-CS3-Code-Portfolio/blob/main/q1/FA4_Arayat_Calaunan_Canto_Magtoto.png

https://github.com/19-Calaunan/-CS3-Code-Portfolio/blob/main/q1/q1_sg5_a1_arayat_calaunan.py

https://github.com/19-Calaunan/-CS3-Code-Portfolio/blob/main/q1/q1_sg6_arayat_calaunan.py

https:// github.com/19-Calaunan/-CS3-Code-Portfolio/blob/main/q1/q1_sg7_arayat_calaunan.py
from abc import ABC, abstractmethod

class Sensor(ABC):

    @abstractmethod
    def get_reading(self):
        pass


class PHSensor(Sensor):

    def get_reading(self):
        return "7.2 pH (Neutral)"


class TempSensor(Sensor):

    def get_reading(self):
        return "24.5°C"


print("--- Lab Inventory System ---")

ph_sensor = PHSensor()
temp_sensor = TempSensor()

print("[pH Sensor] Reading:", ph_sensor.get_reading())
print("[Temperature Sensor] Reading:", temp_sensor.get_reading())
