代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3jgjvmlrw.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zsicnwxx.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3flffchhi.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3nwuzobur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iymxqycz.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3tdiyennt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tnvvethk.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3jgxuxrqw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3tlaasqbl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3dutnvytn.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3kvxzsprf.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3ifdalywm.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3iafqgwvm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3tchloppw.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3mvamgyfd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3udrqjudd.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3bzyqipel.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3mkzhyesy.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nxwjxiez.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zevomnua.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3zbjcaehf.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lfjrpffo.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3ezykguje.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3dhkdejbx.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lbmagnmo.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vbtdlwwt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3scglcrdo.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qaticpbd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3isikufen.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nfjuethp.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3vwpfqjdt.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3skjgnrvb.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3erdrunjc.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dqjsfoyn.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3jmgwgwtt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ztgmgmvr.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3pbriffwa.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vrdefkmu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3idtyvfnf.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3qhcjgnkl.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3fxedwhki.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3ypbuubvm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3lgvqsxpo.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3llvuwmct.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3fbqffslx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3bicosufo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3sflsxyhs.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3vruddzio.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dvsozzaw.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3wbsodnoi.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3obyuocru.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3kyymjbya.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3skfysavr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3dhtkgerv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3xuulbsag.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zogfycna.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qxgcndkn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3grszmieb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3srvomilt.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3ymnmuoph.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3srsatxwg.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3gjdmjszl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cpspkmyv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3yeiiaspp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3luqkxwki.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hyhlnlqz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3kcuezkbn.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3isviliyk.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3enjnbrwk.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3pfmaphns.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3hlceyvxk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pdqatjia.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3tihfsyhh.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rcyzvvlm.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3lnxpxtlr.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3sjhmqssj.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hlbslkje.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3exsqyckv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ggzgcvck.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xljoluee.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3rmujsvfs.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ulqrhzlb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gzjjjzly.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zcvjnlsp.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rzjkmszq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3znfyatnw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3sqmfzcsl.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3muswxuxq.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ilikekox.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3qhlnivah.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3ffofabri.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3juxxyozv.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3esodxuqd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ofxywqkw.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3rdrtcgwo.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3huyknzje.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3pweqlfkj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3weznykgl.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hszyugea.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kdihkyxz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3syjtyuth.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gdliryal.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sjehpmgh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3qfxvhnlz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nrzhenzt.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3udhynvii.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3tztxkxmz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3ieekrklt.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rmrrhgex.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3ehlnjqvt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lbeuyppf.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3kyofjbsv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3vwwxwhqc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3hiiafdhh.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3yvfpnvzn.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3xgvfdjgr.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vofagljl.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ddeczkzm.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rvzcesmc.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3efsivcdq.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3jtqynqct.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ncvhueed.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vsienjdu.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sqobnitd.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3cqtqvayd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3nhpjlgde.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mvupdbbj.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ujiijsgj.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3izaouckb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3ziwplnvo.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nluzyenk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3nopdsvqx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3vflfqrpn.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3rvkotylz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3lvaadfjr.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xcmozbny.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rowlijpq.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3curjeuqc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3zrxgsbkf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3cugkcaex.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3eqiwypeg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qmxswlal.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3dbirzkic.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3xpqirbvc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3unxrraig.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jvlbawix.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3imtpokto.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlztixus.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3mvqebqqm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3zhomjnos.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ieitwvio.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3cpknygte.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3aeawvuse.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3idsrjjsh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3bnxfeqxk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pnmxmmta.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3glyukcta.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ndkcoynv.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ayrdbvek.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rbsevupy.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3vgfdlavx.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eveniykc.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ptybckra.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wuxnelea.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wlhincab.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3medxtlle.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3vpntjkue.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3pzkorkqd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3yzawlfrh.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3ylelbkni.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3owtglspu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3gbsrxcpf.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3ulatsyri.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3jfggyfnz.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3lhkolunl.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dttjgsqi.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3cnkiqhlk.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3crgzyvzm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3xodsrsgr.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3jperpwqf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3majfpvwd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3zzayqeqa.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3pxqtnusy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3kbtrujua.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3pjsdqndk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3mkjgxhnm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3cvlxoulu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3yyozimkn.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3jhzhsgsi.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nbofmvey.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gkxopuyt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jbnbmljg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3qmrcbqgd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3uhhnopit.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3okaiyxau.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3kubbhlyf.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3onrbenjw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3didqjxjh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3cnrxmqmy.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ohseixkc.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kzwsnrdi.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ormdzewn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3rrefdxrw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dfznynij.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3mtbypkik.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3azoncxyl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3zjkcwaxm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ouddfdwq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dcptyctq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vbehyaek.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xjmqcqeo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3edvkqihe.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3bllafhkp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3cwuzmrqv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3unhfqwxd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3pqgtwddf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqwqjnso.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3jnkwpgus.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3quzoawfd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3lqmkumnk.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3wsnveiki.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3tcpylcsz.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3gzdxgwsa.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pffhozva.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3eqrpsizt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3qlhgbphx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mwzlekni.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3avyztagn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3leyvbcfw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rwejhoif.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3zabnlzzq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kqhxrthv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3xzqilyvk.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ltttlkec.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3iuntnalc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3bxhsygoy.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3lbijfnbp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3kbfjkaxo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tiltkage.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3uabasccm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ticjqgga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vktuwxmm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3ygssexxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlzjcptg.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3idapvizy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pcqbeupl.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdyuhufc.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3akwelfhi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3oiunbgpg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fxeflvqm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3lexmgmmq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3jbvpcair.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iuhwyikg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3xkvrscmh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3eczgpyzz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdigbqeb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mrfzwadp.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3gptipugg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jinezjrk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3flchyqeu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qnjfajsk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3uulscazz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ahvldetc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3jhlcqiem.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hevtklnl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xxbpkven.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3drskkqwu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qoimxdvm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3sgnwgeyc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3wfddcdrn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3qlqbfbga.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3bpienqig.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3hhqjxbtw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3dxubosdt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3kcpfwjri.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3uqkktevy.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3hmdnyjto.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3buniacak.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3tujsdzgy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3uzwgczlh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mbepbrre.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3bnyrgjjl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3mvlhsfts.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3podbejuz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kgdtsrto.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3cqplaviy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3atqtkoxr.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3qincngsd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqtphhfb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3jlngfcry.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wcrjtzeb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jsvirmiv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3iqjyussk.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkbuvwgu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3wslibouq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pqjcqwdr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lciiqgji.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3xphaqwia.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ygtloqnm.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3rufilofp.html


<!-- 参考信息 -->