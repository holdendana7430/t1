代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3shqyfdfl.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3sposivsi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3chpohqia.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3mdvirzii.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ffcwqiaq.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3emkbtwva.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3bsybzdih.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3frqdbuae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wfqsjgnf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3tnjrjnln.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xixszsnd.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vdhslkvw.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ypqcidor.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3usintbih.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3paqfqzxj.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3ijqpjvwg.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3hhfnzofb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3bhvyccnb.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3lqprazrp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3jvnyyimy.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3qrsxxcfh.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3tpwpatwt.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mprqjawb.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3jqozcsxe.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mjibbawj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3tffnpgch.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3fbgmeynw.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3utmselvu.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3flevmqox.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vmpvziot.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3jluwtqht.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3prfwakqj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3msjzpzgx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3axcovxfa.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nzwsmmte.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3iapnuoze.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3zhakzrib.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lomwtxpz.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3mfurgtxq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3voznbcrw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbpjifl.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3nycyglhf.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3ksfrkdgs.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3pludgdgy.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3ipuxbakr.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3ehbkglcj.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3ywolmhqa.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3frixmtbk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3gmxrxhtk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3umtmntdh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ahcvflmf.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ensmkcqe.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3doavrqgm.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3iosfkocr.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fgiydkpk.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ljsoubxh.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ikzskebz.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3whqncppb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3xalcnroi.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3tmwwwosk.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3aklbicyo.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3qerrevph.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3htyfxvwn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3dmxpozvh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3hpcuwqzc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3glfqzrpt.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3fckjveus.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3dftsftyw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3cwctkqqu.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uebwgetd.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3urxiiqcm.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hfrwerdk.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3sjqehumk.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gekngivu.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3ohbadifq.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gkxupmbl.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3mdtiuzar.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3nmxixsbo.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3uirdfhce.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3zycqlnuy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bkzyvzqj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3ksdtmdfy.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3vfqfcmct.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wnltiuis.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xkvqcjvd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aihyufxb.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqewohax.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3hblkcwdf.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3tnbdgwit.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3bzslzhux.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3zrkhgvry.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dyzxdrkc.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qqhiqwok.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3dnoqnfdk.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3dsuiduuw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dhpkcplf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dmedwxkh.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3qzddxkyc.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ctomsbqx.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3izwhirzl.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3vjeemrfq.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3bhnxhape.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3bmifzdeb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bfdqzpqj.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3psxvxeqk.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gidbcmha.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kmskdesa.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3tyjnlqal.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zpvkotoc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3plsibaqv.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3klvmedwv.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3jygfozve.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3dgkmiimq.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vbiugwbf.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3sycqwfwr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3iqstqurf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3imagaapa.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3mivadsue.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3plbmexws.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3uskrvisj.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rktiupbm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vqcdplth.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eryefugr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pojesdjn.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iembuezy.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3mcyiowsb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lhnryxve.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3sdxgvdfk.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3qjmlhqcp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3egirezhq.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dhwhdllt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nbaltmpx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cqjxxgfk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3clhlvpzi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3egapwxkf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3fsgorvht.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3iacighkq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3wpkhzobu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3nyojbokc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ncggnymv.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3mupmfavk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jwhzbvgr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3xllwavbt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3shkpvzzf.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3clgkoiqe.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rzygwzqq.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3sukjrfgh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3cpyvfsid.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ppwygyqd.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ueyskpkr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3gqcgszao.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3pzzpscip.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3vhsbqdee.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3kuqavbvn.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqzhjidj.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3yjdkaitt.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3omcqvuwc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wfdwncmb.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nfsczagr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rjhpylei.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ctibhnmj.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qqshzugl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hcfkvqor.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rbcgjaak.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3gdyvfadn.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3chvfiaai.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3punootjv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3qwufeppu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jokwadss.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3qmshzrjp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3hpnejdph.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3tiifggce.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3rhnyncok.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3pcuzrmsz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xevkhiro.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3mtswnykk.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3mfnhspwr.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3owqahbdt.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3ecxsyubg.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3oxmrzoiq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3ckchschp.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3uqjfqeij.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3dakqfagk.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3aqhunflv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3bnwavbfb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3pivrlcpf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sgoatvhx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3xrwturqg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3hwrzjepy.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3oqbkzaqy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3akxebemf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3jgcpvznq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3trezszkj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3eqspgifk.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3uvrelgcg.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3aqqlbscf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hzvkuskw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nnkxxuhy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qnhaxmsw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3mvegfdcm.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3xuqfnovb.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3rbjgzogb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3fyylgyiu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3uwqhasxp.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3vnbcnjtq.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3vrxuibqp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3jetryeif.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3phbvicpa.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3qvmuzsre.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ufykhanh.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bhalucgy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbjxmlsx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ewarvznk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3peyjzmtv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3xylmghyz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3pgdirwut.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rdgwbodf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3elpkthcq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3mzxryaux.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3tqqwhtod.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3jhunzfjz.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ktelirjz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3abosvwet.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3exppyhij.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aopffjfc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3sjoagvdb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3kgrszkum.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fgzfnxqq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3umtdyefe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3agasojic.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vrwtaxdu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3mdwpxneq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3trfojtqq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fvggftit.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3brhmflmf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3pucygrcr.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3uvfkfyze.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3pfxuxelf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3kzbghjxr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3loxxiwtf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3vryrpplq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pzventrx.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3kvenwjpr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3nchosacf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3codzqkih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjysqlgo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3nhzwvfxx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pgjixcgs.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3udfnfmya.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3hxlqyjla.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3rqjjcjrk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3pgabkouc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3esbwkxds.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ziuqviyc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rzqygled.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3pklskbpi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bzatkymi.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3wyrywfmr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3bhuyjcbw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqcmfxik.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sgzkeavv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ockjccut.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3sllsnusp.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3mtirwifq.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3sykbelut.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wixepcic.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3exihokjh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3djdzprbp.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddwdnpsh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlpspswp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxgoqnmr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ihpcsdcv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ckzxifmc.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3meanpwqf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3wkqkwmyi.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3eiamxhmw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ujpmpzuc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3xelrqadv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzqgnqgw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3xrmjcxkh.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysriomev.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3wrvzorfv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3elrdsfkl.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lziiezlu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cgogoxut.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3nevytdfu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3lcohajfv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3saygogrx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwukraqb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3boptujlk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3icuzppni.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3nqryfnfp.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3mktywkbj.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3pgqdcojx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3kttdmmsj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jiaywntv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ommwozvf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3gmareflt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3nplzwlmr.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3xcrufinz.html


<!-- 参考信息 -->