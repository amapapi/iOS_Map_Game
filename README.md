手动部署：
1. 前往 http://lbs.amap.com/api/ios-sdk/download/ 下载最新的地图SDK (4.0版本以上需要基础SDK包)
2. 添加MAMapkit.framework (4.0版本需额外添加AMapFoundationKit.framework)
3. 引入MAMapkit.framework中的AMap.bundle
4. 使用[AMapServices sharedServices].apiKey = @"你的key"; (4.0以下版本使用[MAMapServices sharedServices].apiKey)。key申请地址:http://lbs.amap.com/dev/#/
5. 在viewControl中，使用MAMapView *mapview = [[MAMapView alloc] initWithFrame:self.view.bounds] 即可创建地图

自动部署：
参考：http://lbs.amap.com/api/ios-sdk/guide/buildproject/#t1