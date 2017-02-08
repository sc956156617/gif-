# gif-

使用引入头文件，签订代理

<SCLoopDelegate>

@property (nonatomic, strong) SCLoop *loop;


self.loop = [[SCLoop alloc] initWithFrame:CGRectMake(0, 200, [UIScreen mainScreen].bounds.size.width, 200)];
[self.view addSubview:self.loop];
self.loop.SCDelegate = self;
self.loop.time = 2;


//设置pagecontrolor颜色
[self.loop setPageColor:[UIColor blueColor] andCurrentPageColor:[UIColor redColor]];
//支持gif动态图
self.loop.imageArray = @[@"http://i3.hoopchina.com.cn/u/1212/19/386/16355386/2d4f91db_530x.gif",
@"http://pic2015.5442.com/2015/1118/8/18.jpg%21960.jpg",
@"http://tpic.home.news.cn/xhCloudNewsPic/xhpic1501/M07/1B/9C/wKhTlVeRvImESafHAAAAAGHVmt8775.gif",
@"http://www.pp3.cn/uploads/201606/2016060401.jpg"];