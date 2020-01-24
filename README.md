By Roker2

## libfp_client.so

Need to change B.NE loc_XXXXX to CMP X1, X2

CMP X1, X2 = 5F 00 01 EB in HEX

Based on comparing Leeco S2 blobs

Maybe need to patch Aliplay functions

| Function                                 | Patch place | Patch status (patched or not) |
| :--------------------------------------- | :---------- | :---------------------------- |
| BpFingerPrint::disableFingerScreenUnlock | 13EE0       | yes                           |
| BpFingerPrint::enableFingerScreenUnlock  | 13FB4       | yes                           |
| BpFingerPrint::driverTest                | 14300       | yes                           |
| BpFingerPrint::cancelRecognize           | 14718       | yes                           |
| BpFingerPrint::recognize                 | 14ABC       | yes                           |
| BpFingerPrint::resetRegist               | 14D6C       | yes                           |
| BpFingerPrint::registRollback            | 14E40       | yes                           |
| BpFingerPrint::cancelRegist              | 14F14       | yes                           |
| BpFingerPrint::regist                    | 14FE8       | yes                           |
| BpFingerPrint::query                     | 152E4       | yes                           |
| BpFingerPrint::disconnect                | 154A4       | yes                           |
| BpFingerPrint::setActiveGroup            | 15820       | not                           |
| BpFingerPrint::setPauseRegisterState     | 14404       | yes                           |
| BpFingerPrint::saveRegist                | 14BA8       | yes                           |
| BpFingerPrint::unRegist                  | 14C94       | yes                           |
| BpFingerPrint::sendScreenState           | 1520C       | yes                           |
| BpFingerPrint::setMode                   | 153CC       | yes                           |
| BpFingerPrint::delFpTemplates            | 14640       | yes                           |
| BpFingerPrint::checkPasswd               | 1596C       | yes                           |
| BpFingerPrint::recognizeFido             | 14840       | yes                           |
| BpFingerPrint::recognizeWithRestrict     | 149B8       | yes                           |
| BpFingerPrint::fillAuthTokenHmac         | 15710       | not                           |
| BpFingerPrint::getFpTemplateIdList       | 144FC       | yes                           |
| BpFingerPrint::getInfo                   | 15764       | yes                           |
| BpFingerPrint::getFpNameById             | 1420C       | yes                           |
| BpFingerPrint::modifyFpName              | 1587C       | yes                           |
| BpFingerPrint::setPasswd                 | 17390       | yes                           |
| BpFingerPrint::saveRegister              | 174A4       | yes                           |
| BpFingerPrint::requestPermission         | 175A8       | yes                           |
| BpFingerPrint::SendCmd                   | 1791C       | yes                           |
| BpFingerPrint::connect                   | 17C34       | yes                           |
| BpFingerPrint::getFpTemplateList         | 19848       | yes                           |
| BpFingerPrintService::connect            | 1A72C       | yes                           |
| BpFingerPrintService::check              | 1A81C       | yes                           |

34 functions
