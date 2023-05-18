# Auto_Simulated_Universe
星穹铁道-模拟宇宙全自动化

目前只支持模拟宇宙6（地图数据不全），正在更新地图数据

用法： python states.py --find=1

只支持1920\*1080窗口化，关闭“沿用自动战斗设置”，关闭HDR。模拟宇宙技能树不能存在红点（这个后续会优化）

info.txt中保存了模拟宇宙开局选的角色，1表示第一个角色。最好在一号位选远程角色（艾丝妲、三月七）方便开怪。

选祝福的逻辑是硬选巡猎。

寻路模块基于小地图，所以跑图的时候会低头保持小地图不受高亮的天空干扰

小地图中只会识别白色边缘线和黄色交互点。

----------------------------------------------------------------------------------------------

支持增加地图，具体方法为

进入新图，然后运行 python states.py --find=0

注意，一开始的状态必须是刚进图、视角也没有改变的状态

几秒后角色会后退，然后前进。在角色前进时，你可以移动鼠标改变视角。

在地图中绕一圈，就能得到地图数据了。保存在imgs/maps/xxxxx目录下（可以按修改时间排序）

最好保持低头状态，减少高亮天空的干扰。

有怪的图最好用希儿战技，被锁定会影响小地图识别。

小地图上表示人物视角的淡蓝色扇形（探照灯）也会影响小地图白色边缘线的识别。因此尽量让探照灯少照射到白色边缘。

imgs/maps/xxxxx目录下会存在target.jpg，你可以用windows自带的画图打开它，然后在上面标记点（可以参考其它地图文件中的target.jpg）

靛蓝色：路径点 黄色：终点 绿色：交互点（问号点） 红色：怪点

----------------------------------------------------------------------------------------------

欢迎加入，欢迎反馈bug，QQ：3501801665
