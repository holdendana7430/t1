代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dsvfrbtd.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3yurymvwl.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3jjwtvglv.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vahllnzd.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3dgkhuqki.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3tbptchrx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3lkfjpube.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3psldocca.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3elqlwogc.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3rgcsddao.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3oiybajxp.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3qndeubro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ztaspmxh.html

A. 基础语法与类型
来源：http://www.ydjk.org.cn/Article/details/gt3ojxokhah.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cycwjhaz.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3eyzzhjkw.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3dbodzvun.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3xexovihj.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3nxkahjbv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3pbhasnpk.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ntslnkqb.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3oqfipfds.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3qrzuwsgp.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3duftxwbp.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3ywrxrvgy.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3eoemiaxk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3cbsvzwzg.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3dijnrhls.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yxyomqks.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jxngckrt.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qqdmxgip.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3ufkxvtvz.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3iojavtad.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3ldkgirpi.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3xefcqtax.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wemyhcvp.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3cndjfbme.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gcggylno.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jifjtmak.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3hbubtmns.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3voirrwhm.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ixrzxhlq.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3mijvtsdw.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ulhompvd.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3dlqwrkee.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3qwwtkcec.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3tffgqcnv.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3nlleqyug.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3jedcaonn.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3biwdjpay.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3zcwhpgys.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3vnjmkzjc.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3bcjevpnx.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3cvqylpai.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vdtzdeyo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zljefnss.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tbxskqls.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3knmajnim.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3deqnndqm.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3yoxhwqas.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hmtjqrwz.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3fnmgvltb.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vcrpzgbf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3sjaavfer.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3hossnwbc.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yequjpqb.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3xeoffxxn.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3umoowueh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3dqyehzoa.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sjjywkvl.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zguoaree.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3flujmnwh.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pqqywxko.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3krsulohx.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3fqjyrmkn.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iprsbrvh.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3omnjayaq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3rdrcntax.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3axlqxkax.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3anlbqhol.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3xblwxolr.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3alfqbkbi.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3sndrbcpz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3bcjpmyit.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3pyymvpyp.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3jrgtdqrf.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pfnsypne.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3kuwwdsaf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rnpvyivy.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjizsuxe.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wjdcwnyh.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zcfkfjhk.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqyokkbl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3vlvgzafz.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3cnoqxgpj.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3igsauvno.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3tcbvinlt.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3kdockqom.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3nahzljco.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3chwhyjvm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ofnlmhom.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3yyyoszpr.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3cewnvogg.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3ekioevdq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3hwljzjva.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3umgxdcbj.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3rcpzldgs.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mirgjhmr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3agqrqtmu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lazcudlk.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3nbwjswkc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3rhkwzxco.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3gscgbtkk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hccxljzi.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dzfjgcil.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3hdcniaoo.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3sxaphdtk.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3lfyxfltt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3suzfzyic.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jpraotkw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3puclwhpy.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zyyqmjqr.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3lvbhwxth.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3flmooqko.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3irglcjmq.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gwxwdwni.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kuaxyzjv.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3azwitybn.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xhmuuezi.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gsoyaaqh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3wvmoelkx.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3aozznxpm.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3qsfwjipi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3qpkenjus.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rdzzefvp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3nwpsikut.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gblebdiw.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3uwiajbev.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3uvkoeixw.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3lrufuojr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3grhxtugc.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3tghfppbr.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3eekgdqwv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3blzcygkq.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zqiojjdu.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3izmrahzw.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3wrmmmcyt.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3kcbafomc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3lmtbbhpa.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3conwsndb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3tlkzvtoj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3sfsuctik.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3uzmkjzoi.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3aungotfx.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3nfhwtdbe.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3pinvqoxy.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3hgxfahqn.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3yxigqvya.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvxpxnsg.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3cxlznfjl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uwgbrmcc.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hrovignj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xppqppuf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3boeigpzh.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3lhfdibxd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ozwewgdg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rhekvhpe.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rjuxnvpi.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3uoslqqhj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wmdiyhrx.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3amjbwtey.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nirxveqz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3avmyxpwb.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3nrwcxgrq.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3wtgzufxk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3hkfhkpma.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3wffimvuo.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3akwmvxgb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oosgbtpo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3mdyvxtbj.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hdtxzbkn.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3zbtcithf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3npcrlopz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3xwmnhbjd.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3neskbgaa.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3hgcpjycv.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3pzideylv.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3lmpxhkmm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3pfwszupo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3epsxhdki.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3zltqluvw.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3vzgzmhxj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3nefzpvey.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3xqtgldsz.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3fybgciry.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rxaijqyk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3vnnnhkla.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rsiilske.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3bvphwmtn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3egwqaiap.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3mmbguvie.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jazbkwih.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vrbburgm.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3epesqorn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3cxijgyfp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnqiwgew.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3rcgvhexk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3aadcsjwh.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ibtwvist.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3unkpscpv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3clulecwx.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3bylzshjo.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vohctuty.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3syexvkur.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3blruvpxs.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ihzvuwth.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ibetnfvu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3oxovxrpp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cyvwgkae.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkiatwxk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ilosucjn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3tutgwryp.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3eifvthgi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3cpocvhvn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3tkarxggq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vqqdsqfu.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3tqeiskqm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3uibgahes.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lylszeah.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3okdwbdij.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3pvnrtfku.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fwzlozod.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3djlryvqe.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3zjxptanq.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hbnfwvrm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3blrofvdr.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3herxsxmt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3osrbsibm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3ycbpwety.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yrdqadew.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3qeuxpyty.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3iklelxdc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3jxqtmfql.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3lxjtwrhg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3rjgwelhw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3znwmiccc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3ghhzcsrr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3smdhrafp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lgxxtrxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zizdlbsb.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3dcoioigh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3degqoguo.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3dstsnrfx.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3ybofqidf.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsyabcov.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rftaoqdm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3hhwpyddg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3losxvcnt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3gzkmegqp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3avgblvge.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gbqvrhcp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3zxuzsiuh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3ymtqzder.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3tlidbrhm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jzgsduur.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xyovhewm.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3atckuxha.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3fljckbgf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3mkkbzczh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lbucgkgg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3hsfahqft.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ftarwnxz.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzmmmwgc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3aqxoutmg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3feybxmsc.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dmnvvspw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3yudwgysg.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3tcneauyc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3gesyszxs.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3cwhueydb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3knqcmbtr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3owwuaohu.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dmeooiao.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3anxczdnr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3fmbpesjo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3qmvtkpwd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mbwsmetq.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ygayisgs.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3stwyksxq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3efyyufoe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzxloabl.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oluwudrs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iirdrjzi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fcmkwwbk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3sinfbyrq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ntrxvtcs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jluxkewk.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3pmpqvslz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3seiuyttn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3clqqehxw.html


<!-- 参考信息 -->