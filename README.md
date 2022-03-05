# -function shellSort(arr) {
    var len = arr.length,
        temp,
        gap = 1;
    while(gap < len/3) {          //动态定义间隔序列
        gap =gap*3+1;
    }
    for (gap; gap > 0; gap = Math.floor(gap/3)) {
        for (var i = gap; i < len; i++) {
            temp = arr[i];
            for (var j = i-gap; j >= 0 && arr[j] > temp; j-=gap) {
                arr[j+gap] = arr[j];
            }
            arr[j+gap] = temp;
        }
    }
    return arr;
}
<!DOCTYPE html>
<html lang="zh-cn">

<head>
    <meta charset="UTF-8">
    <title>飘城旅行</title>
    <link rel="stylesheet" type="text/css" href="css/style.css">
    <link rel="stylesheet" href="css/basic.css">

</head>

<body>
    <!--  头部导航 -->
    <header id="header">
        <div class="center">
            <h1 class="logo">瓢城旅行社</h1>
            <nav class="link">
                <ul>
                    <h2 class="none">网站导航</h2>
                    <li class="active"><a href="飘城旅行社门户.html">首页</a></li>
                    <li><a href="旅游咨询.html">旅游资讯</a></li>
                    <li><a href="机票订购.html">机票订购</a></li>
                    <li><a href="风景欣赏.html">风景欣赏</a></li>
                    <li><a href="公司简介.html">公司简介</a></li>
                </ul>
            </nav>
        </div>
    </header>
    <!--  搜索框  -->
    <div id="search">
        <div class="center"></div>
        <input type="text" class="search" placeholder="请输入旅游景点或城市">
        <button class="button">搜索</button>
    </div>
    <!-- 热门旅游 -->
    <div id="tour">
        <section class="center">
            <h2>热门旅游</h2>
            <p>国内旅游、国外旅游、自助旅游、自驾旅游、油轮签证、主题旅游等各种最新热门旅游推荐</p>
        </section>
        <figure>
            <img src="img/tour1.jpg" alt="">
            <figcaption>
                <strong class="title">&lt;曼谷-芭提雅6日游&gt;</strong> 包团特惠，超丰富景点，升级1晚国五，无自费，更赠送600元/成人自费券
                <div class="info">
                    <em class="sat">满意度 77%</em>
                    <span class="price">￥ <strong>2864</strong> 起</span>
                </div>
                <div class="type">国内长线</div>
            </figcaption>
        </figure>
        <figure>
            <img src="img/tour2.jpg" alt="马尔代夫双鱼岛Olhuveli4晚6日自助游">
            <figcaption>
                <strong class="title">&lt;马尔代夫双鱼岛Olhuveli4晚6日自助游&gt;</strong> 上海出发，机+酒包含:早晚餐+快艇
                <div class="info">
                    <em class="sat">满意度 97%</em>
                    <span class="price">¥ <strong>8039</strong> 起</span>
                </div>
                <div class="type">出境长线</div>
            </figcaption>
        </figure>
        <figure>
            <img src="img/tour3.jpg" alt="海南双飞5日游">
            <figcaption>
                <strong class="title">&lt;海南双飞5日游&gt;</strong> 含盐城接送，全程挂牌四星酒店，一价全含，零自费“自费项目”免费送
                <div class="info">
                    <em class="sat">满意度 90%</em>
                    <span class="price">¥ <strong>2709</strong> 起</span>
                </div>
                <div class="type">自助旅游</div>
            </figcaption>
        </figure>
        <figure>
            <img src="img/tour4.jpg" alt="富山-大阪-东京8日游">
            <figcaption>
                <strong class="title">&lt;富山-大阪-东京8日游&gt;</strong> 暑期亲子，2天自由，无导游安排自费项目，全程不强迫购物
                <div class="info">
                    <em class="sat">满意度 97%</em>
                    <span class="price">¥ <strong>9499</strong> 起</span>
                </div>
                <div class="type">自助旅游</div>
            </figcaption>
        </figure>
        <figure>
            <img src="img/tour5.jpg" alt="法瑞意德12日游">
            <figcaption>
                <strong class="title">&lt;法瑞意德12日游&gt;</strong> 4至5星，金色列车，少女峰，部分THE MALL
                <div class="info">
                    <em class="sat">满意度 97%</em>
                    <span class="price">¥ <strong>9199</strong> 起</span>
                </div>
                <div class="type">国内短线</div>
            </figcaption>
        </figure>
        <figure>
            <img src="img/tour6.jpg" alt="巴厘岛6日半自助游">
            <figcaption>
                <strong class="title">&lt;巴厘岛6日半自助游&gt;</strong> 蓝梦出海，独栋别墅，悦榕庄下午茶，纯玩
                <div class="info">
                    <em class="sat">满意度 95%</em>
                    <span class="price">¥ <strong>6488</strong> 起</span>
                </div>
                <div class="type">出境长线</div>
            </figcaption>
        </figure>
        <figure>
            <img src="img/tour7.jpg" alt="塞舌尔迪拜9日自助游">
            <figcaption>
                <strong class="title">&lt;塞舌尔迪拜9日自助游&gt;</strong> 一游两国，4晚塞舌尔，2晚迪拜，香港EK往返
                <div class="info">
                    <em class="sat">满意度 100%</em>
                    <span class="price">¥ <strong>9669</strong> 起</span>
                </div>
                <div class="type">游轮观光</div>
            </figcaption>
        </figure>
        <figure>
            <img src="img/tour8.jpg" alt="花样姐姐土耳其9日或10日游">
            <figcaption>
                <strong class="title">&lt;花样姐姐土耳其9日或10日游&gt;</strong> 最高立减3000！中餐六菜一汤+土耳其当地美食满足您挑剔味蕾
                <div class="info">
                    <em class="sat">满意度 93%</em>
                    <span class="price">¥ <strong>9999</strong> 起</span>
                </div>
                <div class="type">出境长线</div>
            </figcaption>

        </figure>
        <figure>
            <img src="img/tour9.jpg" alt="大阪-京都-箱根双飞6日游">
            <figcaption>
                <strong class="title">&lt;大阪-京都-箱根双飞6日游&gt;</strong> 盐城直飞，不走回头路，境外无自费，超值之旅
                <div class="info">
                    <em class="sat">满意度 100%</em>
                    <span class="price">¥ <strong>5284</strong> 起</span>
                </div>
                <div class="type">国内短线</div>
            </figcaption>
        </figure>

    </div>
    <!-- 底部 -->
    <footer id="footer">
        <div class="top">
            <div class="block left">
                <h2>合作伙伴</h2>
                <hr>
                <ul>
                    <li>途牛旅游网</li>
                    <li>驴妈妈旅游网</li>
                    <li>携程旅游</li>
                    <li>中国青年旅行社</li>
                </ul>
            </div>
            <div class="block center">
                <h2>旅游FAQ</h2>
                <hr>
                <ul>
                    <li>旅游合同签订方式？</li>
                    <li>儿童价是基于什么制定的？</li>
                    <li>旅游的线路品质怎么界定的？</li>
                    <li>单房差是什么？</li>
                    <li>旅游保险有那些种类？</li>
                </ul>
            </div>
            <div class="block right">
                <h2>联系方式</h2>
                <hr>
                <ul>
                    <li>微博：weibo.com/ycku</li>
                    <li>邮件：ycku@ycku.com</li>
                    <li>地址：江苏盐城无名路123 号</li>
                </ul>
            </div>
        </div>
        <div class="bottom">Copyright © YCKU 瓢城旅行社| 苏ICP 备120110119 号| 旅行社经营许可证：L-YC-BK12345</div>
    </footer>
    /**
    * 基数排序
    * 考虑负数的情况还可以参考： https://code.i-harness.com/zh-CN/q/e98fa9
    */
    public class RadixSort implements IArraySort {

    @Override
    public int[] sort(int[] sourceArray) throws Exception {
    // 对 arr 进行拷贝，不改变参数内容
    int[] arr = Arrays.copyOf(sourceArray, sourceArray.length);

    int maxDigit = getMaxDigit(arr);
    return radixSort(arr, maxDigit);
    }

    /**
    * 获取最高位数
    */
    private int getMaxDigit(int[] arr) {
    int maxValue = getMaxValue(arr);
    return getNumLenght(maxValue);
    }

    private int getMaxValue(int[] arr) {
    int maxValue = arr[0];
    for (int value : arr) {
    if (maxValue < value) { maxValue=value; } } return maxValue; } protected int getNumLenght(long num) { if (num==0) {
        return 1; } int lenght=0; for (long temp=num; temp !=0; temp /=10) { lenght++; } return lenght; } private int[]
        radixSort(int[] arr, int maxDigit) { int mod=10; int dev=1; for (int i=0; i < maxDigit; i++, dev *=10, mod *=10)
        { // 考虑负数的情况，这里扩展一倍队列数，其中 [0-9]对应负数，[10-19]对应正数 (bucket + 10) int[][] counter=new int[mod * 2][0]; for (int j=0;
        j < arr.length; j++) { int bucket=((arr[j] % mod) / dev) + mod; counter[bucket]=arrayAppend(counter[bucket],
        arr[j]); } int pos=0; for (int[] bucket : counter) { for (int value : bucket) { arr[pos++]=value; } } } return
        arr; } /** * 自动扩容，并保存数据 * * @param arr * @param value */ private int[] arrayAppend(int[] arr, int value) {
        arr=Arrays.copyOf(arr, arr.length + 1); arr[arr.length - 1]=value; return arr; } } </body>

</html>
