# UICC
To download the [UICC v2.6](https://open-cells.com/index.php/uiccsim-programing/) tar file [click here](https://open-cells.com/d5138782a8739209ec5760865b1e53b0/uicc-v2.6.tgz)

#### To configure sim for SD-Core:
```
sudo ./program_uicc --adm 12345678 --imsi 001010100007494 --isdn 00000001 --acc 0001 --key 5122250214c33e723a5dd523fc145fc0 --opc 981d464c7c52eb6e5036234984ad0bcf -spn "OpenAirInterface" --authenticate
```

#### To configure sim for OAI-Core:
```
sudo ./program_uicc --adm 12345678 --imsi 001010000000001 --isdn 00000001 --acc 0001 --key fec86ba6eb707ed08905757b1bb44b8f --opc C42449363BBAD02B66D16BC975D77CC1 -spn "OpenAirInterface" --authenticate
```
<br>

> **_NOTE:_** If you face any error while running the above commands, then:
- remove the binary file `program_uicc` from the `uicc-v2.6` directory
- and the run `make` command in terminal
- then run the above command/s to wirte the sim configuration
