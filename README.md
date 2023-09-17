# ScanReflectedSSTI

This script allows to find SSTI vulnerabilities with nuclei, taking advantage of this resource in its maximum analysis capacity.

In the community I have not seen XSS Fuzzing with nuclei in general, only focused on exploitations by CVE

## Testing Fuzzing GET

In the first instance they must collect the urls with the GET parameters.

```sh
cat url.txt | nuclei -t ScanSSTI.yaml
nuclei -u 'http://192.168.100.61/xvwa/vulnerabilities/ssti/?name=&submit=' -t ScanSSTI.yaml 
```


![image](https://github.com/HernanRodriguez1/ScanReflectedSSTI/assets/66162160/4eaae9bf-985f-4981-8f80-ec5400aabe2c)

