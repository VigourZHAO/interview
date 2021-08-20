Open vSwitch: 即 OVS
    释：运行在虚拟化平台上的虚拟交换机，支持 OpenFlow 协议，支持 gre/vxlan/IPsec 等隧道技术。
        OpenFlow: SDN控制器，通过控制交换机或路由器来改变数据包走向。
        gre: 网桥中数据穿过的通道
        vxlan: 将网卡(Ethernet)封装成UDP，添加8字节的VXLAN header，区分不同的二层网络（8字节24比特标识，上限1600多万个）
        vlan: 直接在网卡(Ethernet)头部加4字节标记VLAN Tag。（4字节12比特标识，上限4000多个）
        IPsec:
    OVS 可以依靠自己的 MAC 学习实现二层数据包转发功能，如 Linux Bridge。
