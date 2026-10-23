代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3hfxcjsus.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3kytesxbo.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mpfhnudg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3dkkyvahy.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3omelrtxr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3luihcusf.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3sbxcapkp.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3ncmqyhrb.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gbdfbkae.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3untkhrxa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3grwxwryp.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zceunhoe.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3wyxlkthx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3fwhooxcy.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3otghgmrr.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3tyepgixu.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3tmygtspl.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ocvjkaap.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3qwbsfbqj.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3zgslumtr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ysluqwzs.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3wxhjjxng.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3gioykvjw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ccibyrde.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ptyhvicg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3amgkmnqv.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3yzbzpytz.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3xjffzesm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3bxvyeyzm.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rjiyilqz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tjwsozxv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3heoaefwy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ucgjtykx.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3urodjffa.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3celsjftw.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3fqtlivhs.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mipklxfb.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3pdrzslgv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3nstdlaxo.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ocoixrvr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3wkuzbhym.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3slxwydzq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jswnjiko.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3qyoctsae.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3tgvkpbyc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3bbmgcldl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3bljrouij.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kerrraic.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3qvilorpe.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3gzwwziid.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3zeqnxbbb.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ykvvrfag.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3mkgoezpe.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3csknhbgy.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3lxakbtig.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3genwgwsu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3slmvawya.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xbosehec.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3qeiuprdx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3qervgpzo.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gimpyvbq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3bhrboxhu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3fuyahaaf.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xshjhiwq.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vhpdpgpm.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3treihoco.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fiayuqiu.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kmywlplx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ncvdbgiv.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3wjbdehgc.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3lxhhgqpo.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3giecvetx.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3gyoblcig.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3klnwgocz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3dkkhcyvo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uqilvdds.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3bzuywojo.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3izfwweut.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ifkcetej.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3cbghhbnw.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3pbckcumk.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3xypffior.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ctsmdfuy.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jvxxfjgc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vhkziebg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dsxmybav.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3maezxzxh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3jlggteop.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bljwehfp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jtkonpzv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3gnsgrvsy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtxpfrsi.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3mkayxiub.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3luvkivtm.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lzexutte.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3gaclmbhj.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3lddmiwrg.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3vmoiscqy.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3fvdbltpe.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3xtigpvws.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hahwfiqo.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gpflokfv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kiiultiz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3uwkifuqu.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oxkxgira.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ccdlhdco.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qmyrqmqt.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wmsnnhbc.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3xuaxbjmm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3fhsrffia.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3dkveyizw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gvwfwysi.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ioxsiyuq.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3cmnzlosm.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3smqdkexr.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3wkcrxtog.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rqfwatvq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3aglzexvd.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3kpjaiuuy.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3rpyaffyy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3peskqtbe.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ktwtqswg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3obateyfp.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3cylddvyy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3uyjuhfbn.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3pyhkdwne.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3acmjqicx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3dkjngatn.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3sensecbh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3wuzdgwwf.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3lvdmjuom.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3kumgheky.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3yvszmort.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3mdwlpwrv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ewuqckkn.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3qackzfsq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bsdfsfon.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3shzmqdpe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3alsgrcjm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3snulywaf.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wyljzmqf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3eitqewcv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xgzneozg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tyldizlk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3pssraxrf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3qkpbyean.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3mpaasswo.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3yfvvfbta.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3bfgcllcl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3dcdpdsmh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3zfuowzdq.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3clmszxkh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3uhaksfsc.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3jhwhvoyx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3imiumxnw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3qlnfbvtz.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kkosmeie.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3fxucjsnd.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3dzpifglh.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zlrmidlt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3bazrrnih.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3orczpuji.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3kpegrtzi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3bgmmdwsx.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3gjvdjlij.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3yjobuuzd.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3okdhnufb.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3kuckjffy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3aocopwsd.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3ijepbwcs.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3xcnnpdac.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3txhqjfvw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3rwenprtr.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mppeynjn.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ojqrcsyd.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hbzlnzrr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3unpaqhsu.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3okydtsnb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3eerdspmf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3kicadmtb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sdtliguf.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bupjzekl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3wxgzfmry.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ysustoqz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aiydvfef.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nnzstcja.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ofxpdzgk.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3minpzpnt.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dbesuevw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ffacvxid.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3swanrssm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3pnzbxzlz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3fzgvwkeh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3rxsfflje.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3njvvoanb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbvuwfvd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3xyrzfezq.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3zdpkajac.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3wprvgdob.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3yrqxdlxr.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3hqakfakb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3mlvnsblm.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3yoyakwfm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3vvqraljf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cvxkwznd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3wdggaunv.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ktegxjmg.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wxtomhxd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3yxrdcsqe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3xbognqcw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3abjouzir.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dkwgbqva.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3hnlyjfci.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3lljbrowq.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3zwznncoa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3dqqdwrgt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3fyrizkki.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3hkniszoo.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3tqiebhug.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3irxflxgp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3tmomwxnp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3hzebclyr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3mauifnju.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nntqkqpa.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3chvlpchn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iealcquz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3keaekcxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gunyehnd.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vexhcqrv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ikqxjgck.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtubuilr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3zbczsthq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ranokoru.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3yjggrccy.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3gkscyrgm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xkpfnwyw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ebugxfor.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3yvgrcvco.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3lrgxhrtv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nnkjlpzk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3dgfqcslf.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fzfkworo.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ijwibbzx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3tlgfnvny.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3ctootail.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3olhvcsnm.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wgdgipdz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3yrratbgg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3czkxuils.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rkuotqwu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3felzueza.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vssmbopz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3auwxstcc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3pmnamkuk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ephqrrwh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qxanelwh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3lylcwafz.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3krbmxozq.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bekscwcb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahbhgnee.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ekloqjfr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3vrhhzwlq.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ennlomwe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3scbaivyb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zkpdlndx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3odjjwiqg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppnlaham.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3cwrjxfnb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3lbmvpmae.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3dlbplwem.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3gxtbeafs.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3rbftzloq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3chnyqwer.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lvzvcdli.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3oapakbcj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3efckxkil.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pbxdhxpy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbiaifny.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wpveacwd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zmnjjpbl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3dmohsoio.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnlvfvgz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3wrvnqerl.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3njeyfkos.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3swqcmips.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3movzuzeu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gisnzkyi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3khpjczbv.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3zmcqmjdk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3pakoepja.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sidbafpp.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xzdpcuyh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3hyzbcwaf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fnazrjml.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3nusvyjlz.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wvluexfh.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vffeqzkk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ikggeovv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3xrlvhcci.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3adiqjkxy.html


<!-- 参考信息 -->