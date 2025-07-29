# CHANGELOG
## v0.4.0
### Added
- Add the watch as the device tracker entity. [#1189](https://github.com/XiaoMi/ha_xiaomi_home/pull/1189)
- Add the wifi speaker and the television as the media player entity. [#706](https://github.com/XiaoMi/ha_xiaomi_home/pull/706)
- Add an option in CONFIGURE to set the cover closed position. [#1242](https://github.com/XiaoMi/ha_xiaomi_home/pull/1242)
- Add notifications to show the status of the local connection to the central hub gateway. [#1280](https://github.com/XiaoMi/ha_xiaomi_home/pull/1280)
- Import the device from the third party cloud. [#1258](https://github.com/XiaoMi/ha_xiaomi_home/pull/1258)
### Changed
- Add an alongside switch entity for viomi.waterheater.m1. [#1255](https://github.com/XiaoMi/ha_xiaomi_home/pull/1255)
- Do not subscribe BLE device online/offline state message. [#1264](https://github.com/XiaoMi/ha_xiaomi_home/pull/1264)
### Fixed
- Keep the first element of the discovered ip address list as the recently added address when getting mdns result. [#1250](https://github.com/XiaoMi/ha_xiaomi_home/pull/1250)
- Subscribe local topics every time when connected to the central hub gateway. [#1266](https://github.com/XiaoMi/ha_xiaomi_home/pull/1266)
- Record the "closing" and "closed" status that occur frequently in the motor-controller, the window-opener and the curtain service. [#1262](https://github.com/XiaoMi/ha_xiaomi_home/pull/1262)
- Fix xiaomi.aircondition.c24 total power consumption unit, adp.motor.adswb4 motor switch, cgllc.airm.cgd1st environment temperature, and shhf.light.sflt11 fan switch status. [#1256](https://github.com/XiaoMi/ha_xiaomi_home/pull/1256)

## v0.3.4
### Added
- Exclude the unsupported device models. [#1205](https://github.com/XiaoMi/ha_xiaomi_home/pull/1205)
### Changed
- Subscribe the BLE device upstream messages even though the device is offline. [#1207](https://github.com/XiaoMi/ha_xiaomi_home/pull/1207)
- Record "opening", "closing" and "closed" status of the airer service that occur frequently and do not record "stop" status for the cover entity. [#1235](https://github.com/XiaoMi/ha_xiaomi_home/pull/1235)
- Modify README about spec_filter.yaml and the event attributes. [#1237](https://github.com/XiaoMi/ha_xiaomi_home/pull/1237)
### Fixed
- Fix the reconnect delay time to be reset when the client is connected to the broker. [#1200](https://github.com/XiaoMi/ha_xiaomi_home/pull/1200)
- Fix the HA warning in the logs related to vacuum state setting. [#694](https://github.com/XiaoMi/ha_xiaomi_home/pull/694)
- Fix the operation mode when the device does not have a mode property. [#1199](https://github.com/XiaoMi/ha_xiaomi_home/pull/1199)
- Fix 090615.aircondition.ktf environment temperature. [#1210](https://github.com/XiaoMi/ha_xiaomi_home/pull/1210)
- Fix a missing variable in translation it.json. [#1215](https://github.com/XiaoMi/ha_xiaomi_home/pull/1215)
- Fix yutai.plug.fsov8m power consumption and ignore bjkcz.curtain.kczble curtain status. [#1236](https://github.com/XiaoMi/ha_xiaomi_home/pull/1236)

## v0.3.3
### Changed
- Change the log level of error "mips unsub internal error, 4, None". [#1135](https://github.com/XiaoMi/ha_xiaomi_home/pull/1135)
- Add necessary logs for distinguishing the set_properties command source. [#1160](https://github.com/XiaoMi/ha_xiaomi_home/pull/1160)
### Fixed
- Fix tofan.airrtc.wk01 thermostat and air conditioner service. [#1160](https://github.com/XiaoMi/ha_xiaomi_home/pull/1160)
- Fix mrbond.airer.m1t closing status. [#1134](https://github.com/XiaoMi/ha_xiaomi_home/pull/1134)
- Fix the MIoT-Spec-V2 of xiaomi.fan.p69 fan service, ainice.sensor_occupy.3b people number, cykj.hood.jyj22 ventilation switch status, xiaomi.fan.p43 fan level, zhimi.airp.ua1a pm10 density, 090615.switch.x1tpm switch status, dmaker.fan.p33 fan-level. [#1132](https://github.com/XiaoMi/ha_xiaomi_home/pull/1132)
- Fix cubee.airrtc.th123e and cubee.airrtc.th123w MIoT-Spec-V2 instance descriptions in Russian.
- Fix ijai.vacuum.v1 suction-state value-list descriptions in Chinese.
- Fix the misuse of Chinese brackets in multi_lang.json.
- The unit of the humidity-range property of xiaomi.aircondition.mt0, xiaomi.aircondition.c35, xiaomi.aircondition.c24 and xiaomi.aircondition.c20 is "none". [#1187](https://github.com/XiaoMi/ha_xiaomi_home/pull/1187)

## v0.3.2
> Xiaomi Home has been added to the Home Assistant Community Store (HACS) as a default since May 8, 2025.
### Added
- Modify MIoT-Spec-V2 property format by spec_modify.yaml. [#1111](https://github.com/XiaoMi/ha_xiaomi_home/pull/1111)
### Changed
- Update the instructions of Xiaomi Home integration installation from HACS. [#102](https://github.com/XiaoMi/ha_xiaomi_home/pull/102) [#1088](https://github.com/XiaoMi/ha_xiaomi_home/pull/1088)
- Add an alongside switch entity for zimi.waterheater.h03 and xiaomi.waterheater.yms2. [#1115](https://github.com/XiaoMi/ha_xiaomi_home/pull/1115)
### Fixed
- Fix Chinese encoding in LAN Control. [#1114](https://github.com/XiaoMi/ha_xiaomi_home/pull/1114)
- Fix the MIoT-Spec-V2 of lxzn.switch.jcbcsm power consumption, voltage and current, shhf.light.sfla10 fan direction, zhimi.fan.za4 fan-level, zhimi.fan.sa1 fan-level. [#1110](https://github.com/XiaoMi/ha_xiaomi_home/pull/1110)
- Revise the Chinese descriptions of loock.lock.t2pv1 door state value-list. [#1110](https://github.com/XiaoMi/ha_xiaomi_home/pull/1110)

## v0.3.1
### Changed
- Setting the fan speed level when the fan is off will turning the fan on first. [#1031](https://github.com/XiaoMi/ha_xiaomi_home/pull/1031)
### Fixed
- Fix update device list error when there is no shared devices. [#1024](https://github.com/XiaoMi/ha_xiaomi_home/pull/1024)
- Fix the humidifier get_prop_value error when the property is None. [#1035](https://github.com/XiaoMi/ha_xiaomi_home/pull/1035)
- Fix the MIoT-Spec-V2 of zhimi.fan.v3 fan-level, cuco.plug.cp1md voltage and current, zimi.plug.zncz01 electric-power, giot.plug.v8icm power-consumption unit, yunmi.kettle.r3 tds unit, and dmaker.fan.p5 fan-level. [#1037](https://github.com/XiaoMi/ha_xiaomi_home/pull/1037)

## v0.3.0
注意：v0.3.0 变更了部分实体 unique_id 的生成规则，如果勾选 xiaomi_home > 配置 > 更新实体转换规则，会导致部分实体已配置的自动化失效。如果想要避免重新配置大量自动化，可使用这个[补丁](https://github.com/XiaoMi/ha_xiaomi_home/pull/972)。

CAUTION: v0.3.0 changes the unique_id of some entities. If you check the option `xiaomi_home > CONFIGURE > Update entity conversion rules`, it may cause the automation settings for these entities to fail. To avoid having to reconfigure a large number of automation settings, you can use this [patch](https://github.com/XiaoMi/ha_xiaomi_home/pull/972).
### Added
- Import the devices in the shared homes and the separated shared devices. [#1021](https://github.com/XiaoMi/ha_xiaomi_home/pull/1021)
- Support _attr_hvac_action of the climate entity. [#956](https://github.com/XiaoMi/ha_xiaomi_home/pull/956)
- Add custom defined MIoT-Spec-V2 instance via spec_add.json. [#953](https://github.com/XiaoMi/ha_xiaomi_home/pull/953)
### Fixed
- Ignore 'Event loop is closed' when unsub a closed event loop. [#991](https://github.com/XiaoMi/ha_xiaomi_home/pull/991)
- Fix contact-state for linp.magnet.m1 and loock.safe.v1. [#977](https://github.com/XiaoMi/ha_xiaomi_home/pull/977)
- Fix the mode initialization error of aupu.bhf_light.s368m. [#955](https://github.com/XiaoMi/ha_xiaomi_home/pull/955)
- Fix the MIoT-Spec-V2 of lumi.gateway.mcn001, qmi.plug.psv3, lumi.motion.acn001, izq.sensor_occupy.24, linp.sensor_occupy.hb01 and yunmi.waterpuri.s20. [#949](https://github.com/XiaoMi/ha_xiaomi_home/pull/949)

## v0.2.4
### Added
- Convert the submersion-state, the contact-state and the occupancy-status property to the binary_sensor entity. [#905](https://github.com/XiaoMi/ha_xiaomi_home/pull/905)
### Changed
- suittc.airrtc.wk168 mode descriptions are set to strings of numbers from 1 to 16. [#921](https://github.com/XiaoMi/ha_xiaomi_home/pull/921)
- Do not set _attr_suggested_display_precision when the spec.expr is set in spec_modify.yaml [#929](https://github.com/XiaoMi/ha_xiaomi_home/pull/929)
- Set "unknown event msg" log to info level.
### Fixed
- hhcc.plantmonitor.v1 soil moisture and soil ec icon and unit. [#927](https://github.com/XiaoMi/ha_xiaomi_home/pull/27)
- cuco.plug.cp2 voltage and power value ratio.
- cgllc.airmonitor.s1 unit ppb.
- roswan.waterpuri.lte01 tds unit.
- lumi.relay.c2acn01 power consumption unit
- xiaomi.bhf_light.s1 fan level of ventilation.

## v0.2.3
### Changed
- Specify the service name and the property name during the climate entity's on/off feature initialization. [#899](https://github.com/XiaoMi/ha_xiaomi_home/pull/899)
- Remove the useless total-battery property from `SPEC_PROP_TRANS_MAP`.
### Fixed
- Fix the hvac mode setting error when changing the preset mode of the ptc-bath-heater.
- Fix the ambiguous descriptions of yeelink.bhf_light.v10 ptc-bath-heater mode value-list.
- Fix the power consumption value of chuangmi.plug.212a01. [#910](https://github.com/XiaoMi/ha_xiaomi_home/pull/910)

## v0.2.2
This version has modified the conversion rules of the climate entity, which will have effect on the devices with the ptc-bath-heater, the air-conditioner and the air-fresh service. After updating, you need to restart Home Assistant and check `xiaomi_home > CONFIGURE >
Update entity conversion rules > NEXT` to reload the integration.

这个版本修改了浴霸、空调、新风机的实体转换规则，更新之后需要重启 Home Assistant，并且勾选 `xiaomi_home > 配置 > 更新实体转换规则 > 下一步` 重新加载集成。
### Added
- Add conversion rules for the air-conditioner service and the air-fresh service. [#879](https://github.com/XiaoMi/ha_xiaomi_home/pull/879)
### Changed
- Convert the mode of the ptc bath heater to the preset mode of the climate entity. [#874](https://github.com/XiaoMi/ha_xiaomi_home/pull/874)
- Use Home Assistant default icon when device_class is set. [#855](https://github.com/XiaoMi/ha_xiaomi_home/pull/855)
### Fixed
- Fix xiaomi.aircondition.m9 humidity-range unit. [#878](https://github.com/XiaoMi/ha_xiaomi_home/pull/878)
- Fix MIoT-Spec-V2 conflicts of xiaomi.fan.p5 and mike.bhf_light.2. [#866](https://github.com/XiaoMi/ha_xiaomi_home/pull/866)

## v0.2.1
### Added
- Add the preset mode for the thermostat. [#833](https://github.com/XiaoMi/ha_xiaomi_home/pull/833)
### Changed
- Change paho-mqtt version to adapt Home Assistant 2025.03. [#839](https://github.com/XiaoMi/ha_xiaomi_home/pull/839)
- Revert to use multi_lang.json. [#834](https://github.com/XiaoMi/ha_xiaomi_home/pull/834)
### Fixed
- Fix the opening and the closing status of linp.wopener.wd1lb. [#826](https://github.com/XiaoMi/ha_xiaomi_home/pull/826)
- Fix the format type of the wind-reverse property. [#810](https://github.com/XiaoMi/ha_xiaomi_home/pull/810)
- Fix the fan-level property without value-list but with value-range. [#808](https://github.com/XiaoMi/ha_xiaomi_home/pull/808)

## v0.2.0
This version has modified some default units of sensors. After updating, it may cause Home Assistant to pop up some compatibility warnings. You can re-add the integration to resolve it.

这个版本修改了一些传感器默认单位，更新后会导致 Home Assistant 弹出一些兼容性提示，您可以重新添加集成解决。

### Added
- Add prop trans rule for surge-power. [#595](https://github.com/XiaoMi/ha_xiaomi_home/pull/595)
- Support modify spec and value conversion. [#663](https://github.com/XiaoMi/ha_xiaomi_home/pull/663)
- Support the electric blanket. [#781](https://github.com/XiaoMi/ha_xiaomi_home/pull/781)
- Add device with motor-control service as cover entity. [#688](https://github.com/XiaoMi/ha_xiaomi_home/pull/688)
### Changed
- Update README file. [#681](https://github.com/XiaoMi/ha_xiaomi_home/pull/681) [#747](https://github.com/XiaoMi/ha_xiaomi_home/pull/747)
- Update CONTRIBUTING.md. [#681](https://github.com/XiaoMi/ha_xiaomi_home/pull/681)
- Refactor climate.py. [#614](https://github.com/XiaoMi/ha_xiaomi_home/pull/614)
### Fixed
- Fix variable name or comment errors & fix test_lan error. [#678](https://github.com/XiaoMi/ha_xiaomi_home/pull/678) [#690](https://github.com/XiaoMi/ha_xiaomi_home/pull/690)
- Fix water heater error & some type error. [#684](https://github.com/XiaoMi/ha_xiaomi_home/pull/684)
- Fix fan level with value-list & fan reverse [#689](https://github.com/XiaoMi/ha_xiaomi_home/pull/689)
- Fix sensor display precision [#708](https://github.com/XiaoMi/ha_xiaomi_home/pull/708)
- Fix event:motion-detected without arguments [#712](https://github.com/XiaoMi/ha_xiaomi_home/pull/712)

## v0.1.5b2
### Added
- Support binary sensors to be displayed as text sensor entities and binary sensor entities. [#592](https://github.com/XiaoMi/ha_xiaomi_home/pull/592)
- Add miot cloud test case. [#620](https://github.com/XiaoMi/ha_xiaomi_home/pull/620)
- Add test case for user cert. [#638](https://github.com/XiaoMi/ha_xiaomi_home/pull/638)
- Add mips test case & Change mips reconnect logic. [#641](https://github.com/XiaoMi/ha_xiaomi_home/pull/641)
- Support remove device. [#622](https://github.com/XiaoMi/ha_xiaomi_home/pull/622)
- Support italian translation. [#183](https://github.com/XiaoMi/ha_xiaomi_home/pull/183)
### Changed
- Refactor miot spec. [#592](https://github.com/XiaoMi/ha_xiaomi_home/pull/592)
- Refactor miot mips & fix type errors. [#365](https://github.com/XiaoMi/ha_xiaomi_home/pull/365)
- Using logging for test case log print. [#636](https://github.com/XiaoMi/ha_xiaomi_home/pull/636)
- Add power properties trans. [#571](https://github.com/XiaoMi/ha_xiaomi_home/pull/571)
- Move web page to html. [#627](https://github.com/XiaoMi/ha_xiaomi_home/pull/627)
### Fixed
- Fix miot cloud and mdns error. [#637](https://github.com/XiaoMi/ha_xiaomi_home/pull/637)
- Fix type error

## v0.1.5b1
This version will cause some Xiaomi routers that do not support access (#564) to become unavailable. You can update the device list in the configuration or delete it manually.
### Added
- Fan entity support direction ctrl [#556](https://github.com/XiaoMi/ha_xiaomi_home/pull/556)
### Changed
- Filter miwifi.* devices and xiaomi.router.rd03 [#564](https://github.com/XiaoMi/ha_xiaomi_home/pull/564)
### Fixed
- Fix multi ha instance login [#560](https://github.com/XiaoMi/ha_xiaomi_home/pull/560)
- Fix fan speed [#464](https://github.com/XiaoMi/ha_xiaomi_home/pull/464)
- The number of profile models updated from 660 to 823. [#583](https://github.com/XiaoMi/ha_xiaomi_home/pull/583)

## v0.1.5b0
### Added
- Add missing parameter state_class  [#101](https://github.com/XiaoMi/ha_xiaomi_home/pull/101)
### Changed
- Make git update guide more accurate [#561](https://github.com/XiaoMi/ha_xiaomi_home/pull/561)
### Fixed
- Limit *light.mode count (value-range) [#535](https://github.com/XiaoMi/ha_xiaomi_home/pull/535)
- Update miot cloud raise error msg [#551](https://github.com/XiaoMi/ha_xiaomi_home/pull/551)
- Fix table header misplacement [#554](https://github.com/XiaoMi/ha_xiaomi_home/pull/554)

## v0.1.4
### Added
- Refactor miot network, add network detection logic, improve devices filter logic. [458](https://github.com/XiaoMi/ha_xiaomi_home/pull/458) [#191](https://github.com/XiaoMi/ha_xiaomi_home/pull/191)
### Changed
- Remove tev dependency for lan control & fixs. [#333](https://github.com/XiaoMi/ha_xiaomi_home/pull/333)
- Use yaml to parse action params. [#447](https://github.com/XiaoMi/ha_xiaomi_home/pull/447)
- Update issue template. [#445](https://github.com/XiaoMi/ha_xiaomi_home/pull/445)
- Remove duplicate dependency(aiohttp) [#390](https://github.com/XiaoMi/ha_xiaomi_home/pull/390)
### Fixed

## v0.1.4b1
### Added
- Support devices filter, and device changed notify logical refinement. [#332](https://github.com/XiaoMi/ha_xiaomi_home/pull/332)
### Changed
- Readme amend HACS installation. [#404](https://github.com/XiaoMi/ha_xiaomi_home/pull/404)
### Fixed
- Fix unit_convert AttributeError, Change to catch all Exception. [#396](https://github.com/XiaoMi/ha_xiaomi_home/pull/396)
- Ignore undefined piid and keep processing following arguments. [#377](https://github.com/XiaoMi/ha_xiaomi_home/pull/377)
- Fix some type error, wrong use of any and Any. [#338](https://github.com/XiaoMi/ha_xiaomi_home/pull/338)
- Fix lumi.switch.acn040 identify service translation of zh-Hans [#412](https://github.com/XiaoMi/ha_xiaomi_home/pull/412)

## v0.1.4b0
### Added
### Changed
### Fixed
- Fix miot cloud token refresh logic. [#307](https://github.com/XiaoMi/ha_xiaomi_home/pull/307)
- Fix lan ctrl filter logic. [#303](https://github.com/XiaoMi/ha_xiaomi_home/pull/303)

## v0.1.3
### Added
### Changed
- Remove default bug label. [#276](https://github.com/XiaoMi/ha_xiaomi_home/pull/276)
- Improve multi-language translation actions. [#256](https://github.com/XiaoMi/ha_xiaomi_home/pull/256)
- Use aiohttp instead of waiting for blocking calls. [#227](https://github.com/XiaoMi/ha_xiaomi_home/pull/227)
- Language supports dt. [#237](https://github.com/XiaoMi/ha_xiaomi_home/pull/237)
### Fixed
- Fix local control error. [#271](https://github.com/XiaoMi/ha_xiaomi_home/pull/271)
- Fix README_zh and miot_storage. [#270](https://github.com/XiaoMi/ha_xiaomi_home/pull/270)

## v0.1.2
### Added
- Support Xiaomi Heater devices. https://github.com/XiaoMi/ha_xiaomi_home/issues/124 https://github.com/XiaoMi/ha_xiaomi_home/issues/117
- Language supports pt, pt-BR.
### Changed
- Adjust the minimum version of HASS core to 2024.4.4 and above versions.
### Fixed

## v0.1.1
### Added
### Changed
### Fixed
- Fix humidifier trans rule. https://github.com/XiaoMi/ha_xiaomi_home/issues/59
- Fix get homeinfo error.  https://github.com/XiaoMi/ha_xiaomi_home/issues/22
- Fix air-conditioner switch on. https://github.com/XiaoMi/ha_xiaomi_home/issues/37 https://github.com/XiaoMi/ha_xiaomi_home/issues/16
- Fix invalid cover status. https://github.com/XiaoMi/ha_xiaomi_home/issues/11  https://github.com/XiaoMi/ha_xiaomi_home/issues/85
- Water heater entity add STATE_OFF. https://github.com/XiaoMi/ha_xiaomi_home/issues/105 https://github.com/XiaoMi/ha_xiaomi_home/issues/17

## v0.1.0
### Added
- First version
### Changed
### Fixed
