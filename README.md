# ViPSN
<img src="https://raw.githubusercontent.com/dremofly/oss/master/uPic/2020-08-29/NShvox.png" alt="ViPSN"  align="right" width="45%">

**ViPSN** (acronym of vibration-powered sensing node) is a programmable Internet of Things (IoT) platform for the development of vibration- or motion-powered sensing and transmitting systems. It serves as a reconfigurable developing platform for vibration-powered IoT applications. The whole set of **ViPSN** assembles six basic modules: a vibration emulator as the energy generation unit (**EGU**); a piezoelectric transducer as the energy transduction unit (**ETU**); a power-boosting interface circuit as the energy enhancement unit (**EEU**); a dc-dc regulator with energy-level indicating signals as the energy management unit (**EMU**); a Bluetooth low energy (BLE) module as the energy user unit (**EUU**); and a mobile app as the edge demonstration unit (**EDU**). All units or modules are connected with easy mechanical joggle joints and electrical plunger pin contacts.

<!-- ## System overview -->

<!-- ## Project structure -->

## Setup and usage

Coming soon! This is first version (2020-08-28) of ViPSN. 
Right now we are working on a way to get hardware to people, please contact the authors for more information. 
For now, feel free to explore the hardware and software designs, but be sure to cite our work.
```
@article{li2020vipsn,
  title={ViPSN: A vibration-powered iot platform},
  author={Li, Xin and Teng, Li and Tang, Hong and Chen, Jingying and Wang, Haoyu and Liu, Yu and Fu, Minfan and Liang, Junrui},
  journal={IEEE Internet of Things Journal},
  year={2020},
  publisher={IEEE}
}
```
## Prerequisites
### Hardware design
- Altium Designer (version 9.4 or above) is used for the PCB design.
- Solidworks (version 2018 or above) is used for 3D-printer case.
### Software design
- Keil5 is required to compile the software. 

### Specification
<table style="border-collapse: collapse; border: none; border-spacing: 0px;">
	<tr>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>Unit</b>
		</td>
		<td colspan="3" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			<b>Specification</b>
		</td>
	</tr>
	<tr>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			EGU
		</td>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Resonant speaker
		</td>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Type
		</td>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			ADIN-B1BT
		</td>
	</tr>
	<tr>
		<td rowspan="4" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			ETU
		</td>
		<td rowspan="2" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Piezoelectric
			<br>
			 transducer
		</td>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Diameter
		</td>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			30 mm
		</td>
	</tr>
	<tr>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Material
		</td>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			PZT sheet on steel
		</td>
	</tr>
	<tr>
		<td rowspan="2" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Mass
		</td>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Weight
		</td>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			13 g
		</td>
	</tr>
	<tr>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Material
		</td>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Steel
		</td>
	</tr>
	<tr>
		<td rowspan="2" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			EEU
		</td>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			SEH
		</td>
		<td colspan="2" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Full-wave bridge rectifier
		</td>
	</tr>
	<tr>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			SP-SSHI
		</td>
		<td colspan="2" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Parallel SP-SSHI
		</td>
	</tr>
	<tr>
		<td rowspan="3" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			EMU
		</td>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			DC-DC Converter
		</td>
		<td colspan="2" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			LTC3588-1
		</td>
	</tr>
	<tr>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Comparator
		</td>
		<td colspan="2" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			MIC841
		</td>
	</tr>
	<tr>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Storage
		</td>
		<td colspan="2" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Electrolytic capacitor
		</td>
	</tr>
	<tr>
		<td rowspan="2" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			EUU
		</td>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			SoC
		</td>
		<td colspan="2" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			nRF52832
		</td>
	</tr>
	<tr>
		<td style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			Software
		</td>
		<td colspan="2" style="border-width: 1px; border-style: solid; border-color: rgb(0, 0, 0); text-align: center; padding-right: 3pt; padding-left: 3pt;">
			nRF5 SDK V15.2
		</td>
	</tr>
</table>

<!-- ### Software Provided 

In **EGU** and **ETU** folders, this project provides the [Audio](./VSU/Audio/Example) file, which is played by resonant speaker. [AudioGenerator](./VSU/Audio/AudioGenerator.m) can be edited to generate a stable audio wave and . Also, the 3D model file is provided. More details are shown in [VSU README.md](./VSU/README.md).

In **EEU** folder, here are four types circuit model, SEH, self-power P-SSHI, self-power SECE, self-power S-SSHI.

In **EMU** folder, here is a PCB file.

In **EUU** folder, this project provides the [Transmitter Part](.\EUU\software\EUU_trans\examples) and [Receive Part](.\EUU\software\Receiver). And [PCB file](.\EUU\pcb) is also included.  -->

## Related publications
- Xin Li, Li Teng, Hong Tang, Jingying Chen, Haoyu Wang, Yu Liu, Minfan Fu, and Junrui Liang, "ViPSN: a vibration-powered IoT platform," IEEE Internet of Things Journal, doi: 10.1109/JIOT.2020.3016993. <a name="divtop"></a>
- Xin Li, Hong Tang, Yiyao Zhu and Junrui Liang*, “Power solution of a vibration-powered sensing node,” Proceedings of the 9th International Power Electronics and Motion Control Conference, Nanjing, China, May 31-June 3, 2020. (IPEMC - ECCE Asia 2020). <a name="divtop2"></a>
- Xin Li, Hong Tang, Bao Zhao, and Junrui Liang*, “System design and implementation of a transient-motion-powered IoT sensor node,” Proceedings of the ASME 2020 Conference on Smart Materials, Adaptive Structures and Intelligent Systems, Irvine, CA, USA, September 14–16, 2020. (SMASIS 2020) (Finalist of Best Student Hardware Competision).
- Xin Li, Hong Tang, Junrui Liang*, and Lihua Tang, "Exploring the magnetic plucking motion towards a transient-motion-powered IoT sensor node", Proceedings of SPIE Conference 11376, Active and Passive Smart Structures and Integrated Systems IX, 113761U, 22 April 2020. (SPIE SS/NDE 2020).
- Kang Zhao, Yuheng Zhao, and Junrui Liang*, “Live Demo of A Vibration-Powered Bluetooth Sensor with Running PFC Power Conditioning”, Proceedings of the 2017 IEEE International Symposium on Circuits and Systems, Baltimore, USA, May 2017. (ISCAS 2017).
- Kang Zhao, Yuheng Zhao, and Junrui Liang*, “A vibration-powered Bluetooth wireless sensor node with running PFC power conditioning”, Proceedings of the 2017 IEEE International Symposium on Circuits and Systems, Baltimore, USA, May 2017. (ISCAS 2017).

## Contributors
- Yuheng Zhao and Kang Zhao contributed early on to the hardware designs in 2017.
- Xin Li proposed and designed the system of ViPSN in 2019. Hong Tang implemented the hardwares of system. Li Teng and Jingying Chen helped with some works of EMU.
- Prof. Junrui Liang oversaw, funded, and originated the project.

## Funding
This research was supported by the grants from the National Natural Science Foundation of China (Project No. 61401277) and ShanghaiTech University (Project No. F-0203-13-003).

## License
```
Apache License
Copyright 2020 Xin Li, Hong Tang, and Junrui Liang*, ShanghaiTech University.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```
## Contact
If you have technical problems, please contact: lixin1@shanghaitech.edu.cn or tanghong@shanghaitech.edu.cn.

For business cooperation, please contact: liangjr@shanghaitech.edu.cn.
