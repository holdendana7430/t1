代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2fqwilern.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2hgidlzzn.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2epittkbx.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2cezfesqa.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2wxarjmvn.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2tulgxwyu.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2azxctcow.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2zypumhfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vktnxykz.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2gkvnxbft.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yplnxici.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2uhosfbed.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2oqzkagyl.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2oakbdvan.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2qqssaiyi.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2hbixaljq.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tenhvczu.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2etglkjjo.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2fnfkybpz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hnedoxuk.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2uuvrwnne.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2xrkorwxv.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bjcmdpro.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mtlnuozg.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vqijiakk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ohdrzqmj.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2bugfrzuw.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2drzjvnmm.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vwnzrjjh.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2enhsfblu.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2qkipmkjd.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kkesgqog.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zpcxllkh.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2vblcuyov.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2jgfpueiy.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2jevufdse.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2dtcvauil.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2luorhbpo.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2kjekpjgg.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ivzqxyip.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2dwwzwgxj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fwzhlfks.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2gwaduoqh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2yphzwgsq.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2olbulrgv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2djefzedr.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2iesquoqy.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2okeipbxn.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2jnythnxk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vosurneu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cdpkhysc.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vmdcrcvc.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kddnvlja.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lmmekaoq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2xzqzhmnn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2nxvuwlgn.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2uwidnxaj.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2lfpjbcci.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2invxhpvf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zhgzqsav.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ljwkuqxe.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qdeqktru.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2bbxqvrsu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2cvojhvzl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2eueiveuu.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nvylprag.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2ulgmzrco.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2exwtqrku.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bczlqnag.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2wdhyicvi.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yhrwsovs.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hldxltef.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2bykguphc.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2bdiecwlx.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2kegjrpli.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vnuqnfmp.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2doohhqse.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2eccnicbs.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2cihrboyx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2btloccyv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2xnjxvjal.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2vzdnaqit.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ncxjyije.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mvrtkpvo.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2oqxzngdc.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xrdlokfb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mxchiqax.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2awxhjkpg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nbukgrzy.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2esvsvxnj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2irhdgqtt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjeasxpf.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2hmnprnbq.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2jymvxgqv.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2ybpithaq.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2omnahcbc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2ippfeuki.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2vzlrylrn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2jforeurc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2qqzwdcpl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2sssbktgh.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2hvfcblxm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2fcnlzcfe.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zpjkupqa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cbcqyflr.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wysprthi.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2spslbitf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2obuplqmh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2iecvvfgl.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xddgkmzh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2rfyfpzsf.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2njdavdxa.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2liuxbdii.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2sqhhfqrh.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gwkzdmgc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kucqlfwn.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2geyoaqjw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ilpojsfz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2fhcwiiep.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2rkskhqim.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jwvhzpcu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2iynykzge.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2alasledw.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uppezzkj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yqeawrpf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tbinidhr.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uxfuopyr.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fuuehlxh.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2qdbpwphd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2irbaqlfi.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2bxfhlitu.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ofguomra.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sjsujtcw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2xsncawpk.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2shajjlah.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2yndccjbd.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kmgvvtzb.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2njzbtzhe.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2cygvlmtx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yyjaisme.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2onbqyssb.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ntryuqkp.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zolzlbhc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2lfbopwff.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ehmfoqxq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nmyjaych.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2qunxurda.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xyvkdomh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2wvnyepxr.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2yzazxyip.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vvvusjjk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2uixvyqyu.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ggoxfhtb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2lgkrnpus.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2runnsivg.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2fxoynnpv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lkgzqtgh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jaoagbmf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2furgeopm.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kbdyvapc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2kbvkwmjx.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2clcmxiqr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2biqbwltt.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nijokvdk.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2uaczctdy.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2eiogubmx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ighwjhyb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2tnkgjsbp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2enngrvsz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2jedxzogh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2yxysrazf.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2flwbegtk.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2wellebob.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2hihrqdsm.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2tidaphwl.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2lcfumzmr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ehjosnoj.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2aretcsnn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2hgyekogh.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2sigrmlhm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xuvzwmzr.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2uqeflmvi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2juakqqeh.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2jjvmvaiw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2gutibrkb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2xixshzaf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yguysuiy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2owtqoujm.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2oxitwpbx.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2qglnpday.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2wpfbrajl.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2dxjjsvnh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2xowrugjp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ydaoxetj.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wvuuaags.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2urzjvvvb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vydvgfyf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2secrnwqb.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zarnguyy.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2joifrkbt.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xhbuxhfk.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2adhykdgh.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2rykiufoa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2pbobqcho.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2bcqibbfu.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xfmamdqj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwxpdvzl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2oiknfsyk.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2gjpvcxge.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wuexfpry.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2srdsuncz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jafjwyni.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2awdojmie.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ufjedfnf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2akoirfyy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2inzkesyu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2prkfigjz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2ylgfpqwx.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2wdpqtpyb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ckzjjivc.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2halzwsze.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ltuakyxs.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2nsrwqvzu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2laalomyd.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmgatjhg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2gogdsivg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2hjntudrj.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2owsojzgc.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2jjrwtvhu.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ivijkrge.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fpywkvoj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2bqjpfkoo.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uklpqtno.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2psonmoqz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2szaghrsx.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2dwlqvuxt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2lxfnhcjg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2felhxene.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2acnjnnyj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ybepcsrm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2mmxjmuaz.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2npnpjovo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2qgvoqhko.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2frxuuidl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2kwuzviqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pcztfsql.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2dkhducyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vduewgiv.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2xcqfqdty.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2shjekzat.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ntkduwci.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2avakjvcq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rrmxllnx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ixayujru.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2acmgvclb.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2akqpxyhh.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xyrjlpsa.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ehblfvld.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2nretroug.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dyiuipmm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kqxypopl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zyjlifhi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ahyhhyly.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2phamtslw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2gtvtrtxm.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pidqpjfu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2tquotvyb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2gmemxdny.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2zmuipmwd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ouzmifkn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2chmfnuna.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qolfwpnv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2absbwfgk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2autebdup.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2poweptfj.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2awqkpbze.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hedgkijo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2otbmsoir.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2tcdnqcrt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2grmxeqnh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xkcwfzuw.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2yvfcnodw.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ehlmxxfe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2dtnasevp.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yhipiixs.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2ljysanbk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2efyslxlb.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2zkqdfxcy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ffttmrqr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2fwfplvqu.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gwdqucxi.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fypxgzfc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qonukpoc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2rqwieqss.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dxllujvb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxwluzav.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2rihqsbud.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ebujstuo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2qizjvwyc.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2fxvlqvcz.html


<!-- 参考信息 -->