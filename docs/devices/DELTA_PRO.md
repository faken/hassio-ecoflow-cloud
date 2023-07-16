## DELTA_PRO

*Sensors*
- Main Battery Level (`pd.soc`)
- Total In Power (`pd.wattsInSum`)
- Total Out Power (`pd.wattsOutSum`)
- AC In Power (`inv.inputWatts`)
- Solar In Power (`mppt.inWatts`)
- AC Out Power (`inv.outputWatts`)
- DC Out Power (`mppt.outWatts`)
- DC Car Out Power (`mppt.carOutWatts`)
- DC Anderson Out Power (`mppt.dcdc12vWatts`)
- Type-C (1) Out Power (`pd.typec1Watts`)
- Type-C (2) Out Power (`pd.typec2Watts`)
- USB (1) Out Power (`pd.usb1Watts`)
- USB (2) Out Power (`pd.usb2Watts`)
- USB QC (1) Out Power (`pd.qcUsb1Watts`)
- USB QC (2) Out Power (`pd.qcUsb2Watts`)
- Charge Remaining Time (`ems.chgRemainTime`)
- Discharge Remaining Time (`ems.dsgRemainTime`)
- Cycles (`bmsMaster.cycles`)
- Battery Temperature (`bmsMaster.temp`)
- Min Cell Temperature (`bmsMaster.minCellTemp`)   _(disabled)_
- Max Cell Temperature (`bmsMaster.maxCellTemp`)   _(disabled)_
- Battery Volts (`bmsMaster.vol`)   _(disabled)_
- Min Cell Volts (`bmsMaster.minCellVol`)   _(disabled)_
- Max Cell Volts (`bmsMaster.maxCellVol`)   _(disabled)_
- Solar In Energy (`pd.chgSunPower`)
- Battery Charge Energy from AC (`pd.chgPowerAc`)
- Battery Charge Energy from DC (`pd.chgPowerDc`)
- Battery Discharge Energy to AC (`pd.dsgPowerAc`)
- Battery Discharge Energy to DC (`pd.dsgPowerDc`)
- Slave 1 Battery Level (`bmsSlave1.soc`)   _(auto)_
- Slave 1 Battery Temperature (`bmsSlave1.temp`)   _(auto)_
- Slave 1 In Power (`bmsSlave1.inputWatts`)   _(auto)_
- Slave 1 Out Power (`bmsSlave1.outputWatts`)   _(auto)_
- Slave 2 Battery Level (`bmsSlave2.soc`)   _(auto)_
- Slave 2 Battery Temperature (`bmsSlave2.temp`)   _(auto)_
- Slave 2 In Power (`bmsSlave2.inputWatts`)   _(auto)_
- Slave 2 Out Power (`bmsSlave2.outputWatts`)   _(auto)_
- Status

*Switches*
- Beeper (`mppt.beepState` -> `{"moduleType": 0, "operateType": "TCP", "params": {"id": 38, "enabled": "VALUE"}}`)
- DC (12V) Enabled (`mppt.carState` -> `{"moduleType": 0, "operateType": "TCP", "params": {"id": 81, "enabled": "VALUE"}}`)
- AC Enabled (`inv.cfgAcEnabled` -> `{"moduleType": 0, "operateType": "TCP", "params": {"id": 66, "enabled": "VALUE"}}`)
- X-Boost Enabled (`inv.cfgAcXboost` -> `{"moduleType": 0, "operateType": "TCP", "params": {"id": 66, "xboost": "VALUE"}}`)
- AC Always On (`inv.acPassByAutoEn` -> `{"moduleType": 0, "operateType": "TCP", "params": {"id": 84, "enabled": "VALUE"}}`)
- Backup Reserve Enabled (`pd.bpPowerSoc` -> `{"moduleType": 0, "operateType": "TCP", "params": {"isConfig": "VALUE"}}`)

*Sliders (numbers)*
- Max Charge Level (`ems.maxChargeSoc` -> `{"moduleType": 0, "operateType": "TCP", "params": {"id": 49, "maxChgSoc": "VALUE"}}` [50 - 100])
- Min Discharge Level (`ems.minDsgSoc` -> `{"moduleType": 0, "operateType": "TCP", "params": {"id": 51, "minDsgSoc": "VALUE"}}` [0 - 30])
- Backup Reserve Level (`pd.bpPowerSoc` -> `{"moduleType": 0, "operateType": "TCP", "params": {"isConfig": 1, "bpPowerSoc": "VALUE", "minDsgSoc": 0, "maxChgSoc": 0, "id": 94}}` [10 - 85])
- Generator Auto Start Level (`ems.minOpenOilEbSoc` -> `{"moduleType": 0, "operateType": "TCP", "params": {"openOilSoc": "VALUE", "id": 52}}` [0 - 30])
- Generator Auto Stop Level (`ems.maxCloseOilEbSoc` -> `{"moduleType": 0, "operateType": "TCP", "params": {"closeOilSoc": "VALUE", "id": 53}}` [50 - 100])
- AC Charging Power (`inv.cfgSlowChgWatts` -> `{"moduleType": 0, "operateType": "TCP", "params": {"slowChgPower": "VALUE", "id": 69}}` [200 - 2900])

*Selects*
- DC (12V) Charge Current (`mppt.cfgDcChgCurrent` -> `{"moduleType": 0, "operateType": "TCP", "params": {"currMa": "VALUE", "id": 71}}` [4A (4000), 6A (6000), 8A (8000)])
- Screen Timeout (`pd.lcdOffSec` -> `{"moduleType": 0, "operateType": "TCP", "params": {"lcdTime": "VALUE", "id": 39}}` [Never (0), 10 sec (10), 30 sec (30), 1 min (60), 5 min (300), 30 min (1800)])
- Unit Timeout (`pd.standByMode` -> `{"moduleType": 0, "operateType": "TCP", "params": {"standByMode": "VALUE", "id": 33}}` [Never (0), 30 min (30), 1 hr (60), 2 hr (120), 4 hr (240), 6 hr (360), 12 hr (720)])
- AC Timeout (`inv.cfgStandbyMin` -> `{"moduleType": 0, "operateType": "TCP", "params": {"standByMins": "VALUE", "id": 153}}` [Never (0), 30 min (30), 1 hr (60), 2 hr (120), 4 hr (240), 6 hr (360), 12 hr (720), 24 hr (1440)])


