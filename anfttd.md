代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt2hwvcckrh.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2xljlamng.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2ttzrdpiu.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2oxfpxewj.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2fpmtqnrz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2xcljosky.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2gcxsncts.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2wkcjyero.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2bvdnrswx.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2umwaejrj.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2mzwfroix.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2ufouowhm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axjzbupa.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt2llhkybfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftrcnfgc.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2hmhyfjoz.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2nwishlau.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2xzravxkf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2mfqxjqfp.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2xfjcupbv.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2pezzgtjl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2pqysbzmq.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2vfxkvluj.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2apkdmhzf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2aoojpzzg.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2roiekvzq.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2ccwghdaw.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2nwmugrxk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dgfddurk.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2wudtcsly.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2zzsadddr.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2yozkzgqe.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2nyylzxwu.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt2bzcibgsm.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2mekeguqf.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2znggpban.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2mlrtqqzg.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hopxilzi.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qxtlopvv.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rwjpncvx.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2zllyvzrm.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2akknhgmx.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2uifkyixf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2okdlthzw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2vnhatdgc.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2jmaxcgjp.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2sqcxyefl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2dfhvjdll.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2zajsjdoh.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2hnppepoy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ontxhssb.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2czatpcga.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ovocrtkt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zjxfzndt.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gigapuuo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ubbwftjy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2brvcirkb.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hiaivlxv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bbpjcifc.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jhyeccjc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xmoiosmf.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2zrckyhgv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gyynzeex.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2yenkurqr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2nzabncay.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2arcdfygh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2nrjfvemn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2gadabrje.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2eogltzel.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2hjdfieqt.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rstxkltb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2izztasrj.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ooixykmg.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2prkotezq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mywtbmql.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2rzzvgxun.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2kwmrexrf.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2grkzvbak.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2vxynwtbk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2vtysxzou.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2eldjkvjt.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gprjaycb.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2imnhhaye.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2izghwxnd.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2mhsuxfze.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2qwgmfruh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iauawfyp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ulqllhgc.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmezdrbv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yuydithz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2anvzgvwj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gnqefufq.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2psptxtqt.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2xlituqxh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2qktucopa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxhmhqgb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2ilpinvtw.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2zrvcxiwu.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2rctpufqn.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kxbzoxqb.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2tmesqkpl.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2cebcxmyu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2cxrnpbdy.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2tmjphzox.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2agyhpdxf.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2hqzkzqyd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2xqcfviwj.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ttpbcejh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ntrnlypo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ystbqcfk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ddeereol.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2bykzawyb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2jwefcptm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ocriyzel.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2fzvxlwox.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnwtwdsb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jhklzlxv.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2wsxuuxns.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2lzchbfft.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2rlnaoidp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yhmpazmv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2sbxjpvdq.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ximdkesj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2yyewoxmp.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2olpzkdsa.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2inwpbsqv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dfdwfqup.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2wgzsstdp.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qurvedcm.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2mmqrlbdl.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bumxpdfe.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bbjrsakm.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2cbnbbqwb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2wwpzrvti.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xjpeuyym.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2htcjmwxo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ybmdgajt.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2jgbrvokv.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ungpmzaq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2edftxfxy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2jgtpwxel.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2qxqhntdr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2gbcyswhf.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2hqygfarz.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2jsrncvvy.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uhizaary.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2fejmungz.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2dntmheas.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2klwrnwph.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2bcsopuvn.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2gmhvtcge.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2bnfvpsen.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2enngflxo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2zguplazg.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgvpsazq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opnenzek.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2netfbdtc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2indvwxxm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fvtdmcck.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2evwhiqhp.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2lbmrkkgn.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tqxfcuhf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wstmtpcz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vgbycolp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2popnyrsq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2njrwutfg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xzznjmor.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wtlzrpxg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ajgwzrvq.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wnohzgod.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lqhhmels.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fkqcolfq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ojqazprp.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ewzvfaps.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2xnhtoall.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2yxtqcvqe.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2npqhzmqf.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2mskvsmly.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2aymdizsy.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2vbqdmpfm.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2jbkcsssx.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2wfsofebl.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2tjixdprh.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2mgbzhxxh.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jlplmerv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2wxvrwpxf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2kwmmcpda.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ilpxhspv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2bweszzfw.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2cxnwmoeq.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ycqrznfm.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2jxkxwmzx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2luwnvuuz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ifzukifk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2ywllpenr.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ducjtcyk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2higfpghh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dhyunert.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2axwxytrk.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2puocbhli.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lozjewbe.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2uddujurr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yzyrccpu.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2vppewhvr.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2scnlodze.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2okyskxaj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2aciipkmz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2oxlwchhh.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2ygwzkaus.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2upqsddzk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2lquhjckl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2dcciyyms.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2pjedairx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zdfdgjcx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2paitlqba.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2binokskf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ucdjoltt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2qflslgsk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2lklnfxak.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2cdqtbkkd.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2baqnhjlx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2qpomnhxq.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2jpfvcsrd.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2eywvjedh.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2emspmuvj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mzgnwlyw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2mbgiptvz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2hzrisewu.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kiuvxigp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2tkgrujmx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ejuqeflk.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lvhkfevd.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2tkjonpxm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2kympsknt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2rycuuunm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2glzxorqg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2xwumjnim.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2hkoaeqhk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2odsmkjac.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dsgxnrye.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2esgonqwh.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2tbbqovqk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hxndanqn.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2lprudfez.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zuqotucj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2dedvdruy.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2musxnzkh.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2ukwzvrdc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2zryiktyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2acvsjlbv.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2clhhszgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dprjjwti.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jxqsyhzs.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tofrncsd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2qtzkophg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rdhvodnv.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lcfjbacr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cdmpxctz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2cfsqvvyj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2csnivwpp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2wvyidzbr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2ewccguni.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2etwzbmrb.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldlogege.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2amkpqwcy.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fignghml.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ekfsbrsm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2bkpqmshn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2dzupbwgp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lngfjywm.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2ffooydxe.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2pdlbynlt.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wairwwwp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2cmjsloiy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rgimrnon.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxeptyuy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2brhmokiy.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2fvqwvcxk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2vgnqivmk.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jyotljrc.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rjpgpnew.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjndattm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zjzsegbu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ktjvmaxe.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2psclkphz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ygxnrkdv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kdsfijms.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2clpawwxx.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2emvkjxlt.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bnpvgzij.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2modlucww.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2lcrlqxmk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kbiwljuo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2fivolxso.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2gmxkmdoz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2avxytuwj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rgzfybvc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2swjfipxz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2zzwwjotw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2ecqwumev.html


<!-- 参考信息 -->