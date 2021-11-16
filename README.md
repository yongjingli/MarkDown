token:   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

11.15
1.通过overfit的方法来验证模型方法，可能就100张以内。
2.模型的表面结果可能会影响对性能的判断，如centernet的两个分支，中心位置偏移和长宽的预测，表面结果有问题，有可能只是中心点的偏移出现问题和长宽没问题。
3.采用batchsize=1，是否对bn层这些有问题？是否可以实现overfit。

11.16
1.adu_msgs.git用来存储图片这些。
2.adu_services.git用于设备，imu这些的配置。

3.对于person模型，前面也是用到一个focus操作
![image](https://user-images.githubusercontent.com/32613232/141955844-3105159b-a49d-4a5a-93fd-f7a3fbdf2554.png)

4.constexpr表示这玩意儿在编译期就可以算出来（前提是为了算出它所依赖的东西也是在编译期可以算出来的）。而const只保证了运行时不直接被修改（但这个东西仍然可能是个动态变量）

5.make_unique 同 unique_ptr 、auto_ptr 等一样，都是 smart pointer，可以取代new 并且无需 delete pointer，有助于代码管理。

6.mode 是指follow这些模式   camera_list 是指主，前后，左右这些相机

5.adu是指算法板子，msd是可行驶空间算法

6.每个相机main或者right，left作为一个独立的线程，每个线程独立创建一个newwork，通过percetion_mode进行控制，init进行初始化，然后通过start进行启动
