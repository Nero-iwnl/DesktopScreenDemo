## idf版本
xxx@ubuntu:~/work/esp/esp-idf$ idf.py --version
ESP-IDF v4.1.2-316-g5ea980e80c-dirty

## 配置环境
get_idf

## 配置 
idf.py menuconfig

## 编译
 idf.py build

## 清除
idf.py fullclean

## 下载
idf.py -p /dev/ttyUSB0 flash

## 监视器
idf.py -p /dev/ttyUSB0 monitor

## 构建、下载、监视
idf.py -p /dev/ttyUSB0 flash monitor

## 编译成功提示
Project build complete.

## 字体库下载
##                                       端口           波特率                   flash位置     字体库
python esptool.py --chip esp32 --port /dev/ttyUSB0 --baud 115200 write_flash -z 0x15D000 DesktopScreenFont.bin