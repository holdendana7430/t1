代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://hz.xingfuxueyuan.xyz/gtyscfetll.html

[A07] 数字转字符串
来源：http://hz.yanxiufei.cn/gtwcvnrzyl.html

Py:   str(42)
来源：http://hz.316326.xyz/gtqvsztcrr.html

PHP:  (string) 42; strval(42)
来源：http://hz.sufxvd.cn/gtgoivwlqu.html

JS:   String(42); (42).toString()
来源：http://hz.wangdashe.top/gtbomksnpp.html

TS:   String(42)
来源：http://hz.andypj.xyz/gtsbkeakxf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://hz.jinqigufen.top/gtghzpyufs.html

Go:   strconv.Itoa(42)
来源：http://hz.yj202588.top/gtlsisvqbd.html

Ruby: 42.to_s
来源：http://hz.hnxiangtu.top/gtaygbrayx.html

C#:   42.ToString()
来源：http://hz.dianchejie.cn/gtdbonxztt.html

[A08] 取整与四舍五入
来源：http://hz.hysaishi.cn/gteyrdowwb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://hz.shanyushiyangkeji.top/gtgpwggkcg.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://hz.gotoacloud.top/gtverqyhkz.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://hz.ppjwa.cn/gtnfmhmijz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://hz.hongshengwenyu.top/gtvjwaekhr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://hz.nanxuanxn.top/gtgohrpzvv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://hz.yueranfly.top/gtekzpsvck.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://hz.yj202588.top/gtxggybisk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://hz.nanxinkj.top/gtuxznpdkj.html

[A09] 绝对值与最大最小值
来源：http://hz.jianghu66.top/gtemxtshvv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://hz.jyoumei.cn/gtrqghixst.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://hz.dianchejie.cn/gtdbqgahje.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://hz.jqgfzy.top/gtzzduspem.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://hz.hnqzz.top/gtazvenvvz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://hz.fzhhl.top/gtwxeqsuck.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://hz.ppjwa.cn/gtehjannol.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://hz.jinqigfzy.top/gtbkckpqpc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://hz.daria6918.cn/gtmpunxdul.html

[A10] 生成随机数
来源：http://hz.hnxiangtu.top/gtzqjryxhx.html

Py:   import random; random.randint(1, 100)
来源：http://hz.hysaishi.cn/gtxmdvvltt.html

PHP:  random_int(1, 100);
来源：http://hz.yueranfly.top/gtnecyuhkd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.hammf.cn/gtlwooknmb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://hz.zhiwuduotai.top/gtrmlhxrxm.html

Java: new Random().nextInt(100) + 1
来源：http://hz.zhoulong.xyz/gttmujudyp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://hz.nwbrower.top/gtyukkzxjo.html

Ruby: rand(1..100)
来源：http://hz.ybcxt.top/gtrpmszhek.html

C#:   new Random().Next(1, 101)
来源：http://hz.jiagoushi.top/gtawxnkpvg.html

[A11] 条件表达式（三元）
来源：http://hz.ywan-chungtsiang.top/gtcchbuoze.html

Py:   "yes" if x > 0 else "no"
来源：http://hz.cucudq.cn/gtfqlrzahz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://hz.sweek.top/gtjvcwyscg.html

JS:   x > 0 ? "yes" : "no"
来源：http://hz.shzxlz.cn/gtyenkmwor.html

TS:   x > 0 ? "yes" : "no"
来源：http://hz.fengsongda.top/gtqtuloyhl.html

Java: x > 0 ? "yes" : "no"
来源：http://hz.birdmap.top/gtkuokfsoq.html

Go:   // 无三元运算符，需用 if 语句
来源：http://hz.jiagoushi.top/gtfjslqizm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://hz.aibaodan.cn/gtfzqyikxs.html

C#:   x > 0 ? "yes" : "no"
来源：http://hz.bjfxy.top/gtgetcditr.html

[A12] 字符串插值 / 格式化
来源：http://hz.cucudq.cn/gtphbjujpc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://hz.gotoacloud.top/gttdqkqitl.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://hz.birdmap.top/gtuaccfdzn.html

JS:   `Hello, ${name}!`
来源：http://hz.chenlongwang.top/gteesflzwe.html

TS:   `Hello, ${name}!`
来源：http://hz.0kj1m.cn/gtfcrwwfdd.html

Java: "Hello, %s!".formatted(name)
来源：http://hz.ydzc1.top/gtawchztht.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://hz.feifeiyinyue.top/gtksplmwsj.html

Ruby: "Hello, #{name}!"
来源：http://hz.hnxiangtu.top/gtpivzpkph.html

C#:   $"Hello, {name}!"
来源：http://hz.zhoulong.xyz/gtqxidsuew.html

[A13] 多行字符串（练习 \n 转义）
来源：http://hz.kuanghao11.cn/gtskhtkcvo.html

Py:   "第一行\n第二行"
来源：http://hz.shuidangran.top/gtjlyyxcxk.html

PHP:  "第一行\n第二行"
来源：http://hz.yanxiufei.cn/gtekacrwwb.html

JS:   "第一行\n第二行"
来源：http://hz.dashuyun.cn/gtskhlguqr.html

TS:   "第一行\n第二行"
来源：http://hz.dianchejie.cn/gtrhejtsxc.html

Java: "第一行\n第二行"
来源：http://hz.gogol.net.cn/gtboahwozt.html

Go:   "第一行\n第二行"
来源：http://hz.0kj1m.cn/gtcndekhld.html

Ruby: "第一行\n第二行"
来源：http://hz.chenjidiqi.icu/gttkombogy.html

C#:   "第一行\n第二行"
来源：http://hz.jiagoushi.top/gtpkcvjwqj.html

[A14] 注释写法
来源：http://hz.chenzaomai.com/gtdycouqsz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://hz.wangdashe.top/gtiphetnma.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://hz.9152youxi.cn/gtkpketebl.html

JS:   // 单行；/* 多行 */
来源：http://hz.nanxuanxn.top/gtdtxfhapg.html

TS:   // 单行；/* 多行 */
来源：http://hz.xuanzx.com/gtfhgwwmyd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://hz.zhongyouzk.top/gtpqyvtxjr.html

Go:   // 单行；/* 多行 */
来源：http://hz.sxryk.cn/gtpivmagvu.html

Ruby: # 单行；=begin 多行 =end
来源：http://hz.hnqzz.top/gtukmdefsk.html

C#:   // 单行；/* 多行 */
来源：http://hz.shanyushiyangtech.top/gtrqfhzbfd.html

[A15] 空值判断与默认值
来源：http://hz.xylfe.cn/gtmgcvoswk.html

Py:   value = data or "默认值"
来源：http://hz.yuxming.cn/gtgqfnppya.html

PHP:  $value = $data ?? "默认值";
来源：http://hz.guannengcc.top/gtjbbwkaig.html

JS:   const value = data ?? "默认值";
来源：http://hz.ppjwa.cn/gticnbrgmh.html

TS:   const value = data ?? "默认值";
来源：http://hz.zhoulong.xyz/gtapnriorq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://hz.shzxlz.cn/gtwpsmagte.html

Go:   if data == "" { data = "默认值" }
来源：http://hz.hysaishi.cn/gtkuiilgfc.html

Ruby: value = data || "默认值"
来源：http://hz.shuidangran.top/gtpluydtut.html

C#:   var value = data ?? "默认值";
来源：http://hz.yongpay.top/gtcqskykul.html

[A16] 真假值判断规则
来源：http://hz.shzxlz.cn/gteeephntn.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://hz.xuetiantiany.cn/gtyfegqtfl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://hz.xylfe.cn/gtbcadqehk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://hz.tianlin.xyz/gteosfarfi.html

TS:   if (!x) {}
来源：http://hz.yueranfly.top/gtjjqtvcyt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://hz.wangshuangyany.cn/gtljtwltkr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://hz.jqgufenzy.top/gtepppofjs.html

Ruby: unless x            # nil 与 false 为假
来源：http://hz.cdnleiting.top/gtuwxxnxzm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://hz.dashuyun.cn/gtvccsxrod.html

[A17] 位运算
来源：http://hz.wangshuangyany.cn/gthbyypmjb.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.fzhhl.top/gtimlbimdz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://hz.guowangkeji.top/gtmpswopyr.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.xuetiantiany.cn/gtfkafnojp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://hz.shangyingyoupin.top/gtnewcpdkq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.hnqzz.top/gtpxrlbyam.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://hz.hfpthk.cn/gtkpnyoadj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.tanke756.top/gtleqffzxv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://hz.zhaomingkeji.xyz/gtpgnsxuhc.html

[A18] 字符与 ASCII 码互转
来源：http://hz.jlsjyb.cn/gtuioylywg.html

Py:   ord("A"); chr(65)
来源：http://hz.xuanzx.com/gtjveszczg.html

PHP:  ord("A"); chr(65)
来源：http://hz.hfpthk.cn/gtopfydaxm.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.0kj1m.cn/gtdqmauqkw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://hz.jinyuanbaomall.cn/gtdpmcxsxx.html

Java: (int) 'A'; (char) 65
来源：http://hz.316326.xyz/gtswzphcwj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://hz.iojbl.cn/gtutrbqbhc.html

Ruby: "A".ord; 65.chr
来源：http://hz.redwolf501.top/gtxyhdeigc.html

C#:   (int)'A'; (char)65
来源：http://hz.xylfe.cn/gtuledfbuj.html

[A19] 交换两个变量
来源：http://hz.shangyingyoupin.top/gtffwbducu.html

Py:   a, b = b, a
来源：http://hz.xingfuxueyuan.xyz/gtugtkxjzp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://hz.cqqwz.cn/gtrvdugeid.html

JS:   [a, b] = [b, a];
来源：http://hz.yj202588.top/gtriserujy.html

TS:   [a, b] = [b, a];
来源：http://hz.zhaomingkeji.xyz/gtkrdkitco.html

Java: int t = a; a = b; b = t;
来源：http://hz.ydjk.org.cn/gtkjbfjgyb.html

Go:   a, b = b, a
来源：http://hz.xuanzx.com/gtuzlpavit.html

Ruby: a, b = b, a
来源：http://hz.shuidangran.top/gtqthhubmc.html

C#:   (a, b) = (b, a);
来源：http://hz.fzhhl.top/gtjfnkoxoc.html

[A20] 读取标准输入
来源：http://hz.quarkkingdee.top/gtxvdbrvao.html

Py:   name = input("请输入：")
来源：http://hz.gaohongyu789.top/gtugyspyxs.html

PHP:  $name = trim(fgets(STDIN));
来源：http://hz.dashuyun.cn/gttzexiabh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://hz.cucudq.cn/gthipwnzgv.html

TS:   // Node.js：readline 模块
来源：http://hz.yj202588.top/gtashwrzwm.html

Java: new Scanner(System.in).nextLine()
来源：http://hz.hysaishi.cn/gtriipdobe.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://hz.jyoumei.cn/gtfkulscyf.html

Ruby: gets.chomp
来源：http://hz.zhixingplan.top/gtngckusuo.html

C#:   Console.ReadLine();
来源：http://hz.jiagoushi.top/gtljsizlce.html

[A21] 保留指定小数位输出
来源：http://hz.yonumen.top/gtrxcdjkgb.html

Py:   f"{3.14159:.2f}"
来源：http://hz.ydzc1.top/gtrzrypwjp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://hz.ydzc1.top/gtgdxpufbu.html

JS:   (3.14159).toFixed(2)
来源：http://hz.svipenyu.cn/gtpdiizupe.html

TS:   (3.14159).toFixed(2)
来源：http://hz.shanyushiyangkeji.top/gtnbfhmcbb.html

Java: String.format("%.2f", 3.14159)
来源：http://hz.tian-w.cn/gtchmrxgoh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://hz.daxiang520.top/gthywsixdl.html

Ruby: format("%.2f", 3.14159)
来源：http://hz.smart0.xyz/gtkcxepktk.html

C#:   3.14159.ToString("F2")
来源：http://hz.shzxlz.cn/gtlbxefzjx.html

[A22] 获取字符串长度
来源：http://hz.sweek.top/gtglsrmjke.html

Py:   len(s)
来源：http://hz.hnqzz.top/gtgdcegkbf.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://hz.gotoacloud.top/gtxkjynlcf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://hz.0kj1m.cn/gtisewrxqb.html

TS:   s.length
来源：http://hz.zdqjudy.top/gtptcdmxib.html

Java: s.length()
来源：http://hz.nwbrower.top/gtyitbcyxc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://hz.yj20258888.top/gtnkimjshc.html

Ruby: s.length
来源：http://hz.kuanghao11.cn/gtzqsnruvb.html

C#:   s.Length
来源：http://hz.nanxuanxn.top/gtfdglwclj.html

[A23] 大小写转换
来源：http://hz.hfpthk.cn/gtpbkxntca.html

Py:   s.upper(); s.lower(); s.title()
来源：http://hz.zdqjudy.top/gtdvckvtnm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://hz.feifeiyinyue.top/gtgqydrris.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.yvedp.cn/gtrgefjsme.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://hz.jyoumei.cn/gtvkxodyff.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://hz.zhongyouzk.top/gtnqidmdqj.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://hz.andypj.xyz/gtqxrsqtvz.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://hz.dianchejie.cn/gtmfsrcmbu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://hz.yj20258.top/gtvpaxxmvc.html

[A24] 去除首尾空白
来源：http://hz.9152youxi.cn/gtbpouvqcg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://hz.mhx1999.top/gtaezuwuqi.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://hz.zhiwuduotai.top/gtkbwxdizd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.zhijiandao.cn/gttbxopgrb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://hz.ybcxt.top/gtdhtfxdjm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://hz.sysykeji.top/gtisrqljqj.html

Go:   strings.TrimSpace(s)
来源：http://hz.feifeiyinyue.top/gtqwyisbsb.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://hz.yuanzhike.top/gtachzrdgm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://hz.smart0.xyz/gtyursxfzb.html

[A25] 字符串比较
来源：http://hz.ivvv.top/gtwiglqfsc.html

Py:   s1 == s2; s1 != s2
来源：http://hz.shuidangran.top/gtwufvryfp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://hz.wangdashe.top/gtapvjhnbm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.nwbrower.top/gtbqsftaui.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://hz.xinyue.icu/gtrmihqutx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://hz.ybcxt.top/gtcijvtnvi.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://hz.yongpay.top/gtxrlnwzyg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://hz.yangfankeji.com/gtppotpqfv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://hz.haohaochexian.top/gtnjgtbcyu.html

[A26] 类型转换总览
来源：http://hz.havefunace.top/gtnoytouoo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://hz.jiagoushi.top/gtzkulxjgn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://hz.gogol.net.cn/gtdswfgjyu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://hz.dianchejie.cn/gtbwbsgclz.html

TS:   Number() String() Boolean() x as number
来源：http://hz.sufxvd.cn/gtvddopxxx.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://hz.andypj.xyz/gtrirzevaq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://hz.yj20258888.top/gthiakgdid.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://hz.ivvv.top/gtjhtefdri.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://hz.sweek.top/gttnlafzgs.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtrozzstnq.html

B. 流程控制
来源：http://hz.sweek.top/gthxlkiptq.html

================================================================================
来源：http://hz.hywenlv.cn/gtqzemebdd.html

[B01] 条件判断 if / else
来源：http://hz.sweek.top/gtgzxfzmoi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://hz.yj20258888.top/gtiixmdqqa.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://hz.chenjidiqi.icu/gtrjrehmxk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.jlsjyb.cn/gtfvsmkynp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://hz.guowangkeji.top/gtgoqrorpp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://hz.pycfn.com/gtarmrphoa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://hz.gotoacloud.top/gtgdjjwety.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://hz.tianlin.xyz/gtmqoxcdkp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://hz.zhengqikj.top/gtcpudmavq.html

[B02] 多分支 else if / elif
来源：http://hz.cqqwz.cn/gtqsfuwcro.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://hz.fengsongda.top/gtfbgixgrt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://hz.redwolf501.top/gtijjwjhpz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258.top/gtokwtvgld.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.hysaishi.cn/gtlzdjshlr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.shangyingyoupin.top/gthmxwmjxr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://hz.yanxiufei.cn/gtjpvpghly.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://hz.ywan-chungtsiang.top/gtdvfwvgmh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://hz.yj20258888.top/gtctfdblqi.html

[B03] switch / match / case
来源：http://hz.9152youxi.cn/gtpulnhzvd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://hz.hongshengwenyu.top/gtelwpzvum.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://hz.fengsongda.top/gtuvwjmbah.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.jinqigufen.top/gtwdqktgyg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://hz.shuidangran.top/gttuwcabwo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://hz.hnxiangtu.top/gtfwwdevdj.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://hz.ppjwa.cn/gtdmjjalza.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://hz.guowangkeji.top/gtfvfusvvw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://hz.cqqwz.cn/gtjedjcoih.html

[B04] for 计数循环
来源：http://hz.jqgfzy.top/gtgposhnuq.html

Py:   for i in range(10): print(i)
来源：http://hz.zhoulong.xyz/gtzldapmpa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://hz.zdqjudy.top/gtlimhqwai.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.zycfv.cn/gtkondnxwl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://hz.snrcjt.cn/gtcvenukyx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://hz.tian-w.cn/gtvdnkctxh.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://hz.bjfxy.top/gtybeumsii.html

Ruby: 10.times { |i| puts i }
来源：http://hz.zhaomingkeji.xyz/gttrkbdjhv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://hz.wangdashe.top/gtikwmgywz.html

[B05] 遍历数组 / 列表
来源：http://hz.cdnleiting.top/gttcjkvpms.html

Py:   for item in arr: print(item)
来源：http://hz.xziqi.cn/gtijbjntan.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://hz.gotoacloud.top/gtmkoubmmf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://hz.9152youxi.cn/gtnauvyrxr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://hz.hysaishi.cn/gtibakxrjl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://hz.yvedp.cn/gtnrzzkklc.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://hz.cucudq.cn/gtgsiclgux.html

Ruby: arr.each { |item| puts item }
来源：http://hz.gogol.net.cn/gtspdwober.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://hz.nanxuanxn.top/gtkqcxokru.html

[B06] 遍历字典 / 对象
来源：http://hz.jinqigfzy.top/gturjxfhdz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://hz.mhx1999.top/gtoucggdjw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://hz.nanxinkj.top/gtmjcjuswt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.jyoumei.cn/gtovhoursf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://hz.hysaishi.cn/gthjdblwzx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://hz.cdnleiting.top/gtnhxcvzuf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://hz.shanyushiyangtech.top/gttcwqfdpw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://hz.vqdsnc.cn/gtkasuzirp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://hz.zdqjudy.top/gtyswqlizg.html

[B07] while 循环
来源：http://hz.yueranfly.top/gtmueestbk.html

Py:   while i < 10: i += 1
来源：http://hz.hammf.cn/gtjvclgfsz.html

PHP:  while ($i < 10) { $i++; }
来源：http://hz.aibaodan.cn/gtvrsuglaj.html

JS:   while (i < 10) { i++; }
来源：http://hz.fzhhl.top/gtqztmlqxj.html

TS:   while (i < 10) { i++; }
来源：http://hz.xingfuxueyuan.xyz/gttypdvduf.html

Java: while (i < 10) { i++; }
来源：http://hz.xinyue.icu/gtlacxfrvh.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://hz.jyoumei.cn/gtaimfccnb.html

Ruby: while i < 10; i += 1; end
来源：http://hz.ydjk.org.cn/gtprthhkkw.html

C#:   while (i < 10) { i++; }
来源：http://hz.ydzc1.top/gtimwimpag.html

[B08] do-while（至少执行一次）
来源：http://hz.jiagoushi.top/gtzbidyuoa.html

Py:   # 无 do-while：用 while True + break
来源：http://hz.yj20258.top/gtnsdypuoo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://hz.sweek.top/gtwdoyhyrv.html

JS:   do { i++; } while (i < 10);
来源：http://hz.guannengcc.top/gtndqevwxw.html

TS:   do { i++; } while (i < 10);
来源：http://hz.yj20258888.top/gtxzmmtuht.html

Java: do { i++; } while (i < 10);
来源：http://hz.hammf.cn/gtksijtzek.html

Go:   for { i++; if i >= 10 { break } }
来源：http://hz.wangdashe.top/gtwuxascwd.html

Ruby: begin; i += 1; end while i < 10
来源：http://hz.ehwqpu.com/gtbsholsgf.html

C#:   do { i++; } while (i < 10);
来源：http://hz.chenzaomai.com/gtorktkyuq.html

[B09] break 与 continue
来源：http://hz.sysykeji.top/gtpfgyilqg.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://hz.yueranfly.top/gtqlblkyni.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://hz.tianlin.xyz/gthfeitvno.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.birdmap.top/gtwqpxhrgk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.chenlongwang.top/gtqvhezcpv.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.jinghuilouyu.cn/gtjwiguwev.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://hz.c1oappe.top/gtabkwntcz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://hz.zhengqikj.top/gtpxxjlagp.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://hz.0kj1m.cn/gtwhpbzhfi.html

[B10] 遍历同时拿索引
来源：http://hz.ehwqpu.com/gtblbdvrke.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://hz.0kj1m.cn/gtytaiwepe.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://hz.fengsongda.top/gtbpcwqwlf.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://hz.zhongyouzk.top/gtixiuycly.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://hz.dashuyun.cn/gtlbaxxwhg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://hz.aizwys.cn/gtagaaaequ.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://hz.chenzaomai.com/gtfgglpiqs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://hz.shanyushiyangkeji.top/gtpwcbjsoi.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://hz.tianlin.xyz/gtyfofxcfx.html

[B11] 生成数字序列 / 区间
来源：http://hz.shuidangran.top/gtmjnkzczk.html

Py:   list(range(0, 10, 2))
来源：http://hz.fengsongda.top/gtjxxqmngd.html

PHP:  range(0, 10, 2);
来源：http://hz.zhixingplan.top/gtsyssbaed.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.xylfe.cn/gtjnesyvwn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://hz.yanxiufei.cn/gtpxneaufk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://hz.xziqi.cn/gtchmtvzzh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://hz.yueranfly.top/gtvguyniqj.html

Ruby: (0...10).step(2).to_a
来源：http://hz.bjfxy.top/gtbakfsmzm.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://hz.tianlin.xyz/gtqoxrstbg.html

[B12] 跳出多层循环
来源：http://hz.pengpengdd.cyou/gtiaqngfia.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://hz.jinghuilouyu.cn/gtedakqyfz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://hz.yonumen.top/gtfddjeacs.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.haohaochexian.top/gtnhvgobfb.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://hz.yj20258888.top/gtiduwjwtk.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://hz.vqdsnc.cn/gtkhsadokb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://hz.hammf.cn/gtzwzkcgai.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://hz.zycfv.cn/gtwgmkqrkv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://hz.zdqjudy.top/gtpotgjikd.html

[B13] 判断是否为数字
来源：http://hz.iojbl.cn/gtiroibkxp.html

Py:   isinstance(x, (int, float))
来源：http://hz.hnqzz.top/gtkuruaafl.html

PHP:  is_numeric($x)
来源：http://hz.jinyuanbaomall.cn/gttkfieubg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.zhixingplan.top/gtdcpnnhoy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://hz.chenlongwang.top/gtogjxtnaf.html

Java: x instanceof Number
来源：http://hz.hfpthk.cn/gtqhiyodjj.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://hz.wangdashe.top/gtsgnxicas.html

Ruby: x.is_a?(Numeric)
来源：http://hz.52xcode.cn/gtwiunmkmd.html


<!-- 参考信息 -->