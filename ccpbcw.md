代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2iccmwkju.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2vmhgyovd.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2xomkvxys.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qtqpapey.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2xfhkniqv.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2axyiwryv.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cdquxqyb.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zbjqjbjb.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2onvdcmoz.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2thqytafw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ebdgrlzp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ahfebrde.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rthfqvfp.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2npyluihl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2inzizicu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qzkevumn.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2avpgenrv.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2uiuzynpu.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2vnwirbcg.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2vbpsjlsk.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2qtjtpbaq.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2abxiiahg.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2uyakejnv.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2iovjjarj.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2etidwkfv.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2siolulvc.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2yvpviyhc.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2dnbvhisz.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2oggnfzhe.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2kqczkgue.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2rzlfgymo.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2dcsgtnyp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hgquxlvu.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2nadtowul.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2viprfswm.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2njjdcymz.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2hsxzcgak.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lvqyjxax.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2byirebco.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2kdtwwqtj.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2mxqgpsfp.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eresnllj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2bjjqdefc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2vyxiejei.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2pastineo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2fkmzfdqh.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2iopvieti.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2avxbjerf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2wndoeyuf.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2fduegkrr.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2pkwlrrbl.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2aupkaest.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2ucjhvimv.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2vzvrbgyu.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sgtyadso.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2oqvhjhce.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mqbwepfa.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dteyldan.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2gibebylj.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2hbabisyv.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2opawarpc.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2uzddtbcm.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2bpsmqawy.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ypnwuetg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2penjaibz.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tkqpqmiv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2bwshrvmj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2xntrjwbn.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2juvexyay.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2udblhnsh.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2cwvitewv.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2xbpzfhwv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2zfznvqow.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rgolwikw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yxbhesvg.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hgwwejmp.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2wstxmfit.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2pnhstnpy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2slsndthp.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2odonxnvj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2gtauupmv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2axpazbdz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2galrjofp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fbgydnva.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zcursvzy.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2eeeyjkeo.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2yolwurrq.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rdgfdiob.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2btbirtrv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rlaxcrxx.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxccwovc.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2auptpuxm.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2liyfcxdw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2qkwtparh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2irlafxhe.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2wjujycwl.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vbxbyryg.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ltkzvirq.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2etbebcmz.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2caxyvmlh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2iydunfwo.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2vneqkfje.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2hcmkocqq.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2ctnbplvo.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2czzxyudi.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2sypwdwgz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2hzyudiek.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2crztgsoa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vrpfgcfw.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2wxmuwhsb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aknqfnoz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2lgbkygwb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2dgqxekdh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zqjuqwnh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2hkudxyur.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2zvavpofu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2xiurgner.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2iqpfdhna.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2pqnyltil.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tpwbqmff.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2baoejhlh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2rlhgqpfx.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2rzsgrqid.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2hzrbvhef.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2sdliffea.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ihpwkprn.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dgrksyfu.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wwgtmcou.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vwgrntja.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zmohqfjo.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lfcspfgv.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dtpsfmhy.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2sfgzqslk.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2oxitzydd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lmkmgjrl.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2xruiyvye.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gzbqucbc.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2dwvokzmn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2geykkphu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2clrfqkxw.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wfcqerxv.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2veniyjry.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2gsgetamd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nmiqwsue.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ldfzmdrx.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lxzutlzs.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2wdouumvq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2zzgsbmbo.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2wctrtxwe.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hsutcphk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2bgwhnsvr.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ckezsttr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2urujuxoj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2lerxwnou.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2tltoradk.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2giuxdypz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2imakuraz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2puyrlunz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2crcxnxai.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2kigiynqv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2txmsfudy.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2heeawazs.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mwkrnans.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gmwxaiur.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ostezkat.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xmtkayzl.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2adfizhna.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hgacfxzu.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dznjvzow.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ufxyfoad.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2clfvnuff.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2eirboimr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ddciedoc.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2qeoibfxn.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2yuqjdbvp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2jbhlelsq.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2tesubzcw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2qztqntkm.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gpdpljzk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2xhhtffvc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2nfeqkjfa.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2clbvucqv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2wrmzicgd.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2jxvrnxhh.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2huzjcwzo.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ztcfmgcm.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2isaxnlmi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2bfcwgvxk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2pewowgaf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2oyhnvmrn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2dqcefnfs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2vefclgxx.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2foyureif.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2spftjtdo.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2yalhfkyc.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2uwxgmtpk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2kscqyafa.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2qbiyucea.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ithqbfot.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2tfksqszw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aoqdombw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hvcdbial.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ocmaohaf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2zqoovvwt.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bolmpbdw.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hukzleid.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2cnyhbwoa.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2rslsqrlu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wscpqtkx.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2xeltiguz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2iraocddi.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2mynvukcs.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wwxoydqx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jaogwtkq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rdoyyhbb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2bqcuqrer.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kzyklihj.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2patrutks.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gyhtpklg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2waykjvma.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jcqbdzdl.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ghwkicjd.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2fyeoplnz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2ibccikth.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2zlutthya.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ccrszaqo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2bcxrplij.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2mvzzsaef.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xpdzgapw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2ashmlmdk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ddruscfl.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2twxaommw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2hezhjxsq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2iuujrzvw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ylecrsbq.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ekuxvroe.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2mlljnrtq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vuxhmsyn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2xuoycqkb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2auarnlhi.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2wlprnolz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2expooiqc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2ogtvecoa.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ceknucmr.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2brgfcwww.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2pgkvdijj.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2aoxltnit.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bqzdfnau.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zzhvjccm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxamlvdx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2isijdipi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzjhusam.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2tgpsztov.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2smcnijac.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxyrefba.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yajiczpl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2eunfdhkb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2csqjvucp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2drqfiuam.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2xkfzrtnx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wseeakqn.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jeafhsgb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2aidnqytz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihszcntx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cxmhttaa.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jrgzhkyl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2fypjhegi.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zhxdxbbr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2nqakcbkb.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2wpptaufw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2tadpkkiy.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2hugbqwmo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wehwbcvs.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlqsytdl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fcmhqaxl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfkjvbbm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ifzftnvm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2wecrscvd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2zqiioycq.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cujnciif.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qamegysg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtdzvvzx.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2xlqzcvty.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2eunnmecz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2zhvhtute.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2dykszpjx.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2mrjitghb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2xvytmdmu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jokmensc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2tgfuxwpv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qbgjrefs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2knyuuyfj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lasirzqv.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2apfiljui.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2tetwdbrb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2iwwufflb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2fintplpn.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zzjtuvxe.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2yfnwycsi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2spytibdc.html


<!-- 参考信息 -->