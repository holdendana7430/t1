代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.52xcode.cn/Article/details/gt3tcvyhpqx.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3txrpzrgt.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3egtwfkgj.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3vkndejig.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt3velffxyg.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt3pylxzbbi.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lvxbgnnq.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.ydjk.org.cn/Article/details/gt3hccvpyqv.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt3ulogwpad.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt3coihpyzh.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3ebmzqpfo.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3fcxxouoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3keivvmip.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3rymbsbfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdvcobxu.html

[A01] Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3uqmttrzt.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3lwcsintc.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3lkszjnhs.html

JS:   console.log("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3lwdqrdvm.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt3qqekkxlq.html

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3tvwgmlsr.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3dvkvuibt.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3rhvpgvon.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3sdnvgndo.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3musehjob.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3fkjpicsg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3hmqxjxsn.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ddmbisvk.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3gwmwmedc.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3nolxjcme.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3knwzhcwo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3tcxklclg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3qhnpeitz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3xiqzulet.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3veqbwzbb.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gfsgyhuv.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3gqkzpbkl.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jweaihue.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3iaboowon.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3nsssrovc.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3wzdqnkgl.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3syyaozwx.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3lukrtina.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3qpsjdfnt.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3jfjstpsj.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3ptenzrii.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3dmwmcgdb.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3chjiebbm.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3hglslmgg.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3vxtfojij.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3awutrllj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3vioxuilx.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3hemnynrn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nrfjurih.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zrnuvjct.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3elzdjidf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3xildsqvd.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3wxjveyme.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3lykhpdco.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3lpimcmqy.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rxpqzurx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3fukownjl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3aukrgtia.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3iiundgvv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3xvnbndzg.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3xuxpxxjj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3avnadtfk.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3ymkdfnvo.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3wvbtftek.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qaqtqwkf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3lkewljgn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3uiojitgy.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3habumnff.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3ctkptszz.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3razwhvvu.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3ilbqgxxq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3sgywpzhg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3tellhdox.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3lsyqggej.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uevodwen.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3dlxnkusw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3tkdupcho.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3cmqdcebz.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3vcncwsck.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mhkdxvfm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3rlgiouou.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3tlsfxafh.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bmirqgel.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oyzongjf.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3kdtbmsha.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ymnerqnr.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3idmugnnj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3wowjhvrq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3mufviwii.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3olbxhaac.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3aajaqzsu.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3hfkeaekw.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3qwzwwcla.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3lybeephp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lrxizggj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3vsfqkuws.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3lmiavrlu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3zmxkcltd.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3mfyyaoei.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3jfzddwba.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3laqxmgua.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3afjzepmo.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ukaiqubr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3kleorvth.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ugbrngjc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3yxxkheml.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3dtocxjfs.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3svnnsmis.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dlnqagnb.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3itazsose.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3auukpbti.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3roiskesp.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kixbthgs.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3tqaffvtg.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hvjwxpyy.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3zihyoudh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ttveayco.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wplsmyyr.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3hottpith.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3iixeresj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vmkbktid.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uugmdjmz.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dihjzthy.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3dnehsmkw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3pkgiwifs.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3oxleufik.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3wgiajowy.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3vdmvdgvi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3wrazzbvu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mviqpenn.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lorxbaag.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3uqwmbgoe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3dcfcoout.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gfupmour.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3sreybklf.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3snilpcog.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mhbysdzo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3etqzamkl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3fcbyqfjj.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3dplgfvzk.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3laztzegl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3zusldgon.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3oxayrbfd.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3nanuzaaa.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3cyonsgsg.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3xmbwsudc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3huodpdmf.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3osmzspoq.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3urdqczbl.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sydrzndc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3dexzukhw.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3ylgsrxro.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3rnsqmcbc.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uacabjxu.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3kesqvgkf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3oujdwuxh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uwzhnghe.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kbtqlijd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hlmgrdjt.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ltwkklbt.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ummioxiu.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lqnvhckx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rewlkxuv.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3gttwovnn.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zllzsfus.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xcpabbjb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wizawhgf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3fnzjzvwb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3hrimblqi.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3mtebcljk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3xktsafdn.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3bvnxgdda.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3yvvxqege.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3ncjliqei.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3zumzbjti.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3nvpgfzrm.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3orgkixlp.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3rwiskqhn.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3kvkluvxu.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3cnhdhqap.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3pqoctvrk.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3gznfvlgq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3qfwatqnf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3aivqpfar.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3eqboyzek.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3xvelwrtf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3hqyvwtrz.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3jbicdiai.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3iwkgpxan.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3mngpgzev.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3mgqptqon.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3nozhhviq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3obmtjpgy.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vmiyrfux.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3fwvwotms.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xyaqoxtv.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqwpsrq.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ijepxkzz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3ykwiyggm.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rbvuwkuy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kzbxbhlb.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3wrhomxah.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3yctaygss.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dimrvncv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fbveaixq.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3uwydzqxl.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3mgqxgfww.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3pihfbamw.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tpnkblzj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ipwejkyv.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3wwkqchdj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ifwzrary.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ntlnlzrm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3dkhzxbvs.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3iveepmex.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ljuroxgk.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3wehpivhh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3ukbevuan.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3lyapmigf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dysfwwrc.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uqfyslvn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3smdihgxy.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3ngcqctoz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3irwrvgup.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3gjelhjyk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3axrqvlzt.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3txldewmc.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3uavnsqkm.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3wycbfjsn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3amotsrkf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3vvbjnsoz.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3abmpfpei.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3crjfjpsx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3cxnswtwg.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3hemeeemq.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3nctlbycc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3mpaeydhc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3ufjycsnq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3ydytzfps.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3iuxkweym.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vafksrdk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3tuxghqtw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nmcdqdpf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3yysgvweu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ayzdvvwk.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3vhdnvkrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mncwznvi.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3eskjtbei.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3bbuezkuw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpisorip.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dynmzwvo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fbdvztsd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rmnqajqx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3jgtnjhiz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3sfuhyacg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3zxmqeval.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3ikahbnmk.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3yeispxmq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tylkndwj.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3fhofedcz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ffqpjnfr.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3cxpkyycq.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3zozmlbsr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3eeknbdie.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3tibamgve.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3zezerose.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3ldncqxre.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xlrtbjgr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eiurywcn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dhsjvzyg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ivnaooet.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3hneiecyr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3dqrywkfv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ihqslnnh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ibnpcsjb.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3hjwghgca.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3qkkypinm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qhregnos.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ewozuabn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vkecsfzx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3aqiztqco.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ujgldcrp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3rxnjqfsp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3nbtvxayx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3vpjfkjzx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3idbcgqmj.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqoypxoy.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jaqrbyhl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3pgotabdp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3cqnwqmey.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3zjhpxvfy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3vzxqnbzt.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3rstwoptz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3jiqidgte.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3vmnjactr.html


<!-- 参考信息 -->