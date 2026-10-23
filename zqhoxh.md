代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ccxhyeyh.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3ctzomaoh.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3hkktlshr.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3uqvlexhl.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zqpjqxgo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dfrdfvph.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3vxtxural.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ccerpdjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sytyyfav.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3wvkqzfyt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpfwuamv.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3usvuqiwb.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3kvwygzhh.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3yiwgujsg.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3vrchiqrk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3jeovvyok.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3adhtfwlf.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3siswdouy.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3cadnxbbl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3idqtjmcg.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ulxdgmiy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3oqcisbot.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xkyftgjp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3gibrejba.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3rsvywshd.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3omrqmqri.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3psrqmiio.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3ymwmhdgp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3gkbduedo.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3kxawoxod.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3qlvhuybk.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zsejsxpx.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yazmypek.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3twegnrxu.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ceewtehq.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3usajfdas.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3mjkgizvw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xwlkwfgi.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3qywjtleg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3amlyiqzj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpbeizdv.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3hpmqcevv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3zciolhfz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3qgfeqkfm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3qpncgabf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3yeymrcxo.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3wzwolqpq.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3flekvwym.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3golurhry.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ybpchlut.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zhvizhgg.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cpvddfwq.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3rfbufdvc.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3aopgokxk.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3pccctqtn.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yiadbrdj.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3tczrsbhm.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3gqyyubgw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3ybknxmot.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3whlkhbmk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3mageofwg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qpedahqt.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3wrqwgeku.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3tssreonb.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ylgakvvp.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3eywidvyh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3jueknaqa.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dhslyzem.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vmuacsxd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vpdxfcip.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3wlxclarh.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ltxhfbky.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3rhrwfldt.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3xfhihdxz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3whgjlkrg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bfuhaiqe.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3efnvwyzi.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rjqrmitd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3hsjfshop.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qwlnoxms.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3yiphemgl.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3zhuwlrjs.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3aszdgwsi.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vbllvmoi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gubjncll.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3qpelwmeg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3xxeunkal.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkhslixe.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tjnxodaq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vhhuvlyo.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3fhtwhfai.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kquqjngu.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3iohleklf.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3nyvqytni.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3wsgnmkqv.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3adrqxclh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3jzkqxvhd.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uhkpfhqt.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3jprobtav.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3llnlomcx.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3vylsldmh.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3vjvhlzyj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3vthxvadl.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nrnkexpc.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pooetyqb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3pdulvmhs.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pngsjiii.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3qbfkxwce.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jvunzwfh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3gmqpvwou.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3wmwofwnw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3asunrcyq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3rribjtge.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3mmnalkna.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3hqsmrqab.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3coapsalo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3odexiken.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3hsuantlz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ftqhpyrr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3ipltfrhu.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zdxulvri.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mvlfzcfu.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qareqtsq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ivnxfbgx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dxmtjqbu.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zpwrryys.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nhkimibd.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3bbkasonn.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3iowghsxp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3flwixufj.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3pxmzujff.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dpxbfeiz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3xvhsuxrv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3tdvmcgvh.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ujhnolww.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3nnnujtwp.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oefgbrkv.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3pzseyogx.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nocsrakk.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3whymxpfv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3orbifxrs.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3kqrkdmaf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3jugdcrxd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3pxfrtzmd.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3nkjteotm.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3utygvbuo.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3nqgkduga.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3papsszns.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3frlmbtdp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3qtbwokrx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3svawfqab.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btkcxnwl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3aklxfozu.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3yoeiosyu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rfxcboie.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3otqhqlhx.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3dsvuyjkq.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hdsvtewo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3jvtsifgw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uorlcner.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nnifuxhf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mnipcigx.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zlwxhmpz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wagxkitd.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3llzxifzo.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3berkzynm.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3gwdiosgu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3ikfeinhn.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3txjhpwap.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3nihmkssb.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3xkqeqcfw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3qsqulrxv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3uxmjqfpp.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3bmmsfypv.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3hojkgegf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3rsjkeohq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3fvowggnb.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3yblarwlo.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3udoqdovh.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3msluxjrg.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3eonjubkd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3asotblsm.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3eflaqohq.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3cxdixcyo.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3hzciynzu.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3upodbwkb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3uprbidrp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3fnvmjdyu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3beymuwsw.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3obktqzka.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3czwiaxmw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3muhqtrjh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3itdqdupp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tuetepcc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nczunrsa.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3vaqcymwl.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3sbqzadwz.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3esqkqntu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qqdswrjm.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3tfcthkvi.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tydjkbbt.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3dthseyyr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3jxtdycvh.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3siylasbd.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qvmnoptl.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wsunwuoi.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3qcvbkmba.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3kcqfbbjj.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yvzjtthr.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hernbgbc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jtuplnbx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwdwjgiw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rwdubgbp.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3inmkepbm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3wwkyorgs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3qsbwvhwf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yuvnfqno.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3tbgtvqgq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3bwsugihg.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3qbajgoiv.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3vjhphykb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3dczpvqio.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uchnalpv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3gkzpjoye.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qbsiomji.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3fnpyrxom.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3itrlimch.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3iyhhujum.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3xoyexcsv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mxavhtzu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hkpfycfw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uyrcdzxz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ouuoogpk.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uxnpieye.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3wpklrooe.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3gapojtra.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wbfjypbe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3rdkktysw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3kpfgzato.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3uvucamsz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3bmiropgm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zbyxgofx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3nnaybcnz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3uruajqjf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3ziibfzko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpguoywh.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wcvkhraf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbylzoyb.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3wgvzufam.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3jgloloha.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3admbdfka.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3udcjqzsg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3iepdrkww.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3mkxuggwl.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3mnnynrlj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3otpwokye.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3opjvxgpj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3imydkmeh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3oddshspb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3hvommdck.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3fdihiycw.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pfizrjww.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xpunbunv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3pfmbjfgq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3nkqeddmz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bumctrpk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3xkjjepbz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ertfwdop.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vxnuwyvw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kjdjxhhd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ezzhjcpk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjypvlmh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3exhpsihv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3gpeotlca.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3cydkeqdv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cqbvmdfl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vdwvcems.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfkezkqi.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bljivmkf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wvjwxitu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3hjatfivq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3gbddyhzz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3tymlbdwc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oaxgprwh.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rqyavcoi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mvraykok.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xprmchuy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xyzygwfo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rtmvmgqk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ccifsncb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3yscefnlu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3eblgxlax.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3pbaxybcg.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3sqnkghzq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3rldmfcpy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3hdldzcwi.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmaxzhot.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gtulcjrb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3nzvjbmmb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3svxssdxh.html


<!-- 参考信息 -->