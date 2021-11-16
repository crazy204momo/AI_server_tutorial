# AI server tutorial
## 終端機中python執行步驟:
### (此方法不能使用tensorflow, pytorch等套件)
1.	登入帳號
2.  在AI server中開啟終端機
3.	在$後直接輸入python3
```console
myaccount@ie54122:~$ python3
```
4.	即可在文字模式下執行python指令

## Docker中執行python步驟:
### (在docker環境中可使用tensorflow, pytorch等套件)
(pytorch環境請使用run_pytorch.sh開啟docker，tensorflow環境請使用run_tensorflow.sh開啟docker)
1.	登入帳號
2.  在AI server中開啟終端機
3.  建立自己的docker檔案路徑(以建立路徑data/mnist為例)
```console
myaccount@ie54122:~$ mkdir -p data/mnist
```
4.  從/tmp/路徑中複製兩份sh檔案(一份檔案為tensorflow使用, 一份檔案為pytorch使用)
```console
myaccount@ie54122:~$ cp /tmp/run*sh .
```
5. 開啟gedit文字編輯軟體，更改兩份sh檔案中的路徑為你剛才建立的路徑
```console
myaccount@ie54122:~$ gedit run_tensorflow.sh
```
![image](https://user-images.githubusercontent.com/50980857/142040011-637839a3-d9fd-4a08-b4e5-8220a51d2dbe.png)

改完這份後將gedit後方檔案換成run_pytorch.sh進行相同的更改

6.  開啟Docker
```console
myaccount@ie54122:~$ sh run_tensorflow.sh
```
看到以下畫面表示成功開啟docker
![image](https://user-images.githubusercontent.com/50980857/142040613-64fcb729-b893-4db9-91e5-2a2a3716708e.png)

7.  切換到建立py檔的路徑
```console
root@a7ad9b8eb0:/workspace# cd data/mnist
``` 
8.
