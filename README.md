# rk3568-kernel5.10-alldrivers
源码是rk3588-5.10.66内核，提取自https://github.com/radxa/kernel/tree/stable-5.10-rock5  

本版本是对rk3568适配以及panfrost适配，

dts文件仅仅适配了rock-3a，其他开发板请自行设置dts文件，原则上支持rk33**，rk356x（未作测试）

npu,rga,vop2,mpp,panfrost for rock3a

不需要编译内核仅使用镜像文件请到 https://github.com/qxhome/rk3568-kernel5.10-alldrivers/releases  下载镜像

本内核版本内核可能缺乏部分wifi网卡驱动，请自行移植

rk对drm操作或其他硬件操作做了特殊的权限设置，使用内核时候碰到权限问题需自行在内核模块源码中对相关权限做调整（常见操作需要权限已经调整好）

内核config文件中部分模块未开启，导致部分通用程序依赖缺乏，根据需求自行需要开启相关模块config
