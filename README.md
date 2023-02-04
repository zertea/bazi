# 简介

- bazi.py 八字排盘，能比常用的排盘更清晰地显示冲、合、刑等关系，计算五行分数，附加《三命通会》等命理评判
- luohou.py 计算罗喉日时,用于提示风水师何时慎用罗盘。
- shengxiao.py 用户生肖合婚等。

软件部署定制技术支持及批八字学八字：微信或钉钉pythontesting

# 命理书籍(访问密码: 2274) 点击“普通下载”下面的“立即下载”可浏览器下载

- [三命通会.pdf 文字版本](https://url97.ctfile.com/f/18113597-649595228-10f29e?p=2274) 
- [图解三命通会 第3部论命精要 - 2009.pdf](https://url97.ctfile.com/f/18113597-649699807-d4cd2a?p=2274)
- [图解三命通会 第2部吉凶推断 - 2009.pdf](https://url97.ctfile.com/f/18113597-649699779-b87c3c?p=2274)
- [图解三命通会 第1部 八字神煞 2009 -扫描.pdf](https://url97.ctfile.com/f/18113597-649699750-44b525?p=2274)
- [千里命稿.pdf 古籍图片版本](https://url97.ctfile.com/f/18113597-612723542-319345?p=2274)
- [千里命稿.pdf 文字版本](https://url97.ctfile.com/f/18113597-612723571-e22c74?p=2274)
- [千里命稿.pdf 古籍图片版本](https://url97.ctfile.com/f/18113597-612723542-319345?p=2274)
- [千里命稿.pdf 文字版本](https://url97.ctfile.com/f/18113597-612723571-e22c74?p=2274)
- [朱鹊桥 -鹊桥命理【一】.pdf](https://url97.ctfile.com/f/18113597-723734086-4b23bf?p=2274)
- [朱鹊桥 -鹊桥命理【四】.pdf](https://url97.ctfile.com/f/18113597-723734085-b3d415?p=2274)
- [命运的求索 中国命理学简史及推演方法 (陆致极.pdf ](https://url97.ctfile.com/f/18113597-756319536-0f0ae7?p=2274)
- [中国命理学史论 (陆致极).pdf ](https://url97.ctfile.com/f/18113597-756319535-ef2812?p=2274)
- [八字命理动态分析教程 (陆致极).pdf ](https://url97.ctfile.com/f/18113597-756319531-48e4d9?p=2274)
- [又一种“基因”的探索 (陆致极).pdf ](https://url97.ctfile.com/f/18113597-756319530-dd8028?p=2274)
- [八字命理學進階教程 (陆致极).pdf ](https://url97.ctfile.com/f/18113597-756319525-a897c1?p=2274)
- [梁湘润-星相书简法卷宇册.pdf ](https://url97.ctfile.com/f/18113597-756715812-4ca590?p=2274)
- [梁湘润-星相书简法卷 天册.pdf](https://url97.ctfile.com/f/18113597-756715812-4ca590?p=2274)
- [梁湘润 - 星相书简法卷 黄册.pdf ](https://url97.ctfile.com/f/18113597-756715796-203c11?p=2274)
- [梁湘润 星相书简法卷地册.pdf](https://url97.ctfile.com/f/18113597-756715783-34e1f8?p=2274)

# 安装
- 安裝依赖库

```python
pip install  sxtwl bidict
```

Windows下如果安装sxtwl报错，安装 [BuildTools_Full.exe](https://url97.ctfile.com/f/18113597-800958828-d3b94d?p=2274) 点击普通下载，不用注册，访问密码: 2274
注意：sxtwl可能不支持python3.11。 Linux下的兼容性会好很多。

- linux打开终端或windows打开cmd或git的bash或powercmd等工具

进入到代码所在目录。


# 使用

- 生肖合婚

```python
$ python shengxiao.py 虎
你的生肖是： 虎
你的年支是： 寅
================================================================================
合生肖是合八字的一小部分，有一定参考意义，但是不是全部。
合婚请以八字为准，技术支持：钉钉或微信pythontesting
以下为相合的生肖：
================================================================================

与你三合的生肖：马狗
与你六合的生肖：猪
与你三会的生肖：兔龙
================================================================================
以下为不合的生肖：
================================================================================

与你相冲的生肖：猴
你刑的生肖：蛇
被你刑的生肖：猴
与你相害的生肖：蛇
与你相破的生肖：猪
================================================================================
如果生肖同时在你的合与不合中，则做加减即可。
比如猪对于虎，有一个相破，有一六合，抵消就为平性。

```


- 计算罗喉日时

```python
$ python luohou.py 
公历:2021年3月23日	农历:2021年二月十一日   	辛丑-辛卯-庚午	杀师时:卯5-7申15-17
公历:2021年3月24日	农历:2021年二月十二日   	辛丑-辛卯-辛未	杀师时:午11-13辰7-9
公历:2021年3月25日	农历:2021年二月十三日   	辛丑-辛卯-壬申	杀师时:戌19-21丑1-3
公历:2021年3月26日	农历:2021年二月十四日   	辛丑-辛卯-癸酉	杀师时:子23-1午11-13
公历:2021年3月27日	农历:2021年二月十五日   	辛丑-辛卯-甲戌	杀师时:卯5-7午11-13 	年猴:丑年甲戌日 
...
```


- 八字排盘

```python

$ python bazi.py -h
usage: bazi.py [-h] [-b] [-g] [-r] [-n] [--version] year month day time

positional arguments:
  year        year
  month       month
  day         day
  time        time

optional arguments:
  -h, --help  show this help message and exit
  -b          直接输入八字
  -g          是否采用公历
  -r          是否为闰月，仅仅使用于农历
  -n          是否为女，默认为男
  --version   show program's version number and exit


# -- 左宗棠八字

  python bazi.py 1812 11 10 4 -g

男命
======================================
公历:   1812年11月10日
农历:   1812年10月7日 穿=害
------------------------------------------------------------------------------------------------------------------------
墓库： {辰: 水土, 戌: 火土, 丑: 金, 未: 木} 解读:钉ding或v信pythontesting 壬申 辛亥 丙午 庚寅
甲己-中正土  乙庚-仁义金  丙辛-威制水  丁壬-淫慝木  戊癸-无情火   三会: {亥子丑: 水, 寅卯辰: 木, 巳午未: 火, 申酉戌: 金}
========================================================================================================================
壬 辛 丙 庚       杀 财 -- 才       申子辰:水 寅  巳酉丑:金 亥  寅午戌:火 申  亥卯未:木 巳
申 亥 午 寅       才 杀 劫 枭       生：寅申巳亥 败：子午卯酉　库：辰戌丑未    子丑土 寅亥木 卯戌火 酉辰金 申巳水 未午土
------------------------------------------------------------------------------------------------------------------------
　　　【年】-5:-2亥　　　　　　【月】-3:-5酉　　　　　　　【日】6:6　　　　　　　　【时】-1:3申　　　　
------------------------------------------------------------------------------------------------------------------------
壬＋水【杀】冲丙　　　　　　　辛－金【财】合丙　　　　　　　丙＋火合辛冲壬　　　　　　　　庚＋金【才】　　　　　　　　　
申＋病【长】　　　　　　　　　亥－绝【沐】　　　　　　　　　午＋帝　　　　　　　　　　　　寅＋长【绝】空　　　　　　　　
庚金才　壬水杀　戊土食　　　　壬水杀　甲木枭　　　　　　　　丁火劫　己土伤　　　　　　　　甲木枭　丙火比　戊土食　　　　
冲　　　　　　　　　　　　　　六：寅　暗　　　　　　　　　　合：寅　暗　　　　　　　　　　冲　被刑：申　合：午　六：亥　
害：亥　　　　　　　　　　　　害：申　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　　
↑剑锋金　　　　　　　　　　　 ↓钗钏金－亡　　　　　　　　　 =天河水　　　　　　　　　　　 →松柏木　　　　　　　　　　　
驿马　文昌　　　　　　　　　　 孤辰　劫煞　天乙　　　　　　　 阳刃　　　　　　　　　　　　 红艳　　　　　　　　　　　　
------------------------------------------------------------------------------------------------------------------------
甲:枭 祖父-绝 长 死 建  乙:印 母亲-胎 死 长 帝  丙:比 兄弟-病 绝 帝 长  丁:劫 姐妹-沐 胎 建 死  戊:食 下属-病 绝 帝 长
己:伤 孙女-沐 胎 建 死  庚:才 父亲-建 病 沐 绝  辛:财 妻子-帝 沐 病 胎  壬:杀 儿子-长 建 胎 病  癸:官 女儿-死 帝 绝 沐

五行分数 {'金': 15, '木': 11, '水': 17, '火': 12, '土': 5}   八字强弱： 23 通常>29为强，需要参考月份、坐支等 weak: False
湿度分数 -6 正为暖燥，负为寒湿，正常区间[-6,6] 拱库气： []
甲[枭]-11   乙[印]-0   丙[比]-7   丁[劫]-5   戊[食]-2   己[伤]-3   庚[才]-10   辛[财]-5   壬[杀]-17   癸[官]-0
------------------------------------------------------------------------------------------------------------------------
日主专位劫财，壬子和丙午，晚婚。不透天干，一般是眼光高、独立性强。女性婚后通常还有自己的事业,能办事。
日支劫：男的克妻。如再透月或时天干，有严重内忧外患。
偏印坐绝，或者天干坐偏印为绝，难以得志。费力不讨好。
偏印在时：女与后代分居；男50以前奠定基础，晚年享清福。
偏财明现天干，不论是否有根:财富外人可见;实际财力不及外观一半。没钱别人都不相信;协助他人常超过自己的能力
偏财出天干，又与天月德贵人同一天干者。在年月有声明远扬的父亲，月时有聪慧的红颜知己。
偏财透天干，四柱没有刑冲，长寿。女子为孝顺女，主要针对年月。时柱表示中年以后有自己的事业，善于理财。
财格基础80:比劫用食伤通关或官杀制；身弱有比劫仍然用食伤通关。
偏财透天干，讲究原则，不拘小节。喜奉承，善于享受。财格基础80
偏财和七杀并位，地支又有根，父子外合心不合。因为偏财生杀攻身。偏财七杀在日时，则为有难伺候的女朋友。
偏财根透年柱，家世良好，且能承受祖业。
偏财坐阳刃劫财,可做父缘薄，也可幼年家贫。也可以父先亡，要参考第一大运。
官或杀与财并行透出，女压夫，财生官杀，老公压力大。
七杀是非多。但是对男人有时是贵格。比如毛主席等。七杀坐刑或冲，夫妻不和。成格基础85可杀生印或食制印、身杀两停、阳刃驾杀。
杀格：喜食神制，要食在前，杀在后。阳刃驾杀：杀在前，刃在后。身杀两停：比如甲寅日庚申月。杀印相生，忌食同成格。
年干七杀，早年不好。或家里穷或身体不好。
七杀地支有根时要有阳刃强为佳。杀身两停。
财生杀，如果不是身弱有印，不佳。
杀多者如果无制，性格刚强。打抱不平，不易听人劝。女的喜欢佩服的人。


大运
========================================================================================================================
9        壬子 桑柘木    杀:壬＋冲丙　　　　　子＋胎 - 癸水官　　　　　　　　　　　　 会:亥  合:申  冲:午
  9 1821 辛巳 白蜡金    财:辛－合丙　　　　　巳－建 - 丙火比　戊土食　庚金才　　　　 被刑:寅  害:寅  冲:亥  六:申  刑:申  会:午
 10 1822 壬午 杨柳木    杀:壬＋冲丙　　　　　午＋帝 - 丁火劫　己土伤　　　　　　　　 合:寅  刑:午  冲:子  暗:亥  被刑:午
 11 1823 癸未 杨柳木    官:癸－　　　　　　　未－衰 - 己土伤　丁火劫　乙木印　　　　 害:子  六:午  合:亥  会:午
 12 1824 甲申 井泉水    枭:甲＋冲庚　　　　　申＋病 - 庚金才　壬水杀　戊土食　　　　 合:子  害:亥  冲:寅  刑:寅
 13 1825 乙酉 井泉水    印:乙－合庚冲辛　　　酉－死 - 辛金财　　　　　　　　　　　　 会:申
 14 1826 丙戌 屋上土    比:丙＋合辛冲壬　　　戌＋墓 - 戊土食　辛金财　丁火劫　　　　 合:寅  会:申  合:午
 15 1827 丁亥 屋上土    劫:丁－合壬　　　　　亥－绝 - 壬水杀　甲木枭　　　　　　　　 刑:亥  害:申  六:寅  暗:午  被刑:亥  会:子
 16 1828 戊子 霹雳火    食:戊＋　　　　　　　子＋胎 - 癸水官　　　　　　　　　　　　 会:亥  合:申  冲:午
 17 1829 己丑 霹雳火    伤:己－　　　　　　　丑－养 - 己土伤　癸水官　辛金财　　　　 会:亥  六:子  暗:寅  害:午  会:子
 18 1830 庚寅 松柏木 *  才:庚＋　　　　　　空寅＋长 - 甲木枭　丙火比　戊土食　　　　 冲:申  被刑:申  六:亥  合:午
19       癸丑 桑柘木    官:癸－　　　　　　　丑－养 - 己土伤　癸水官　辛金财　　　　 暗:寅  会:亥  害:午
 19 1831 辛卯 松柏木    财:辛－合丙　　　　空卯－沐 - 乙木印　　　　　　　　　　　　 暗:申  合:亥  会:寅
 20 1832 壬辰 长流水    杀:壬＋冲丙　　　　　辰＋冠 - 戊土食　乙木印　癸水官　　　　 合:申  会:寅
 21 1833 癸巳 长流水    官:癸－　　　　　　　巳－建 - 丙火比　戊土食　庚金才　　　　 被刑:寅  合:丑  害:寅  冲:亥  六:申  刑:申  会:午
 22 1834 甲午 砂中金    枭:甲＋冲庚　　　　　午＋帝 - 丁火劫　己土伤　　　　　　　　 合:寅  刑:午  暗:亥  害:丑  被刑:午
 23 1835 乙未 砂中金    印:乙－合庚冲辛　　　未－衰 - 己土伤　丁火劫　乙木印　　　　 刑:丑  六:午  合:亥  冲:丑  会:午
 24 1836 丙申 山下火    比:丙＋合辛冲壬　　　申＋病 - 庚金才　壬水杀　戊土食　　　　 害:亥  冲:寅  刑:寅
 25 1837 丁酉 山下火    劫:丁－合壬冲癸　　　酉－死 - 辛金财　　　　　　　　　　　　 合:丑  会:申
 26 1838 戊戌 平地木    食:戊＋合癸　　　　　戌＋墓 - 戊土食　辛金财　丁火劫　　　　 合:寅  被刑:丑  会:申  合:午
 27 1839 己亥 平地木    伤:己－　　　　　　　亥－绝 - 壬水杀　甲木枭　　　　　　　　 刑:亥  害:申  六:寅  暗:午  会:丑  被刑:亥
 28 1840 庚子 壁上土    才:庚＋　　　　　　　子＋胎 - 癸水官　　　　　　　　　　　　 会:亥  合:申  会:丑  六:丑  冲:午
29       甲寅 大溪水    枭:甲＋冲庚　　　　空寅＋长 - 甲木枭　丙火比　戊土食　　　　 冲:申  被刑:申  六:亥  合:午  破:亥
 29 1841 辛丑 壁上土    财:辛－合丙　　　　　丑－养 - 己土伤　癸水官　辛金财　　　　 暗:寅  会:亥  害:午
 30 1842 壬寅 金泊金    杀:壬＋冲丙　　　　空寅＋长 - 甲木枭　丙火比　戊土食　　　　 冲:申  被刑:申  六:亥  合:午
 31 1843 癸卯 金泊金    官:癸－　　　　　　空卯－沐 - 乙木印　　　　　　　　　　　　 暗:申  合:亥  会:寅
 32 1844 甲辰 覆灯火    枭:甲＋冲庚　　　　　辰＋冠 - 戊土食　乙木印　癸水官　　　　 合:申  会:寅
 33 1845 乙巳 覆灯火    印:乙－合庚冲辛　　　巳－建 - 丙火比　戊土食　庚金才　　　　 被刑:寅  害:寅  冲:亥  六:申  刑:申  会:午
 34 1846 丙午 天河水 *  比:丙＋合辛冲壬　　　午＋帝 - 丁火劫　己土伤　　　　　　　　 合:寅  暗:亥  被刑:午  刑:午
 35 1847 丁未 天河水    劫:丁－合壬　　　　　未－衰 - 己土伤　丁火劫　乙木印　　　　 六:午  合:亥  会:午
 36 1848 戊申 大驿土    食:戊＋　　　　　　　申＋病 - 庚金才　壬水杀　戊土食　　　　 害:亥  冲:寅  刑:寅
 37 1849 己酉 大驿土    伤:己－合甲　　　　　酉－死 - 辛金财　　　　　　　　　　　　 会:申
 38 1850 庚戌 钗钏金    才:庚＋冲甲　　　　　戌＋墓 - 戊土食　辛金财　丁火劫　　　　 合:寅  会:申  合:午
39       乙卯 大溪水    印:乙－合庚冲辛　　空卯－沐 - 乙木印　　　　　　　　　　　　 暗:申  破:午  合:亥  会:寅
 39 1851 辛亥 钗钏金 *  财:辛－合丙冲乙　　　亥－绝 - 壬水杀　甲木枭　　　　　　　　 刑:亥  害:申  六:寅  暗:午  被刑:亥  合:卯
 40 1852 壬子 桑柘木    杀:壬＋冲丙　　　　　子＋胎 - 癸水官　　　　　　　　　　　　 会:亥  合:申  刑:卯  被刑:卯  冲:午
 41 1853 癸丑 桑柘木    官:癸－　　　　　　　丑－养 - 己土伤　癸水官　辛金财　　　　 暗:寅  会:亥  害:午
 42 1854 甲寅 大溪水    枭:甲＋冲庚　　　　空寅＋长 - 甲木枭　丙火比　戊土食　　　　 冲:申  被刑:申  会:卯  六:亥  合:午
 43 1855 乙卯 大溪水    印:乙－合庚冲辛　　空卯－沐 - 乙木印　　　　　　　　　　　　 暗:申  合:亥  会:寅
 44 1856 丙辰 砂中土    比:丙＋合辛冲壬　　　辰＋冠 - 戊土食　乙木印　癸水官　　　　 合:申  会:卯  害:卯  会:寅
 45 1857 丁巳 砂中土    劫:丁－合壬　　　　　巳－建 - 丙火比　戊土食　庚金才　　　　 被刑:寅  害:寅  冲:亥  六:申  刑:申  会:午
 46 1858 戊午 天上火    食:戊＋　　　　　　　午＋帝 - 丁火劫　己土伤　　　　　　　　 合:寅  暗:亥  被刑:午  刑:午
 47 1859 己未 天上火    伤:己－　　　　　　　未－衰 - 己土伤　丁火劫　乙木印　　　　 六:午  合:卯  合:亥  会:午
 48 1860 庚申 石榴木    才:庚＋合乙　　　　　申＋病 - 庚金才　壬水杀　戊土食　　　　 暗:卯  害:亥  冲:寅  刑:寅
49       丙辰 砂中土    比:丙＋合辛冲壬　　　辰＋冠 - 戊土食　乙木印　癸水官　　　　 合:申  会:寅
 49 1861 辛酉 石榴木    财:辛－合丙　　　　　酉－死 - 辛金财　　　　　　　　　　　　 六:辰  会:申
 50 1862 壬戌 大海水    杀:壬＋冲丙　　　　　戌＋墓 - 戊土食　辛金财　丁火劫　　　　 冲:辰  合:寅  会:申  合:午
 51 1863 癸亥 大海水    官:癸－　　　　　　　亥－绝 - 壬水杀　甲木枭　　　　　　　　 刑:亥  害:申  六:寅  暗:午  被刑:亥
 52 1864 甲子 海中金    枭:甲＋冲庚　　　　　子＋胎 - 癸水官　　　　　　　　　　　　 合:辰  会:亥  合:申  冲:午
 53 1865 乙丑 海中金    印:乙－合庚冲辛　　　丑－养 - 己土伤　癸水官　辛金财　　　　 暗:寅  会:亥  害:午
 54 1866 丙寅 炉中火    比:丙＋合辛冲壬　　空寅＋长 - 甲木枭　丙火比　戊土食　　　　 冲:申  会:辰  被刑:申  六:亥  合:午
 55 1867 丁卯 炉中火    劫:丁－合壬　　　　空卯－沐 - 乙木印　　　　　　　　　　　　 暗:申  会:辰  合:亥  会:寅  害:辰
 56 1868 戊辰 大林木    食:戊＋　　　　　　　辰＋冠 - 戊土食　乙木印　癸水官　　　　 刑:辰  被刑:辰  合:申  会:寅
 57 1869 己巳 大林木    伤:己－　　　　　　　巳－建 - 丙火比　戊土食　庚金才　　　　 被刑:寅  害:寅  冲:亥  六:申  刑:申  会:午
 58 1870 庚午 路旁土    才:庚＋　　　　　　　午＋帝 - 丁火劫　己土伤　　　　　　　　 合:寅  暗:亥  被刑:午  刑:午
59       丁巳 砂中土    劫:丁－合壬　　　　　巳－建 - 丙火比　戊土食　庚金才　　　　 被刑:寅  害:寅  破:申  冲:亥  六:申  刑:申  会:午
 59 1871 辛未 路旁土    财:辛－合丙　　　　　未－衰 - 己土伤　丁火劫　乙木印　　　　 六:午  会:巳  合:亥  会:午
 60 1872 壬申 剑锋金 *  杀:壬＋合丁冲丙　　　申＋病 - 庚金才　壬水杀　戊土食　　　　 被刑:巳  害:亥  冲:寅  六:巳  刑:寅
 61 1873 癸酉 剑锋金    官:癸－冲丁　　　　　酉－死 - 辛金财　　　　　　　　　　　　 合:巳  会:申
 62 1874 甲戌 山头火    枭:甲＋冲庚　　　　　戌＋墓 - 戊土食　辛金财　丁火劫　　　　 合:寅  会:申  合:午
 63 1875 乙亥 山头火    印:乙－合庚冲辛　　　亥－绝 - 壬水杀　甲木枭　　　　　　　　 刑:亥  害:申  六:寅  暗:午  被刑:亥  冲:巳
 64 1876 丙子 涧下水    比:丙＋合辛冲壬　　　子＋胎 - 癸水官　　　　　　　　　　　　 会:亥  合:申  冲:午
 65 1877 丁丑 涧下水    劫:丁－合壬　　　　　丑－养 - 己土伤　癸水官　辛金财　　　　 暗:寅  会:亥  合:巳  害:午
 66 1878 戊寅 城头土    食:戊＋　　　　　　空寅＋长 - 甲木枭　丙火比　戊土食　　　　 冲:申  刑:巳  害:巳  被刑:申  六:亥  合:午
 67 1879 己卯 城头土    伤:己－　　　　　　空卯－沐 - 乙木印　　　　　　　　　　　　 暗:申  合:亥  会:寅
 68 1880 庚辰 白蜡金    才:庚＋　　　　　　　辰＋冠 - 戊土食　乙木印　癸水官　　　　 合:申  会:寅
69       戊午 天上火    食:戊＋　　　　　　　午＋帝 - 丁火劫　己土伤　　　　　　　　 合:寅  暗:亥  被刑:午  刑:午
 69 1881 辛巳 白蜡金    财:辛－合丙　　　　　巳－建 - 丙火比　戊土食　庚金才　　　　 被刑:寅  害:寅  冲:亥  六:申  刑:申  会:午
 70 1882 壬午 杨柳木    杀:壬＋冲丙　　　　　午＋帝 - 丁火劫　己土伤　　　　　　　　 合:寅  暗:亥  被刑:午  刑:午
 71 1883 癸未 杨柳木    官:癸－合戊　　　　　未－衰 - 己土伤　丁火劫　乙木印　　　　 六:午  合:亥  会:午
 72 1884 甲申 井泉水    枭:甲＋冲庚　　　　　申＋病 - 庚金才　壬水杀　戊土食　　　　 害:亥  冲:寅  刑:寅
 73 1885 乙酉 井泉水    印:乙－合庚冲辛　　　酉－死 - 辛金财　　　　　　　　　　　　 会:申
 74 1886 丙戌 屋上土    比:丙＋合辛冲壬　　　戌＋墓 - 戊土食　辛金财　丁火劫　　　　 合:寅  会:申  合:午
 75 1887 丁亥 屋上土    劫:丁－合壬　　　　　亥－绝 - 壬水杀　甲木枭　　　　　　　　 刑:亥  害:申  六:寅  暗:午  被刑:亥
 76 1888 戊子 霹雳火    食:戊＋　　　　　　　子＋胎 - 癸水官　　　　　　　　　　　　 会:亥  合:申  冲:午
 77 1889 己丑 霹雳火    伤:己－　　　　　　　丑－养 - 己土伤　癸水官　辛金财　　　　 暗:寅  会:亥  害:午
 78 1890 庚寅 松柏木 *  才:庚＋　　　　　　空寅＋长 - 甲木枭　丙火比　戊土食　　　　 冲:申  被刑:申  六:亥  合:午
79       己未 天上火    伤:己－　　　　　　　未－衰 - 己土伤　丁火劫　乙木印　　　　 六:午  合:亥  会:午
 79 1891 辛卯 松柏木    财:辛－合丙　　　　空卯－沐 - 乙木印　　　　　　　　　　　　 暗:申  合:未  合:亥  会:寅
 80 1892 壬辰 长流水    杀:壬＋冲丙　　　　　辰＋冠 - 戊土食　乙木印　癸水官　　　　 合:申  会:寅
 81 1893 癸巳 长流水    官:癸－　　　　　　　巳－建 - 丙火比　戊土食　庚金才　　　　 被刑:寅  害:寅  会:未  冲:亥  六:申  刑:申  会:午
 82 1894 甲午 砂中金    枭:甲＋合己冲庚　　　午＋帝 - 丁火劫　己土伤　　　　　　　　 合:寅  刑:午  会:未  暗:亥  六:未  被刑:午
 83 1895 乙未 砂中金    印:乙－合庚冲辛　　　未－衰 - 己土伤　丁火劫　乙木印　　　　 六:午  合:亥  会:午
 84 1896 丙申 山下火    比:丙＋合辛冲壬　　　申＋病 - 庚金才　壬水杀　戊土食　　　　 害:亥  冲:寅  刑:寅
 85 1897 丁酉 山下火    劫:丁－合壬　　　　　酉－死 - 辛金财　　　　　　　　　　　　 会:申
 86 1898 戊戌 平地木    食:戊＋　　　　　　　戌＋墓 - 戊土食　辛金财　丁火劫　　　　 合:寅  刑:未  会:申  合:午
 87 1899 己亥 平地木    伤:己－　　　　　　　亥－绝 - 壬水杀　甲木枭　　　　　　　　 刑:亥  合:未  害:申  六:寅  暗:午  被刑:亥
 88 1900 庚子 壁上土    才:庚＋　　　　　　　子＋胎 - 癸水官　　　　　　　　　　　　 会:亥  合:申  害:未  冲:午
89       庚申 石榴木    才:庚＋　　　　　　　申＋病 - 庚金才　壬水杀　戊土食　　　　 害:亥  冲:寅  刑:寅
 89 1901 辛丑 壁上土    财:辛－合丙　　　　　丑－养 - 己土伤　癸水官　辛金财　　　　 暗:寅  会:亥  害:午
 90 1902 壬寅 金泊金    杀:壬＋冲丙　　　　空寅＋长 - 甲木枭　丙火比　戊土食　　　　 冲:申  被刑:申  六:亥  合:午
 91 1903 癸卯 金泊金    官:癸－　　　　　　空卯－沐 - 乙木印　　　　　　　　　　　　 暗:申  合:亥  会:寅
 92 1904 甲辰 覆灯火    枭:甲＋冲庚　　　　　辰＋冠 - 戊土食　乙木印　癸水官　　　　 合:申  会:寅
 93 1905 乙巳 覆灯火    印:乙－合庚冲辛　　　巳－建 - 丙火比　戊土食　庚金才　　　　 被刑:寅  害:寅  冲:亥  六:申  刑:申  会:午
 94 1906 丙午 天河水 *  比:丙＋合辛冲壬　　　午＋帝 - 丁火劫　己土伤　　　　　　　　 合:寅  暗:亥  被刑:午  刑:午
 95 1907 丁未 天河水    劫:丁－合壬　　　　　未－衰 - 己土伤　丁火劫　乙木印　　　　 六:午  合:亥  会:午
 96 1908 戊申 大驿土    食:戊＋　　　　　　　申＋病 - 庚金才　壬水杀　戊土食　　　　 害:亥  冲:寅  刑:寅
 97 1909 己酉 大驿土    伤:己－　　　　　　　酉－死 - 辛金财　　　　　　　　　　　　 会:申
 98 1910 庚戌 钗钏金    才:庚＋　　　　　　　戌＋墓 - 戊土食　辛金财　丁火劫　　　　 合:寅  会:申  合:午
99       辛酉 石榴木    财:辛－合丙　　　　　酉－死 - 辛金财　　　　　　　　　　　　 会:申
 99 1911 辛亥 钗钏金 *  财:辛－合丙　　　　　亥－绝 - 壬水杀　甲木枭　　　　　　　　 刑:亥  害:申  六:寅  暗:午  被刑:亥
100 1912 壬子 桑柘木    杀:壬＋冲丙　　　　　子＋胎 - 癸水官　　　　　　　　　　　　 会:亥  合:申  冲:午
101 1913 癸丑 桑柘木    官:癸－　　　　　　　丑－养 - 己土伤　癸水官　辛金财　　　　 暗:寅  会:亥  害:午  合:酉
102 1914 甲寅 大溪水    枭:甲＋冲庚　　　　空寅＋长 - 甲木枭　丙火比　戊土食　　　　 冲:申  被刑:申  六:亥  合:午
103 1915 乙卯 大溪水    印:乙－合庚冲辛　　空卯－沐 - 乙木印　　　　　　　　　　　　 暗:申  冲:酉  合:亥  会:寅
104 1916 丙辰 砂中土    比:丙＋合辛冲壬　　　辰＋冠 - 戊土食　乙木印　癸水官　　　　 六:酉  合:申  会:寅
105 1917 丁巳 砂中土    劫:丁－合壬　　　　　巳－建 - 丙火比　戊土食　庚金才　　　　 被刑:寅  害:寅  冲:亥  六:申  合:酉  刑:申  会:午
106 1918 戊午 天上火    食:戊＋　　　　　　　午＋帝 - 丁火劫　己土伤　　　　　　　　 合:寅  暗:亥  被刑:午  刑:午
107 1919 己未 天上火    伤:己－　　　　　　　未－衰 - 己土伤　丁火劫　乙木印　　　　 六:午  合:亥  会:午
108 1920 庚申 石榴木    才:庚＋　　　　　　　申＋病 - 庚金才　壬水杀　戊土食　　　　 会:酉  害:亥  冲:寅  刑:寅
109      壬戌 大海水    杀:壬＋冲丙　　　　　戌＋墓 - 戊土食　辛金财　丁火劫　　　　 合:寅  会:申  合:午
119      癸亥 大海水    官:癸－　　　　　　　亥－绝 - 壬水杀　甲木枭　　　　　　　　 刑:亥  害:申  六:寅  破:寅  暗:午  被刑:亥
9.0
星宿 ('危', '') ('危', '吉事不取的日子。 宜：入殓、破土、火化、进塔、安葬。 忌：入宅嫁娶诸吉事。')
========================================================================================================================
格局: 杀         | 玉堂贵人： 亥 学堂: 寅


------------------------------------------------------------------------------------------------------------------------
出身: 一般
财少身强，柱有比劫，不为福

杀(偏官)分析 **** 喜:身旺  印绶  合煞  食制 羊刃  比  逢煞看印及刃  以食为引   忌：身弱  财星  正官  刑冲  入墓
一曰偏官 二曰七煞 三曰五鬼 四曰将星 五曰孤极星 原有制伏,煞出为福,原无制伏,煞出为祸   性情如虎，急躁如风,尤其是七杀为丙、丁火时。
坐长生、临官、帝旺,更多带比同类相扶,则能化鬼为官,化煞为权,行运引至印乡,必发富贵。倘岁运再遇煞地,祸不旋踵。
七杀喜酒色而偏争好斗、爱轩昂而扶弱欺强
======================================
逢煞看财,如身强煞弱,有财星则吉,身弱煞强,有财引鬼盗气,非贫则夭;
有阳刃配合,即《经》云:煞无刃不显,逢煞看刃是也。
七煞重逢
七煞遇长生乙位，女招贵夫。

------------------------------------------------------------------------------------------------------------------------
========================================================================================================================
你属: 丙 特点：-- 电 冶 禄巳 火无西向

年份: 申 特点：-- 名都 帝王所居；申宫壬水生 亥时，乃地天交泰


羊刃: 丙 午
======================参考：https://www.jianshu.com/p/c503f7b3ed04
羊刃重重又见禄，富贵饶金玉。 官、印相助福相资。
文星贵人:  丙 申


五行缺土的建议参见 http://t.cn/E6zwOMq


命
=========================

    六丙日生时庚寅，学堂生气助其身；运中有合通金局，必是荣华富贵人。
    丙日庚寅时，生气学堂，丙寅上长生，文章秀气；丙以庚辛为财，寅上庚绝丙旺。若通月气金局者财旺，富贵双全，喜西方运；不通局者财薄。

    丙庚相合遇寅时，险难消除福自随；运至寒门名将相，时来平步上云梯。
    丙日庚寅时准，双亲衰旺离乡。妻儿早害晚荣昌，白虎归山正旺。木有成林松柏，生涯广聚财粮。堆金积玉满高堂，共羡人言上样。

    丙子日庚寅时,生子月,近贵。癸酉月,行水木运,高贵;火木运,五品以上贵。未申、癸午年月,身居武职,大贵,寿浅。

    丙寅日庚寅时,贵不久。生酉申年月,世裔冷职。子丑寅未,贵显。纯寅尤吉。

    丙辰日庚寅时,生寅午戌未年月,妻贤子孝,富贵双全。申子,行北运,大贵。酉丑,富。

    丙午日庚寅时,年月无壬癸子未巳字,飞天禄马,贵。巳酉丑申,主文学,不贵即富。未月,伤官。辰月,先贫后富。亥月,行西运,贵显。

    丙申日庚寅时,亥卯未、申子辰二局,官印两旺,大贵。巳丑财局,吉。寅午戌火局,平。

    丙戌日庚寅时,生亥子月,贵显。申酉年月,行北方运; 寅午戌,行官鬼运,俱大贵。若运临死绝,即入黄泉无疑。

======================================
阴杀:话少,性格柔和
男:因女致祸、因色致祸; 女:赔货
偏印因偏财而不懒！


```


-- 鸣谢：本程序的日历使用库　https://pypi.org/project/sxtwl/。
