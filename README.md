# WJSegmentMeunVc
a smiple menu change view controllers

     /* 创建WJSegmentMenuVc */
    WJSegmentMenuVc *segmentMenuVc = [[WJSegmentMenuVc alloc]initWithFrame:CGRectMake(0, 64, self.view.frame.size.width, 40)];
    [self.view addSubview:segmentMenuVc];
    
    /* 自定义设置(可不设置为默认值) */
    segmentMenuVc.backgroundColor = [UIColor colorWithRed:240/250.0 green:240/250.0 blue:240/250.0 alpha:1];
    segmentMenuVc.titleFont = [UIFont systemFontOfSize:13];
    segmentMenuVc.unlSelectedColor = [UIColor darkGrayColor];
    segmentMenuVc.selectedColor = [UIColor greenColor];
    segmentMenuVc.MenuVcSlideType = WJSegmentMenuVcSlideTypeSlide;
    segmentMenuVc.SlideColor = [UIColor greenColor];
    segmentMenuVc.advanceLoadNextVc = YES;
    
    /* 创建测试数据 */
    NSArray *titles = @[@"巴士",@"顺风车",@"快车",@"出租车",@"专车",@"代驾",@"试驾",@"其他"];
    oneVc      *vc1 = [[oneVc alloc]init];
    twoVc      *vc2 = [[twoVc alloc]init];
    threeVc    *vc3 = [[threeVc alloc]init];
    fourVc     *vc4 = [[fourVc alloc]init];
    fireVc     *vc5 = [[fireVc alloc]init];
    sixVc      *vc6 = [[sixVc alloc]init];
    sevenVc    *vc7 = [[sevenVc alloc]init];
    eigthVc    *vc8 = [[eigthVc alloc]init];
    NSArray *vcArr = @[vc1,vc2,vc3,vc4,vc5,vc6,vc7,vc8];
    
    /* 导入数据 */
    [segmentMenuVc addSubVc:vcArr subTitles:titles];
