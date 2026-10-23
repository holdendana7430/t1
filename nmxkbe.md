代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3tzfbcegt.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3mpkpsjiu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3aztzzaqr.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3uplsvlsw.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hdcrvekp.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zuygeqlo.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hzbtwnvg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3haiyiciw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3mwbfqmvt.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3avbiunao.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3fczuoklm.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3adtgyjcx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3nsahkjtu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3lntbmprc.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3cmxwzevy.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3jnosivxi.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3uhlkvcpt.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3uiutehhl.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3ptodpeqf.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3vquploxu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3elirtfak.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ulqgbfgu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pndcyaxe.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xddcimcw.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rtbzoigi.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vojxfvmb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vbdpvmcv.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ftuvlber.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3suldqrrr.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qrqmhlhn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3myrvnxmw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rgabmnmo.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ucwegbxo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hbsexcbv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3dtdvtkvz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3lbwvkthr.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3uemzeomj.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hhpdgipx.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3adirhgrm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3guxsqpis.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3qtsufdhx.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3hbahecbd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3yceoolsc.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3virsnofi.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3dmcoudvm.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3dkwwiqdn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3zywmcpqv.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ujfuveqk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3krjlvusu.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sftlsaus.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3mdeybxjd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ailymdsb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qftgvmfw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vrbufikp.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wzxjvfly.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3brycmlxl.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cwbiastn.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bonnkgyt.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3bhddxuli.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hxyllxyo.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ytqixajd.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3nxoaftdc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3zyrplurd.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gldbbsqk.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3jlgewwbs.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3ntqdcemn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3qdkzwukl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vtdktanu.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3ulwufyrk.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vnrugmzt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3eurbnuik.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3qeeewzog.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3wufgblgg.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3uihctqhx.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3jgamuvbo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aqnycsom.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mngzlkdm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gihtftbi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qamhbmmb.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3fbmulybo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3eqvuzwxl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3sicrjvtq.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zdnnzwqp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3iwoplapn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3wjwcrzir.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3jggepeph.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3iwdwobgn.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3nnwkbhhm.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hruuglta.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3dbhleazc.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3jyslnakc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3zfnvlmxe.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rpjpodlf.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ixgwyznd.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3umxkoawf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mhsxhcye.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hiqvcqpd.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qyygqtwx.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hhdkhmyd.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nycbmvqq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3hfymewqp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3qcghmvpi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3iznprtvf.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nxuwyail.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ngakoctv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3rnlygnhq.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3fjwmplhw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3xgeeilzc.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hucxbmrv.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3zbplyhnm.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3mapiqcva.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cwxkkbhe.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3vdwctgjn.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3igfuvpbg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3txsirmbf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3hajdfmyi.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3gsalqujs.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3giuqfipg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3frkofzis.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3vlwodehq.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3eqqqpapa.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3otwxhofg.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3eitumdnn.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxhgnupm.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3boqjaumi.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3hasjkvbm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptojlurx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3fhurxrdj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bdsigvzj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ttgqfomj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bcouysnv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xorypzxf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3oxofrmdq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3spekxicm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zadmffdc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rjwtfxri.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3kqayfnpl.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vdtoxprv.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3dcqilljt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gevutkly.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hvpxsxjv.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ufyaqfqm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3rccohxkj.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3zhgeljfq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3giovtlnj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3qghszkby.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3jrinefwq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3ojhglcht.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pvqxeknf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3sepynghf.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3kwjbqwhv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3lacpapjo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3qmwchxgf.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ndogqlrh.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3pwalpfjy.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3tivrdttr.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3nkxpsjzk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3jmewqycu.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3aarjzgdy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3mvpicfci.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3jnxjalkv.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3gblbpakg.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3tzfxosow.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3srolgmal.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3depgesmu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mqxdjlbo.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3nbngvryz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zsmtwevr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3xefbfupz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3jclkomfm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lesrllxf.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3xnzafppb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hrnukern.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ztdflseu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3svwuchcj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3obxhotoo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3areughht.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rtxxgbxj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzjbdvbr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aahsancy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3bmjrgapm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uartbqem.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hyegowck.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vaxwrnhu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3baunllaa.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ccpvklgg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rwlmqhak.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3trcmckvm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3aylznkab.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ytfjhtxk.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ahhkxqjx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3kcwelich.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3jemywpsf.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wtwxzdwb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hkdpncyw.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3bcqineoo.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3zbxxejqz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3vokctapl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fxaicewl.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rdgvvvbn.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3jikcyrgt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pogtlpuq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lpgifbbm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cueekcsa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3itykenlp.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cyxjowvz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3hulmlmsw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3getlqcdd.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3ocpxursu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3qtiwkxou.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lkqijhbj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3snnqjqtd.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3tzplplgw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lkvvmiur.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ekbtpubv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qzvuztir.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dyrgxbcy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xmdgicxg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3zdzoonyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdhfrcqi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gypnwtlq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3rcnpedgx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaydtivd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3xsxdcffg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3abmselot.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3xzddgepa.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ygepaiwj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3hsccpmlj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mmgeftdf.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3miakadab.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3nksmsdoo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3lpfdlfkf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3zteelmyw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ejniiibr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3negwqlym.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3tcrtlign.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zfkkvbqu.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ymjuwdvq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ahgjqqpt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3kjeiacrk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjmhdelc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kagstdxa.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rerkwhuy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlqgeqph.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ohmgonyy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3mubjjzal.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3jfvngync.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xjtnatza.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fpwonzps.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3eazzgfub.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3saaxpfto.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3krlqqpin.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hixolotz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3izqlpbld.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3mgqoanai.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3rpikdkks.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fatcpwmp.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3nuvpbvhn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozxenyow.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvpurahc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lqjyvalh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3azoclapz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lhznminn.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3kvikgvar.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3fccfoedy.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3iolzhafr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3nuazqyca.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3haukokgv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jcneryid.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3oyaggqjk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3bsungerh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3lbszmupv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3inbibevd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rnevzbql.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ziafunje.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3qczfptge.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnnizbxc.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpeveewy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xkwnkhca.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wjdfwpso.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ljocctow.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xoqbyglh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkapbfry.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gyqohxtx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kqfajldh.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bcwntjix.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3otodtplf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3bptzdqte.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rwpmyidj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3srsbkybt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3phmtkjdx.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3rokkmjpl.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ybvnmuhe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3kyqgkcfh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3judicoyo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsgdvpfv.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mfurybdm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tamisxpw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tusmzcwo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3hyrlenom.html


<!-- 参考信息 -->