代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3xyaaolxq.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3vriiisqm.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3dydqnqft.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3wrotleia.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3gjjbwfjb.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vwiuhtcw.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3lorakjir.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3lixeymne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ussblxjf.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3hfoxnyuk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjnkduri.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3odeyeejh.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3qtfklxkj.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3hkrwtpuq.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3mqbqqwra.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3qsafnlun.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3bgkqcubl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3tyeyymdy.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3qcabadbw.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gxppcjje.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3sqeajxeq.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3mopsippk.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3zykzximo.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3yuxdvkpi.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nqylutjr.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3uvxqnnvh.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3qwnanael.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3dkdwjtsd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cndngpxt.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3rwqmagoo.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3towcyeyc.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uxvlqilp.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bpnugwgr.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3opiuppbc.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3njqjrsbm.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vdkomzdq.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vrymdhlk.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cvqnyoji.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vuzzpcde.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3flxchmvk.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3bubdsoqw.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3cvhtjwfv.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3uiktkjzb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3ybgrmjaf.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ofxzztgd.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3hmzojkhl.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3fckpgdta.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3tomgadkp.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3zmjxibnt.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lwvaqolv.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3odxzzifm.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3tbmbcbjw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3fswkogdj.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hzhwadts.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wgxgxacg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3tiarekmx.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3geihzvab.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3txmjzbhw.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3izmrbezd.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rzxncfur.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3rgxguyzm.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3swlyawyg.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3bsjhkrnz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3dukazund.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3xxumcdii.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3vajmxemi.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3sybzbmvl.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3feuhrnqd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3vvqjtthf.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3zbfronbq.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3lelitrkd.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3fmcoqeil.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3elokiumw.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3hzixloza.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3smbzbfiy.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kgxkdtub.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3etlevwyn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3pfnukurg.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3iapbnwoj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lpzufqqu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qdxxvhmw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3wadrspms.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3oqsvgisp.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3wylmysmh.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cosbnkjl.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbwoxazz.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3eadcsmyo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rsrznihg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3onzdimvs.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3pcyfutyb.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3onyycldh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ktifqsmy.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3kuekmbqb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3doeawpjx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3pivibtve.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3btzrxjdx.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3sjghcimw.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3wcmezxwp.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3vpfkobbl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3quuzddxt.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3kcjefrsv.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3ukdlgyin.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3dekxvwlg.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ndlegwsh.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lxxtnuzj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bkkjwerl.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oidmirow.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3lqrraati.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hmgzzgkb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3icgcyhir.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rfbdspqh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3fqkedukm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3tithpfsv.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3slokxpix.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fncwnhtb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ywhcmmnv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3hcnfesji.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3hiuzupwx.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ofmafhay.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3xbxmyshw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kpmtzgnt.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3tiprxvvf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bpwnsegf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dniorwct.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rrhqpgca.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mzthgcgp.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kftkezfk.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3yotxkjug.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3gbuzqmdf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ymolsocd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3srhwbxkc.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ldzxyhyp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jwwlsicd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3sdxclyvp.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3kagfumbc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ixocxuit.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kspnduim.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3pgyckylw.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3wsoubrey.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ozjmlnfo.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qzpbpdft.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3yrmngwzb.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3dvakaacm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3nzhyjyns.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3tfxjokws.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3jnxbezsn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3mvfewnuw.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3uazntykf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3ytmhjsun.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3solpnxkn.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbquzxev.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oizhglwj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3nckemafo.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ftrrbplv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3rowvrlee.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3mupgcpmi.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wajmtqdv.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nxvnxpek.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xnxkkkgu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3geaticoz.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fbdzrhmd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tcjlkupt.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dqjrnhxa.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xrikhkwl.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ilczcrnw.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3harysoiy.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3owjzfpfr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3eyytomil.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3bjcijmym.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3vqwrifdi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3huhlzutw.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3bdsyhprb.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3efihilwp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3stkuaask.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xnaapsni.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3jllftsxr.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3glljtdlp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ruuynfwl.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3xndptacr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3rnjiuylm.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3gkghncbl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ixcuimku.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3awmwsbzd.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3sshgwyws.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3tqdvaaqo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3wvfhmxag.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3csqlaxqx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3kmbbsrla.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ggfxkadz.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3xqrwiyzk.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3kafgwxfa.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3tvzrfgxu.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3jhlzyqqg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3erpwslre.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3idtxknhu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3lucistft.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ddljjney.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3thuonivn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3edijmnfq.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3lqjcfyhc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lbhwztxi.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3tybvdrja.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3tgifvtsp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ulzgadms.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3cucjoojx.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3iqsnysap.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3rwmqmlns.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3oxhfpapg.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lgidfkhv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vacsvadq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3abvqfmbc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3bylyetmy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mxvxnjgs.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3vimctbzt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3mngklefi.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3gwflgngx.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3whfjtxtj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3fwzyqvzp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3nwqnhawt.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3rxidgfki.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3zjoizloa.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3hqhimmrj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3npiavlde.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3prhbyutn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrdqjrep.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3vfmqlmoi.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3uojvsysn.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bbnktrku.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3koyugmmq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgxvscbw.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3hmahgile.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qkigcoes.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iqkggodx.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ozcdsqht.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3lapvdhpp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xljqhbfv.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3joneghcb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3hmvbqlhv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3ehwgghyz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3oxtwznbs.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3blbgsqqo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zhsvkarf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3hjrkstxr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3oofmrabk.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3aweawllw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrmxieao.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3luwmntfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pktrxfcj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3huayuexq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3rofmukge.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3igltmznu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fpjhzozz.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rfycwyuc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dcwavitq.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3rysnuxsf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3sjbhjbjw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3iyhcqbgr.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3kctkyjps.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3vihpmsbz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3iyxnejcm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ofnrbhnr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3imvssmpi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ebtoyvkm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3solihoqi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jexedwpw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lisxozdu.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3nwrsvauf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3tydnaeak.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vaimapau.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhvphfwd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zxtmdvag.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tdlfeggm.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3gjbtqgus.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3pxnngtlx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yzkckwoo.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ynnbdzpm.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3kljzjyco.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ojqqvsdz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hvmbtcec.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysurlpem.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3agscmecm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3hchtrgjy.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3qshzbptt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypkcfmoq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3qqagciju.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qhvavdzh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzptrari.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rmtawdkv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfzlxbxb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3uwmiijef.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3mxexzkoy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ppqxgtnr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3rzhkvtah.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3cekohooa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zxstvrdz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eciojrwv.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jijqfpjo.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3orslxrvh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3jabwgzhn.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3tcrxmjxl.html


<!-- 参考信息 -->