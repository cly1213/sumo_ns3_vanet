# sumo_ns3_vanet
Softwares used:

ns-3.30

sumo 1.5.0 

OSM - Open street Map (osmWebWizard.py)

```bash

cd sumo/tools

python osmWebWizard.py

sumo -c osm.sumocfg --fcd-output trace.xml

cd sumo/tools

python traceExporter.py -i trace.xml --ns2mobility-output=mobility.tcl

cd ns-allinone-3.30/ns-3.30

./waf --run "scratch/ns2-mobility-trace --traceFile=/home/leo/mobility.tcl --nodeNum=1813 --duration=100.0 --logFile=ns2-mob.log"

cd netanim-3.108

./NetAnim 
```
## sumo
<img src="https://github.com/cly1213/sumo_ns3_vanet/blob/master/demo2.gif"/>

## ns3
<img src="https://github.com/cly1213/sumo_ns3_vanet/blob/master/test2.gif"/>


recording by https://github.com/phw/peek
