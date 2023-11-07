# dynamix.system.autofan

- Add cpu temperature and motherboard temperature monitor when only including nvme devices

- When getting the temp of nvme devices, skip sdspin because the exit code of sdsping is always 25, resulting that the temperature of nvme devices is always 0C.

由于机箱采用上下分层接口，同时检测上层的一个固态温度、CPU温度、主板温度并取最大值。

在检测固态温度时，跳过sdspin命令，因为其退出码一直是25，导致获取到的温度一直为0.
