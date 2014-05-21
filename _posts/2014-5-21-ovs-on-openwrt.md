---
layout: post
title: "OVS on OpenWrt"
---
`git clone git://git.openwrt.org/openwrt.git`

`cd openwrt`

`./scripts/feeds update -a`

`./scripts/feeds install -a`

`make menuconfig`

`make V=s`

`echo 'src-git openvswitch git://github.com/aigamo/openvswitch.git' >> feeds.conf`

`./scripts/feeds update openvswitch`

`./scripts/feeds install -a -p openvswitch`

`make menuconfig`

select openvswitch and others

`make V=s`
