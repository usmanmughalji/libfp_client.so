By Roker2

## libfp_client.so

Need to change B.NE loc_XXXXX to CMP X1, X2

CMP X1, X2 = 5F 00 01 EB in HEX

Based on comparing Leeco S2 blobs

Maybe need to patch Aliplay functions

| Function                                 | Patch place | Patch status (patched or not) |
| :--------------------------------------- | :---------- | :---------------------------- |
| BpFingerPrint::disableFingerScreenUnlock | 153D8       | no                            |
| BpFingerPrint::enableFingerScreenUnlock  | 154AC       | no                            |
| BpFingerPrint::driverTest                | 15A30       | no                            |
| BpFingerPrint::cancelRecognize           | 15E48       | no                            |
| BpFingerPrint::recognize                 | 162F0       | no                            |
| BpFingerPrint::resetRegist               | 165A0       | no                            |
| BpFingerPrint::registRollback            | 16674       | no                            |
| BpFingerPrint::cancelRegist              | 16748       | no                            |
| BpFingerPrint::regist                    | 1681C       | no                            |
| BpFingerPrint::query                     | 16C14       | no                            |
| BpFingerPrint::disconnect                | 16DD4       | no                            |
| BpFingerPrint::setActiveGroup            | 15820       | no                            |
| BpFingerPrint::setPauseRegisterState     | 15B34       | no                            |
| BpFingerPrint::saveRegist                | 163DC       | no                            |
| BpFingerPrint::unRegist                  | 164C8       | no                            |
| BpFingerPrint::sendScreenState           | 16B3C       | no                            |
| BpFingerPrint::setMode                   | 16CFC       | no                            |
| BpFingerPrint::delFpTemplates            | 15D70       | no                            |
| BpFingerPrint::checkPasswd               | 17294       | no                            |
| BpFingerPrint::recognizeFido             | 15F70       | no                            |
| BpFingerPrint::recognizeWithRestrict     | 161EC       | no                            |
| BpFingerPrint::fillAuthTokenHmac         | 15710       | no                            |
| BpFingerPrint::getFpTemplateIdList       | 15C2C       | no                            |
| BpFingerPrint::getInfo                   | 1708C       | no                            |
| BpFingerPrint::getFpNameById             | 1593C       | no                            |
| BpFingerPrint::modifyFpName              | 171A4       | no                            |
| BpFingerPrint::setPasswd                 | 17390       | no                            |
| BpFingerPrint::saveRegister              | 174A4       | no                            |
| BpFingerPrint::requestPermission         | 175A8       | no                            |
| BpFingerPrint::SendCmd                   | 1791C       | no                            |
| BpFingerPrint::connect                   | 17C34       | no                            |
| BpFingerPrint::getFpTemplateList         | 19848       | no                            |
| BpFingerPrintService::connect            | 1A72C       | no                            |
| BpFingerPrintService::check              | 1A81C       | no                            |