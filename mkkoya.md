代发 wailian999

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.ydjk.org.cn/Article/details/gt3ijhkuzae.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.ydjk.org.cn/Article/details/gt3widfgupx.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt3tluicxol.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt3biqimbps.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3drivwman.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3bitssakf.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3cvkqjrea.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3kgyinuto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uuivnorj.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3zixcybgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3phynebqu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kfrjuiha.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3cinpqhjs.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3rmcvytjf.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3qxqmqxpz.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3xutagkra.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3gcmftlcm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3rtrlebsh.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3gshzikoz.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3bdkjcegr.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3uizwqaka.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3mcsdklqw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3zpheiled.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3bgkpsuxs.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3qhfwqzue.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3mqmwkxgk.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3zdnetayl.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3zxapqhlw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3cwmpyndi.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3qpjxxlip.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3irjnuluk.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hcwgguqa.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3rrhxulyx.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3przctggn.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3yhgppume.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3njmlhagv.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3hnedbuel.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3isxljeoe.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3hakrchjv.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3esrzhuho.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3dkuwmobq.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3vuxmxwtg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3muznbqzb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3hqqwfgsw.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3pjecdwea.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3amhodccy.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3begrtnjw.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3xfuxpkpo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3tnwhnddy.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3oramlkmg.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3syhpoorp.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3brycqwuw.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3mhevtuys.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3gtzksygw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lxmdigkp.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3auyguyif.html

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3jjgsoxbq.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3whjvxeyg.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3aklbnrxl.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3gopprxdn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3pwnxphkl.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3woqfhezx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ljoeibst.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3pvulioga.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3ewevhple.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3kmkfnety.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xuorlmsk.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3lklcfyox.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3jeqystrp.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hepklwhs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vspzciqo.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3qymjtczb.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3ocsivcch.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3pjpcsyfp.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3rmuwgyej.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tcyhoycb.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3itdwsvrv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3snpyovuw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3fwxcjwxa.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3llvrkquu.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tghuoceu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3rggpitgi.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3gurgnjen.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3rqmfoidf.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pmnhcpor.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oivlwttp.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgihddkq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tzonjogx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3frdroskj.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3uigwzvou.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3qoxxesos.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lsybycyh.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ivykitvz.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3iuayvldm.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3fcshnhkw.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qzkdrekd.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3kihxabeg.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3oapqssmd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3rnlbxnhn.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3vcfbngtu.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3xljvqcbs.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3fnnwjwyw.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pjprjgbh.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mzkdgxps.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mhbngamq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ihqzfzaa.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cgwbhzjr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wwwdxpgs.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3hsjpmsai.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vmfpjwhy.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3eoalqqgs.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3zwnsqier.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3convsscp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xhzyevum.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kxxkgjfz.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ldygfuck.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3beyqssws.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3cwmblgzs.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3lbtwqwyj.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3hdfwkinf.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ikfvigbj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3skhgxgux.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ytxtpkmr.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ijettdmj.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3hdxohxhe.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3adgyczna.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nwyzaigt.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fqltaqye.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3zikgwirz.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3xyzgfbhh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uzvzlxbt.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3mhvwyjkp.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ischvdso.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3soffynpr.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3ecsejnnf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3dfhgiira.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kueafvho.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3anagkvfz.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3hjkkshib.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3cjhnppjg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3saonffkv.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ivcydamc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3bwhxjxpq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3hbgijzvk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3iowtrxnn.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vtozckdu.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3sykwfigm.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wnpiqnve.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3xwbxptbf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3syvovhqf.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xngatcma.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwjmbqjw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3xqfvnshp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3kbmayjal.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ptnbgbiu.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3jonjdgca.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3njdodjfi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rshaikov.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xrggbfhy.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zlnaspiv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3wiqvtkse.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mcfqhzlp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vupqdeaw.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mgjomowg.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3ksyhdckt.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3zepmciya.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3itfoedgk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3discbqxz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3sdgpontf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3cjkfieuw.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3zeazuwil.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3dyusjadw.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3srrqomvk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3lqekdkiv.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lavtfren.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3nudcflvi.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3aabxdxne.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ukitadko.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3iwklhyee.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mbfurqwo.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3zbdhsewv.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3zhohfiaj.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3zbjfnwcy.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3vdrnenfh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3evawkcaz.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3xfppraan.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3vsniahju.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3eihadutp.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3bdkuctph.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3bgvqmffv.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3kxmnjids.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3qvauvjtk.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3ykzhuqob.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3weksrvvq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mawtaqap.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3zkcsaudr.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ammxoymx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3oupempwe.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vjuhfexo.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3pcarmxni.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3jyznhobd.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3oifawlqu.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3jvcxcahm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3awzfsffu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ltdffniz.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3rjknpjpv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3egihexvu.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3esmdxkpm.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3nnejadkk.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xdxnjmwm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3vvrwfqup.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3sunmxfrn.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3orupvyvw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3itqdnzcj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ejvcuaxy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3oxmzripu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yrhunxed.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3qfejmvig.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3jpoqoktx.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3gyliuysz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3lcislmoq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3unexwjfb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3aekmcpeu.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3ronrjvxp.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ksgbuvnq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3oohoilgq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nrwrejmx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cjbufbyz.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3pnrinset.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lfvszljt.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nxyjepdu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wowiqkdx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kulvhmah.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3fyysfxok.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3mwuautoh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqczjevs.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3xvrvegim.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3vjmeuuen.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3pchbkebe.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ymazftxx.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3vvpamtgv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3bkfnjntr.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xazwmnoy.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3skxktddr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3irzpgwdp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yegyzyan.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3kpmaacjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jqjaeuuc.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3vqjutnbj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3cppzccst.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3jbfzzcwk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ykhauqbx.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3lfxnczgx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zavjxzvs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3sfxnafgx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3aotfqnog.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gqdmdbjq.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hpdwwsni.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3sjbolfwg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikkxftng.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rcfhrdfc.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nsdnhkgv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3egbkuewj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3edcvgoyd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3mxbgdavl.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3odjeygyb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3sxirjeqj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3pwvxejlo.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlrttitr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tnojcuwz.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3nlsbvhdu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojpymnrd.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vfdizvaf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3wvczfbum.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3soaakkhh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qwqkprwc.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3emnjjnlg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnkolfnf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ooonnezl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3hrqltndx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jquqanxx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3qhlylnjs.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ibzbxqst.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tskdpngb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mpbfhbxm.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3hnshbxva.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3xzotxpwz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ojudvnkw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmshcyjl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3sosfpldp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3qkwqzuxl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3lynwikrj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3uhcdtjdc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tsowthlg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3mkcalndi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3ptrzpboh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3anizpymg.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbhpnzed.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjxuyyfh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3gvzbyjoc.html


<!-- 参考信息 -->