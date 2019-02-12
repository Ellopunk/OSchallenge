# Printer Woes 

**Objective:** Getting my printer to work on openSUSE


## [Brother HL-L2350DW](https://support.brother.com/g/b/downloadhowto.aspx?c=us&lang=en&prod=hll2350dw_us_eu_as&os=127&dlid=dlf006893_000&flang=4&type3=625)

Steps taken:

1) Downloaded RPM package.

2) Unzipped package

`gunzip linux-brprinter-installer-*.*.*-*.gz` 

3) run install script 

`sudo bash linux-brprinter-installer-2.2.1-1` 

**error:** no provider libusb-0.1-4

## My solution attempt

`zypper install libusb`

```
|libusb-0_1-4|0.1.13-36.12|x86_64|
```

### Question

The package needed is libusb-0.1-4

The package installed is libusb0_1-4

Has anyone had a similar experience and have an answer or an idea for what I should be trying next?