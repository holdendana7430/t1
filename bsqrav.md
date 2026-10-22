代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wmgvwewd.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2jwkebwbj.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2bibnhoos.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rudbuilm.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dfheimgm.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dsjqjnei.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mdvdlohe.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2jqmuvlmd.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2clirsefw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qrnbvggq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2gbfusvfd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2qufqmplj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2assmqgow.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2oaqbnvll.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gnocpddz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2uraufofg.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2ugtulctm.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ruygzsyk.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2oadvjhso.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2smbpaerm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2drdjolhi.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ghneawgd.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ppdzaipa.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2yivtnmmh.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bfmibfvl.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vzutdtkq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zemkavrk.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2kbvrgaoz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ozgbwjqf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2twqujirb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2vrjlycmo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2iqwcnrex.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2bpcqwtdn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jrzqyoas.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2hgbyrjxa.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2fjwcfpnf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jtjqhxem.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2agcqpzwl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hgmixigs.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2lrpvfulp.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wkivzdce.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ltwapptq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2sxvbakxk.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2icgremba.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2qyycloiz.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2fyhhsvwt.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2hzpdyags.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ybjzzmbn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2amhgjvcl.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qjtxhdsk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ifkupapj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xquuzutg.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xypzlhgf.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2hufytose.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yewycbhx.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rpmhojfk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xmnlmdze.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lohslrvp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ztflsbhx.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pbojptmg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2dyxyzkiz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2svamuvfr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2zhkptbev.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpylwsov.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2tkohknxt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2dwtizjet.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2koqmylad.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qkhiezgc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2aduxkurk.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2khrgfrsv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2rxyysfsa.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2bbktnzds.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qpyquszi.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2ljdoyugl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ooekiovr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zcsuyxlu.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fctvvjxp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2glbgkkaw.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wruesmvf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ttbpstyy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oznejkhy.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gwvzndzs.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zexjfzvx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2rcsdnevw.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2tjguayaz.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2nspzczde.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qycmwglf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2gdpzsygz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eytiaxiz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2weogxfne.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2toxvmyvu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ygrnzrtu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hjtesabe.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iigwiuua.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ncbbtlbv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ksfgnqlt.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rugyzyjw.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rbfjvhmt.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mruvayar.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dlzcaqbf.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2imzmrrbj.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2taxnovvd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yvdbyzhr.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fbutdcie.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sdafxcqm.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2dvqknjdn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nsnlejeq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2ncdsocwn.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jionudyp.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ntxsextk.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2pgkcrfou.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zucycqer.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2kntkytoj.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qjpuwcen.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2wthhfenw.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2htanvdzo.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2uehialzp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2xrctunpc.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2rsqmxkmm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2mnwedtld.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2qmlsnooy.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2zrmlljco.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqfeapps.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofafbbzl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2gbonceha.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jtcdlhdc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qxfxzjwm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2olafaadm.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qryedpgz.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2schnninl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ervcwvnw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bvinouss.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2egxvppmf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ojzttvdd.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xijhnqkd.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2hfrxxajr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2pwkafdtd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2aaqeixof.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2pnozppav.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mwlxenrg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2idzzomgx.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2pzpvckme.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2yserpiih.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2hocjbixg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2ftxsgvko.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2bovcjypk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2recyamst.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2xljkmqij.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mfwlzuza.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2akqvmtdo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2hvaowzvs.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bnirntap.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uvftkwjx.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2cdantxqb.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2kubdscez.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2tsmiaqtn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2doizrokx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ophlosli.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2etxdsjcl.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2hwecgech.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2dopmtswd.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2defpnmas.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2gbohtxhl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2peuxshzl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2svbkhwxi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2txvotpjl.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2lbnqmqmo.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2isoxvlva.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2szneeiww.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dgcvrzql.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yktbdzet.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2jglgqqpq.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nikperrs.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2swebajvm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2baxxorby.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2jyiuykrr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tgeeudmz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2fkjborgz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2cvvzzqqa.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zggaqdgt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tttwsefw.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nnsyyyuf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2axoaukir.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2tiflhnhd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ssnezkix.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2bkzmnbkd.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2ahqbhned.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2unfrkalm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qyunuvby.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2gvijvuhd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2bogbbpdn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ismpmdzu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nfnqmkzt.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yidpkxto.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yehycfbt.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ljwaktgy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2iuubcrhq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ogngbaai.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2dvexrizg.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ahgwxmfo.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2nbwycueu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2fdvbassu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tefrnyin.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zwevxmrp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2yzepytea.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2umncsslw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2tzhlidet.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2weynbnfe.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2gwanfmzr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2xtqnvfqj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2avsorjam.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2bghpyzrd.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2jwvogizr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2qnhronyy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2scuyviyh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2oxxunjxb.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2lhcptsyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ctekxbzv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2pgqfnoyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ukdkopwb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2norsycku.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2dtbfbuyy.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjdjwbdn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2tjsfrppg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jafvzuru.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zozhbnoq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ziirpchz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nvvqckgz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rdtptucq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2uymgeqda.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2uarlrsbe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2xemzbuti.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eoyfqybf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gtkfhnmo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2arkrsuhy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ludsquyt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2waxuticn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2byigdgnp.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2iqzwublq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xbyaevjj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2khupricb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rigajkwm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rsosjmow.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zieovhgf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2hiooclou.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2rcnzypkg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2kxtzvsti.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jlcogbrj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2amdxhjxb.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ygwgybpg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cdgcyvzy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zayrfepx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2yqnwijkm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2scyxpudq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2zoqgwubj.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2pvpyebwq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ughayoia.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2knytyxqa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2batvqnvm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hhzrngfy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ycdygfcn.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2flrvhkck.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2okpglnql.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2nkknufyt.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvsebiww.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2xdxlcked.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dkyennir.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpgqsyme.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuwjfpvy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrrxyblm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2epjxswwf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2qpsvjqsq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2wejargof.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2itjughxl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2vkcorlce.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2tsqenoqx.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2dtohciyb.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hhgezhzv.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2inwwjmrv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gdgmarsq.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vkhqlbve.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2qejgpqzz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqalkver.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2hhivkfha.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2uyroryhf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2boyxpzrr.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qfrlgdjk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vewgdkbz.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vnunqhnm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2oxmrxuiy.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2mhetybnh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nsbypnuj.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2quppgopz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2pccuduxk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxwlzdtt.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2grmxmwvy.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pslqpatf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ufxaivcw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fgdanhkd.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2imfdpjub.html


<!-- 参考信息 -->