代发 wailian999

Ruby: PI = 3.14159
来源：http://www.m.share.zdbjq.cn/Article/details/gcobfyjcv.sHtML

C#:   const double PI = 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gucsvjerc.sHtML

[A04] 判断变量类型
来源：http://read.share.hesvh.cn/Article/details/gbyvhyofo.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://read.share.fehbvm.com/Article/details/giaisrjeq.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://3g.hesvh.cn/Article/details/gcmkvmbtg.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://baike.fehbvm.com/Article/details/gqextnirq.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/ggrzfxplv.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://baike.zdbjq.cn/Article/details/gbobalynu.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://mobile.fehbvm.com/Article/details/gelramohe.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://www.share.hesvh.cn/Article/details/grpcisrvn.sHtML

C#:   x.GetType().Name; x is int
来源：http://mobile.hesvh.cn/Article/details/grinbmlnz.sHtML

[A05] 整数除法与取模
来源：http://read.share.zdbjq.cn/Article/details/gqxjzirha.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.share.fehbvm.com/Article/details/gpkmlgymq.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://3g.hesvh.cn/Article/details/gyehkzcwx.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.fehbvm.com/Article/details/ghtbsxlcw.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://m.share.fehbvm.com/Article/details/gaejnjgnv.sHtML

Java: 7 / 2; 7 % 2
来源：http://wap.hesvh.cn/Article/details/ghogxzouy.sHtML

Go:   7 / 2; 7 % 2
来源：http://read.share.zdbjq.cn/Article/details/gnczlkune.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gxqszsyit.sHtML

C#:   7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/ggmcgrynm.sHtML

[A06] 字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gzvoynbvm.sHtML

Py:   int("42"); float("3.14")
来源：http://baike.fehbvm.com/Article/details/ggecvoswm.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.blog.fehbvm.com/Article/details/ghjqownxf.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gieqwclio.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://www.blog.hesvh.cn/Article/details/gkocqhjwa.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://baike.hesvh.cn/Article/details/gztirvowv.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://wap.fehbvm.com/Article/details/gvdugzhya.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://www.blog.fehbvm.com/Article/details/gfvdkfzmx.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://m.share.fehbvm.com/Article/details/gnkmykohv.sHtML

[A07] 数字转字符串
来源：http://m.share.hesvh.cn/Article/details/gaoyzzwzy.sHtML

Py:   str(42)
来源：http://3g.fehbvm.com/Article/details/gzpsybnqd.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/ggwrqobcq.sHtML

JS:   String(42); (42).toString()
来源：http://mobile.fehbvm.com/Article/details/grgfyjdka.sHtML

TS:   String(42)
来源：http://www.m.share.hesvh.cn/Article/details/guycowigr.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://3g.fehbvm.com/Article/details/gbxqxydlg.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.fehbvm.com/Article/details/gmkxqwfxl.sHtML

Ruby: 42.to_s
来源：http://m.share.hesvh.cn/Article/details/gmxzsgtjo.sHtML

C#:   42.ToString()
来源：http://blog.fehbvm.com/Article/details/glkrvvymu.sHtML

[A08] 取整与四舍五入
来源：http://3g.fehbvm.com/Article/details/gqazggsmv.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gutqhngvr.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.hesvh.cn/Article/details/gkmoadkhw.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://wap.hesvh.cn/Article/details/giosawstq.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.hesvh.cn/Article/details/guvgzvwon.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.fehbvm.com/Article/details/gzuwkzqbd.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://read.share.fehbvm.com/Article/details/glhacislo.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://3g.hesvh.cn/Article/details/gvozccxfh.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://wap.zdbjq.cn/Article/details/gkxsakfoz.sHtML

[A09] 绝对值与最大最小值
来源：http://baike.fehbvm.com/Article/details/gaqmmfyom.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://baike.fehbvm.com/Article/details/gnxsukbhm.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/grmrpdupu.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.zdbjq.cn/Article/details/gmjbarhsz.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gnkypzhkb.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/grhpiwspi.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://3g.fehbvm.com/Article/details/gcycwhurg.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.hesvh.cn/Article/details/gljnbwjkn.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.blog.fehbvm.com/Article/details/gofrqboyy.sHtML

[A10] 生成随机数
来源：http://3g.zdbjq.cn/Article/details/gzshhujim.sHtML

Py:   import random; random.randint(1, 100)
来源：http://www.share.zdbjq.cn/Article/details/gyeyoiewa.sHtML

PHP:  random_int(1, 100);
来源：http://wap.zdbjq.cn/Article/details/gaxkkfssm.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://3g.zdbjq.cn/Article/details/gooavocpd.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.m.share.zdbjq.cn/Article/details/gmnxqzslo.sHtML

Java: new Random().nextInt(100) + 1
来源：http://wap.fehbvm.com/Article/details/gcezvprby.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://blog.zdbjq.cn/Article/details/gwhvkedek.sHtML

Ruby: rand(1..100)
来源：http://baike.hesvh.cn/Article/details/gdjlgxbca.sHtML

C#:   new Random().Next(1, 101)
来源：http://read.share.zdbjq.cn/Article/details/gekfrnifv.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gmrohshji.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://mobile.fehbvm.com/Article/details/gxnldyqlv.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/gazsbbmtb.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://blog.zdbjq.cn/Article/details/gfkdaaaym.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.hesvh.cn/Article/details/goiarxvsc.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://wap.fehbvm.com/Article/details/gmaqtdxyg.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://m.share.fehbvm.com/Article/details/gwbwyadbr.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gzosxxsxq.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.fehbvm.com/Article/details/gmbgpcjdu.sHtML

[A12] 字符串插值 / 格式化
来源：http://blog.zdbjq.cn/Article/details/gmpnojwtb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.m.share.fehbvm.com/Article/details/gjpmcvmyx.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://3g.fehbvm.com/Article/details/gpldpxgaj.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.zdbjq.cn/Article/details/gbqyotlwt.sHtML

TS:   `Hello, ${name}!`
来源：http://www.share.zdbjq.cn/Article/details/gcenodhka.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://3g.zdbjq.cn/Article/details/gaiznoruw.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://3g.hesvh.cn/Article/details/guudypcwv.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.hesvh.cn/Article/details/gvimajnti.sHtML

C#:   $"Hello, {name}!"
来源：http://www.blog.zdbjq.cn/Article/details/gjahujphy.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.zdbjq.cn/Article/details/gvweelugj.sHtML

Py:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gpybmivyl.sHtML

PHP:  "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gdjftnvxa.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/gbkjmcufr.sHtML

TS:   "第一行\n第二行"
来源：http://3g.fehbvm.com/Article/details/glgizknnd.sHtML

Java: "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gaewlleol.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.fehbvm.com/Article/details/grcrhfjzz.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gyarjcbqb.sHtML

C#:   "第一行\n第二行"
来源：http://baike.zdbjq.cn/Article/details/gitbparqs.sHtML

[A14] 注释写法
来源：http://blog.fehbvm.com/Article/details/gakctdsmr.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://baike.zdbjq.cn/Article/details/gqbpxzykz.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gsnfsdews.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gyipujgwc.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/goqfhmwkv.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://baike.zdbjq.cn/Article/details/gibzdexhr.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/ggosindcx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://blog.fehbvm.com/Article/details/gibayhqun.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gylqongyi.sHtML

[A15] 空值判断与默认值
来源：http://wap.hesvh.cn/Article/details/gqrnadwyi.sHtML

Py:   value = data or "默认值"
来源：http://read.share.hesvh.cn/Article/details/guohfjeaz.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gyajqlmrk.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gckxsqaab.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/gbplsgiii.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.blog.fehbvm.com/Article/details/gpofetyoi.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://blog.fehbvm.com/Article/details/gnmazwoev.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gzvmnlopj.sHtML

C#:   var value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gyxesphhg.sHtML

[A16] 真假值判断规则
来源：http://blog.zdbjq.cn/Article/details/ggtoungya.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://mobile.zdbjq.cn/Article/details/gdkobtrsg.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.m.share.zdbjq.cn/Article/details/ghsmlhvhs.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gvbqctwjd.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/gpgyswnqs.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.share.fehbvm.com/Article/details/grwepwair.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.zdbjq.cn/Article/details/gepqhaaic.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.hesvh.cn/Article/details/ghedlzzck.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.fehbvm.com/Article/details/gviixdxhy.sHtML

[A17] 位运算
来源：http://www.m.share.zdbjq.cn/Article/details/ginfcrewk.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gdxghnhoy.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.hesvh.cn/Article/details/gcsounhyd.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gjeydcyoc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gjsoyiauc.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gbarldtvz.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gsiocdjui.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gxplxgazl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gscsdyzsc.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.fehbvm.com/Article/details/grypehxqb.sHtML

Py:   ord("A"); chr(65)
来源：http://wap.zdbjq.cn/Article/details/gqifzzxlk.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/gmipfqzun.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gxgirqfpg.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/gxtmyfmug.sHtML

Java: (int) 'A'; (char) 65
来源：http://wap.zdbjq.cn/Article/details/ghozfucbs.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://baike.zdbjq.cn/Article/details/greoogxgn.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.zdbjq.cn/Article/details/gtmifmism.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.zdbjq.cn/Article/details/gcxyruoav.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/gohkhqxmc.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/ghwxizzfq.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.zdbjq.cn/Article/details/gnqjnavkm.sHtML

JS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/guprzvsjm.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/geuhsbfmz.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.zdbjq.cn/Article/details/gvqhdqjfb.sHtML

Go:   a, b = b, a
来源：http://3g.zdbjq.cn/Article/details/gmfsqttex.sHtML

Ruby: a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gblpxknfc.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.zdbjq.cn/Article/details/gojbjfomf.sHtML

[A20] 读取标准输入
来源：http://mobile.zdbjq.cn/Article/details/gynikndep.sHtML

Py:   name = input("请输入：")
来源：http://m.share.fehbvm.com/Article/details/gyexctujg.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.fehbvm.com/Article/details/grfraanpo.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://baike.hesvh.cn/Article/details/gvarljsrc.sHtML

TS:   // Node.js：readline 模块
来源：http://wap.hesvh.cn/Article/details/gtkwewtre.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://blog.hesvh.cn/Article/details/gadrpnnvk.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://3g.zdbjq.cn/Article/details/gaptijxrv.sHtML

Ruby: gets.chomp
来源：http://wap.fehbvm.com/Article/details/gfxgzsobc.sHtML

C#:   Console.ReadLine();
来源：http://blog.fehbvm.com/Article/details/gmskcygev.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.hesvh.cn/Article/details/gdnctouna.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fehbvm.com/Article/details/gpvlnhdca.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/gotjxnjws.sHtML

JS:   (3.14159).toFixed(2)
来源：http://m.share.zdbjq.cn/Article/details/giuzgvifg.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gdgvblwpz.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gpochyujv.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gpdgycire.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gpleevakx.sHtML

C#:   3.14159.ToString("F2")
来源：http://wap.zdbjq.cn/Article/details/gplhbvktr.sHtML

[A22] 获取字符串长度
来源：http://baike.zdbjq.cn/Article/details/ghfxanley.sHtML

Py:   len(s)
来源：http://mobile.fehbvm.com/Article/details/gcwweasnm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gyzpcsqiy.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://baike.fehbvm.com/Article/details/gwvtxmunc.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gwwxivujm.sHtML

Java: s.length()
来源：http://3g.fehbvm.com/Article/details/gpfhggwbm.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://mobile.hesvh.cn/Article/details/gckhgtffd.sHtML

Ruby: s.length
来源：http://www.share.fehbvm.com/Article/details/gcfejsbbp.sHtML

C#:   s.Length
来源：http://blog.zdbjq.cn/Article/details/gofjxfsml.sHtML

[A23] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/glvgpgvrz.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.zdbjq.cn/Article/details/gemuhscck.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.fehbvm.com/Article/details/glxjsjkfo.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gmpiaovnx.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/grmopccta.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/guhqnbrhl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.zdbjq.cn/Article/details/gbhbfrksr.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gsrjnjpvu.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://blog.hesvh.cn/Article/details/gfeivjwid.sHtML

[A24] 去除首尾空白
来源：http://www.share.fehbvm.com/Article/details/gyyeabpix.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.hesvh.cn/Article/details/gwzehwwbe.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://mobile.hesvh.cn/Article/details/gwujonebn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gbohafahv.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.fehbvm.com/Article/details/gtfrcoxnx.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.fehbvm.com/Article/details/gmmkucziq.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.zdbjq.cn/Article/details/gvzffncrp.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.hesvh.cn/Article/details/glsgwgcdg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.zdbjq.cn/Article/details/gpzdnlpvo.sHtML

[A25] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gseftsqcc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.fehbvm.com/Article/details/geeidzyuq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.zdbjq.cn/Article/details/gepbknqzu.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/grmxdkwgu.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.zdbjq.cn/Article/details/glmrwsxuo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.hesvh.cn/Article/details/ggrmsuenf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/giflyuind.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.hesvh.cn/Article/details/gjfqswpdp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.hesvh.cn/Article/details/gcqtpfrvx.sHtML

[A26] 类型转换总览
来源：http://m.share.fehbvm.com/Article/details/ghzmwbcwz.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.fehbvm.com/Article/details/gadgcvrit.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.fehbvm.com/Article/details/ghatsflcp.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.share.zdbjq.cn/Article/details/gvxtlasjk.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.fehbvm.com/Article/details/gqwxxbkuz.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://read.share.fehbvm.com/Article/details/gvcrlhkqc.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.hesvh.cn/Article/details/gnnvchfmv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/gmecmbybr.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/gualxbndx.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcvxulzua.sHtML

B. 流程控制
来源：http://www.m.share.fehbvm.com/Article/details/gtaoagedg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvcpvllog.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/gyxqbglmo.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.zdbjq.cn/Article/details/gatgzovcr.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gsscxcfcx.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gdwhrxbsc.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.hesvh.cn/Article/details/gzpxqtmug.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/gadhdtcqo.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://3g.zdbjq.cn/Article/details/gociyogoq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.fehbvm.com/Article/details/gulcksqyx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gpdnagylc.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.fehbvm.com/Article/details/gtaiegqtq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fehbvm.com/Article/details/gnqkndqgm.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.zdbjq.cn/Article/details/gxqeanuvn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.hesvh.cn/Article/details/gcrsbjirp.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gptrttgpy.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gzkhppuji.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.hesvh.cn/Article/details/guphhnnxo.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/gayfzpqwz.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gwacnarnd.sHtML

[B03] switch / match / case
来源：http://mobile.hesvh.cn/Article/details/gccqcfcag.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://m.share.fehbvm.com/Article/details/gzqbothqq.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gejyosjce.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/goefdtyil.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.zdbjq.cn/Article/details/gjddfwiwv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/gbhpvwzbu.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/grthtjeic.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.zdbjq.cn/Article/details/gtdpkzfff.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://mobile.zdbjq.cn/Article/details/gaftpgeia.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gicsggfeb.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gjskgfkfc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.zdbjq.cn/Article/details/gstjgbjmf.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gvxomyyxd.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.hesvh.cn/Article/details/gyqvsquch.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gyocfwoft.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gjxpwrrcu.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/gzhcgedqk.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gkutiozmo.sHtML

[B05] 遍历数组 / 列表
来源：http://wap.zdbjq.cn/Article/details/gokosqyjk.sHtML

Py:   for item in arr: print(item)
来源：http://3g.zdbjq.cn/Article/details/gglrzdddk.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://mobile.hesvh.cn/Article/details/gybdehknx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/gxwyeeouf.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://3g.zdbjq.cn/Article/details/gmvxgowkj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://wap.zdbjq.cn/Article/details/gwkybbnlv.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://wap.hesvh.cn/Article/details/gafvlonye.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.zdbjq.cn/Article/details/gqiopwqtr.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.hesvh.cn/Article/details/gnpcafbhc.sHtML

[B06] 遍历字典 / 对象
来源：http://3g.hesvh.cn/Article/details/gbcmpjqak.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.zdbjq.cn/Article/details/glsnsirna.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.hesvh.cn/Article/details/gowhqlxdr.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://mobile.fehbvm.com/Article/details/gsnzylxnb.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fehbvm.com/Article/details/gxwvfqaoa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/gkcrfrixe.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.blog.zdbjq.cn/Article/details/gzjxsrevf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://3g.zdbjq.cn/Article/details/gagjfdutc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gchkpjdoe.sHtML

[B07] while 循环
来源：http://3g.hesvh.cn/Article/details/gcczlydmn.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.hesvh.cn/Article/details/gzxbcseff.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/glzfanwwb.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.zdbjq.cn/Article/details/gajsgunpe.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gbkdkcvwg.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gcrmrrhtz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.blog.fehbvm.com/Article/details/grubgjngp.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.fehbvm.com/Article/details/gjnsywejd.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gizlitllr.sHtML

[B08] do-while（至少执行一次）
来源：http://www.blog.zdbjq.cn/Article/details/gfcstaohx.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/ggoaolppn.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.hesvh.cn/Article/details/gbhifefbb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gebvqajep.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gnczpibgj.sHtML

Java: do { i++; } while (i < 10);
来源：http://wap.zdbjq.cn/Article/details/gkzdbrzlm.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gjdhytjgu.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gtowjpaii.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/goioooqma.sHtML

[B09] break 与 continue
来源：http://www.share.zdbjq.cn/Article/details/ghqpjlzjm.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.fehbvm.com/Article/details/gkwcgssvk.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gxuqyvdaa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fehbvm.com/Article/details/gawwrcrjz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/gguslwmds.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.zdbjq.cn/Article/details/gmweqptzk.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.hesvh.cn/Article/details/gczpvwccv.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.zdbjq.cn/Article/details/ggjbxxkrh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gpxaplqgq.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.zdbjq.cn/Article/details/gybliuyuy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.fehbvm.com/Article/details/ghhcbabfp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.hesvh.cn/Article/details/gfjdutipu.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gndtclxfz.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/glltbvpwt.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.zdbjq.cn/Article/details/gfkcygmmh.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.zdbjq.cn/Article/details/gqaceaxfs.sHtML


<!-- 参考信息 -->