# 数据平面

## 南向协议

### OpenFlow
### NETCONF
### OVSDB
### PCEP
### OF-CONFIG

## Switch_OS

### OVS
### DPDK
### OpenSwitch
### FD.io

## 芯片

## 数据平面可编程语言

### P4
Programming Protocol-Independent Packet Processors

### Introduction

SDN因其能让网络使用者对网络行为进行编程而取得了巨大的成功, 但当前SDN的可编程性局限于SDN控制平面, 数据平面(即包转发逻辑)仍主要由固定功能的交换芯片所决定。而P4编程语言的出现解决了这一窘境，其对交换机内部数据报处理过程的灵活定义让网络设计者可以自上而下地定义数据报的完整处理流程。

P4(www.p4.org)是由斯坦福大学的Nick McKeown教授和普林斯顿大学的Jennifer Rexford教授、以及谷歌、英特尔、微软和 Barefoot Networks共同发起并创立的一个开源项目, P4作为数据平面领域专用语言(DSL)描述了交换机内部对数据报报文的处理逻辑, 从CPU到高端的 ASIC皆有广泛的应用前景。P4开源社区现巳有超过60个成员, 正在开发各种新的网络行为和新的运用, 其成果已在多项国际会议发表, 并在商业部署中取得了突破性的进展。

### Resources

P4语言联盟 官方网站：P4.org

Barefoot 官方网站：https://barefootnetworks.com

Wikipedia: [P4 (programming language)](https://en.wikipedia.org/wiki/P4_(programming_language))

#### Paper：

[P4: Programming Protocol-Independent Packet Processors](http://www.sigcomm.org/sites/default/files/ccr/papers/2014/July/0000000-0000004.pdf)

#### Github

> P4语言 Github主页：

[p4language](https://github.com/p4lang)

> Repository(部分):

仓库名称：仓库介绍

[tutorials](https://github.com/p4lang/tutorials): P4 language tutorials. 

[switch](https://github.com/p4lang/switch): Consolidated switch repo (API, SAI and Nettlink).

[p4factory](https://github.com/p4lang/p4factory): Compile P4 and run the P4 behavioral simulator.

[p4c-bm](https://github.com/p4lang/p4c-bm): Generates the JSON configuration for the behavioral-model (bmv2), as well as the C/C++ PD code.

[behavioral-model](https://github.com/p4lang/behavioral-model): Rewrite of the behavioral model as a C++ project without auto-generated code (except for the PD interface).

[p4c](https://github.com/p4lang/p4c): P4_16 prototype compiler.

#### [SDNLAB](http://www.sdnlab.com)

> 学习类：

[P4语言规范](http://www.sdnlab.com/resource/11954.html)

[P4语言编程详解](http://www.sdnlab.com/17882.html)

[《P4语言规范》Header & Instances详解 ](http://www.sdnlab.com/17955.html)

[《P4语言规范》parser详解 ](http://www.sdnlab.com/18021.html)

> 介绍类：

[P4:开创数据平面可编程时代](http://www.sdnlab.com/17795.html)

[P4: 面向服务器主导网络互联推进技术创新](http://www.sdnlab.com/18380.html)

[P4和POF的对比](http://www.sdnlab.com/17869.html)

[用P4对数据平面进行编程](http://www.sdnlab.com/17456.html)

[P4：编写协议无关的包处理器](http://www.sdnlab.com/17107.html)

[p4-latest](http://www.sdnlab.com/resource/15188.html)

[P4 Programming Protocol-Independent Packet Processors](http://www.sdnlab.com/resource/15186.html/)

[P4语言,踢馆OpenFlow的SDN新秀](http://www.sdnlab.com/11884.html)

> 实战类：

[P4开源Tutorials实战及对P4规范的初分析](http://www.sdnlab.com/18618.html)

[P4语言编程快速开始](www.sdnlab.com/18072.html)

[PISCES:可编程、协议无关的软件交换机解析及应用实例](http://www.sdnlab.com/18040.html)

[搭建P4C与P4FPGA联合编译环境](http://www.sdnlab.com/18366.html)

> 会议类：

[国内首届P4技术交流圆满成功](http://www.sdnlab.com/18039.html)

[12月8日，P4 Workshop亮相GNTC全球网络技术大会](http://www.sdnlab.com/18084.html)

[Network Field Day 14–Barefoot Networks](http://www.sdnlab.com/18443.html)

> 资讯类：

[北京邮电大学加入P4项目，系国内首个高校成员单位](http://www.sdnlab.com/17849.html)

[P4研究备受关注，2017或将落地商用](http://www.sdnlab.com/15177.html)

[Barefoot将通过Tofino重新定义网络设备中的ASIC](http://www.sdnlab.com/?s=P4)

[Barefoot发布基于Tofino芯片的Wedge 100B交换机系列](http://www.sdnlab.com/18447.html)

[Barefoot Networks进军白盒市场](http://www.sdnlab.com/18413.html)

#### [sdxcentral](https://www.sdxcentral.com)

> 资讯类：

[Barefoot Networks Steps Into the ONS Spotlight](https://www.sdxcentral.com/articles/news/barefoot-networks-steps-into-the-ons-spotlight/2015/06/)

[Barefoot Networks Just Raised Another $57M](https://www.sdxcentral.com/articles/news/barefoot-networks-just-raised-another-57m/2016/06/)

[Barefoot Networks Steps Into the White Box Market](https://www.sdxcentral.com/articles/news/barefoot-networks-steps-white-box-market/2017/01/)

[AT&T Is Giving the P4 Language a Whirl](https://www.sdxcentral.com/articles/news/att-giving-p4-language-whirl/2016/04/)

[Support Builds for P4 to Boost NFV](https://www.sdxcentral.com/articles/analysis/p4-lanugage-to-boost-nfv/2016/06/)

> 介绍类：

[Why Barefoot Networks Decided SDN Needs a New Chip](https://www.sdxcentral.com/articles/news/barefoot-networks/2016/06/)

[Barefoot Networks’ McKeown: On OpenFlow, P4 & the Programmable Network](https://www.sdxcentral.com/articles/interview/mckeown-barefoot-networks-openflow-p4/2016/06/)

[Barefoot Networks' McKeown: Part 2](https://www.sdxcentral.com/articles/interview/barefoot-networks-mckeown-part-2/2016/06/)

[P4 SDN Language Aims to Take SDN Beyond OpenFlow](https://www.sdxcentral.com/articles/news/p4-language-aims-to-take-sdn-beyond-openflow/2015/05/)

[OpenFlow's Possible Successor P4, Gets Into Hardware](https://www.sdxcentral.com/articles/news/p4-openflows-possible-successor-gets-into-hardware/2015/11/)

#### Barefoot

[Whitepaper: The World's Fastest & Most Programmable Networks](https://barefootnetworks.com/white-paper/the-worlds-fastest-most-programmable-networks/)

#### Netronome

[P4 Network Data Plane Programming: What it is, and Why it Matters ](https://www.netronome.com/blog/p4-network-data-plane-programming-what-it-is-and-why-it-matters/)

#### YouTube

[P4 Language Consortium](https://www.youtube.com/channel/UCOQAFkDKucJWr-KafdJsdIQ)

#### Blogs

[Milestone P4](http://www.muzixing.com/tag/p4.html)

[Takeshi's Blog SDN](https://takeshi.tw/category/sdn/)

[P4 台灣社群](https://p4tw.org/)

[Wasdns P4Language](http://www.cnblogs.com/qq952693358/category/887928.html)

