代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2sogsrihw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2rwroukre.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2invkopei.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2qytrsjtc.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt2vuctnngg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt2ceqlojir.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jngizeng.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2mtpyisnu.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2edfavymo.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt2njygszej.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wgfiewsu.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2cpdtndwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yyoyqiep.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2hclvkuyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zquflcvm.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ffjdmjld.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wrrmboap.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2aghwsnmb.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2hhjzhiee.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2obpwxnup.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2juphfubc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2makkdmdk.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2qulsyqnp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2xihbzlfc.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2zwjmtvlx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2hilazara.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2rmyrfpus.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qknhsjny.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2favvsvfb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2adtkahdn.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2bbpowuub.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2aqwznmms.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2tkkzdhma.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2ympnbjpt.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2citrdycm.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2umetezlj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dtohkjmt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wbungdpi.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2wzrdxdey.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2coikllqp.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2fwwzoinp.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2syekdhib.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2evylbwhd.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2iibigndb.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2oasxyvjd.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2ojecpgtd.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2xqjpnpld.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2nprgsaya.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2qqodsqze.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2kexfzmht.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2befemysx.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ocgconpr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2rwolcfmg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lhzaxbiv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fvwnikwm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ymqtaunn.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qtmbdnkm.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fvztbooy.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wtcgugmp.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2qyjcwzim.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tlkalfko.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2jfevjljd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2aadtzhcb.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cflwqkng.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2woynkccm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2gbnekgmu.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vvztpcwf.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2qnpasdey.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2hotqylyr.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iaqgivmk.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mjhbqnns.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2igxpehvr.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lfhiigha.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2lagzvgqg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kdeqpnlz.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2gnlfrexg.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2gkkquegy.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2omufxube.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2jdnwlzni.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ahruexgn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2djcqixcy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2wwgkbniv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2ooqhtfgh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2lpmpqnau.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2zxgwpfvj.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2xqwnvbif.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2pmhojiap.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mgjkkrzi.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2frdfgbve.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aedrfflg.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgqiaies.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2cdpwrvym.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2svirzdoe.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2lpigcqlj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2ptekhwet.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjzpuaaw.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fkbbedfq.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2tefjeren.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2obuvesce.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kzkulxgj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2eumngceo.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2mvdfiwrx.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2kasnjhdt.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2gryvixry.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ndacxokp.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2erspbroy.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uvykvewp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2cebsmdiw.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2irxffwwx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jpzyufio.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2abmtdrkh.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2gvnuizvg.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2oevgzowv.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mtksmxri.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zqqwkamy.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2tbdwxvgm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2fswpwpgh.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fwjkutog.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2ceyildlt.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2kiarxclf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2gctynztj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wnzrkhym.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2wzinfnxu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2bzxpwhvo.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2jcosxfls.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mhnuuzsn.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2htqcmsol.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2chwloqlh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ubylhmmp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wyygmqmb.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2nwguppis.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vqafhvel.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2yvrijhzm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2nblrzmme.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tajtxska.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tlzddden.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eqwzscsf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2awmmyreo.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2gmbfccwf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2qfxsxwen.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zoiqvanm.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sulxkpth.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2zrxocydt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vuvmwlux.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wttupbwj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dlmhnomq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2jhxhbqkf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2iylxivqx.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ekcnhocj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2frzgbgui.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ywtkxprw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2qcsndovf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2tfnblmmi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2hvcueqpe.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2jcaqcdme.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2igheqlis.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2zpagkqrn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jvmghbdf.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebekaiku.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2dkvlmzin.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qunlcxqv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2pvjtjrpk.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xhqqmgwg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jgepgzlb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vmnlizpp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qgxutwcz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xumpgtpu.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ckqrynib.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2njgmynti.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2inyoeskc.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2aacxcgwi.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2vqaihjly.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2thcktchq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2kvvpmwqt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2wrdunbdi.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2reedwzun.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2zmsygofp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2xmyhdlfi.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jltzjwfp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2umyjugdn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2qxoqpoxa.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2pcuxrasc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2tclkxvhv.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2glrlvewt.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lmbyjaur.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2mgelgcne.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2lysocege.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2phtubawi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2gzxhifuj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2pxuhqpwt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2mhtkfpms.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2wecaslal.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ddykagjm.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ccnclprm.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2derqoijp.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2fnazmkln.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2sjentziu.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qsqwunbq.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vlmgyzzi.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2fuqblbdm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2vvvuxtsd.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tspscoox.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2akvtfyod.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2glbouhqh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uefhrloq.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hddlsffo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2cmalppbs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2zdopzncr.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vfgqvjpd.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2pnuvwonm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mwzmftqf.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tidpqidy.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rfxuzbcw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cmjxcngj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2hxmnqlzs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xnxrmkbj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2vqoucxvf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2bbtlciju.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qhsshlrq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2cpkwwlwk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2hblwudtt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2iskdupwy.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2lbmkbpjw.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2qalxczcs.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2eczsvece.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rliukqet.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2yinicfxz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2xtsyyobs.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ujuoimke.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2xewilbcd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gnibfgoh.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ppdxqhgy.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ufxgpfnf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ocstrgos.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2vrcptvtw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2komveqmn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gthjxuhc.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2zpfgqnsj.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2pfasxhro.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kkwbynwn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2xghbbbfd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2bxvuygrj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ajxothkd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2otmpzaxs.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2benrjbwc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2qogiwtps.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2kvzsyfed.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kossmgrl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kvhnbjzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gzzzjcaq.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2reryoqme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nxtfgwpw.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2gvapnrtb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2arkhvxnj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwwcnofd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2plkvlqda.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2jupmulzz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vhattuin.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2kipcdldv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2zpbstxfz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mkbcwtjj.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2lfvtdtof.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2mldfkxql.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyvhffsc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2phqesufg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yterxgpl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2aibewczh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2qtdgogax.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2aolnqsni.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dsnhosgw.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2nfojmkdm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2uqbbnsui.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfzyjrzi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ycrwmfdo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2clmodyck.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ccmujhle.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2eaeatcre.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2ixbghomo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2eqwcefie.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gvxptnng.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2mrafmoqw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2uzvellat.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2lecpzyvl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ycirwicg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2frsxzapy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2aowojrmi.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2fyvpirkb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2mgjgkjdy.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2flajdxto.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2cysfwuhs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2lbjujtvl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vsduyvgn.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gyqawpiy.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2eledlmya.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2mgscbbbj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2yqhrmevf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mebqlspp.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jbiyjqym.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2daizqlmo.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xyarpdsl.html


<!-- 参考信息 -->