# dynamix.system.autofan

### Add cpu temperature and motherboard temperature monitor when only including nvme devices

### When getting the temp of nvme devices, skip sdspin because the exit code of sdsping is always 25, resulting that the temperature of nvme devices is always 0C.

