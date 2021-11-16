token:   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

11.15
1.通过overfit的方法来验证模型方法，可能就100张以内。
2.模型的表面结果可能会影响对性能的判断，如centernet的两个分支，中心位置偏移和长宽的预测，表面结果有问题，有可能只是中心点的偏移出现问题和长宽没问题。
3.采用batchsize=1，是否对bn层这些有问题？是否可以实现overfit。

11.16
1.adu_msgs.git用来存储图片这些。
2.adu_services.git用于设备，imu这些的配置。
