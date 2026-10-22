代发 wailian999

J. 日期与时间                  （第 10 节，10 个任务，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt2mytijghw.html

K. JSON 与序列化               （第 11 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2arzluwrp.html

L. 网络请求                    （第 12 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2pjxpjora.html

M. 命令行 / 进程 / 环境        （第 13 节，8 个任务，64 条）
来源：http://www.52xcode.cn/Article/details/gt2wafmkohx.html

N. 数据结构与算法              （第 14 节，12 个任务，96 条）
来源：http://www.52xcode.cn/Article/details/gt2lffkiuyz.html

O. 并发与异步                  （第 15 节，6 个任务，48 条）
来源：http://www.52xcode.cn/Article/details/gt2mgqqxaof.html

P. 常用工具函数                （第 16 节，8 个任务，64 条）
来源：http://www.ydjk.org.cn/Article/details/gt2hujbrnuk.html

Q. SQL 专题                    （第 17 节，90 条）
来源：http://www.52xcode.cn/Article/details/gt2byhlxsoy.html

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2tayjebsg.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kwdqghgq.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2wklwdsdh.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2zgbhqbxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ckhehukc.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2yaqqexvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fxjumfkd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2spzjiujk.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2lzzeyedg.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt2vxwflijw.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2ukaksbyv.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt2avtjindh.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2hebcbbcl.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2mqiaflbu.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2ntztzcho.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2omgnafec.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2ojuvyoqx.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2uyvigksu.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2xgahchtf.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2lknmrzdw.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2dagmgafn.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2rudmgfce.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ymuuxtux.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2lktechro.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2qekylxyi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2tskpotom.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2qxbhvhir.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2evlonfnd.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ddibuhom.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lndlobva.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zfrlefmk.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mtetqcdq.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2ajlybrmw.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2xfhdifrv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2awovviyy.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2yyylyzvq.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2xadtuztt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2ofkvnlgy.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2zkttupto.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2fxilexsh.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2pfsofwpz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2ciczsihq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2esjkjgnq.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2aciwzxmw.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2ujjyccmh.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zjpuylcq.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ewpsiuhz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2aumlorxn.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rczogdfn.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bwbhqprc.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2utzshgsy.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ubdzsfwz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2qvjdooys.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2qxhmarhu.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2oithkppp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2klwxoaty.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2fpdbywyt.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ptqrabix.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2esbswfrd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2rtzizbia.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2blhwgvck.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2stdtbdcw.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2uujmphdc.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2hnfyimre.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gfvkoguz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2tbrelgsv.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2yekouiin.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2vvzxatxq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2pvydgbme.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2yykoxocc.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2qmktzwin.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2lowbbsvx.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2zszfqojs.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uwizbbjq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2gawwulol.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ibbtmarb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2iswxueqo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2yjlxcejh.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2utawally.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2sdwdrzuk.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uezywkex.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pkdlcjif.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vhppgxed.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2yyjtkabg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2imcryrtl.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2kzdtekln.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2cougwaba.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2twwqqkjf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2pluukjke.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ojonezhm.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2phhfvgfc.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ehsxaalk.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2sgsyrkxb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ydlfiuhf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2rieyquln.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2gaiyksfs.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2ivekbeqk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2iabideaf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2qoovgama.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dpwlldvf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tanuvszl.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wgkrfeds.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2mmifplag.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2xcntuuke.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2sujnaucm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2jqftqlgg.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2grmlsrab.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2plbmnxdn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2kicspltb.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2swfbqdlw.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kfdtqrgj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vpfoztua.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2karzkwnv.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jgehobjt.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2kuvijbor.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2vhdpnwmn.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tldrudwb.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wregeerd.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2icfekfgl.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2igjjsadh.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2pvptglxg.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2odnghwhs.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pgcxfwir.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sakywuya.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2wqdjoebr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2bdjrjofk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2meehgrbl.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wmvdagrz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uczmcdpa.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2bifryycn.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lcrxiiaq.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2mtsxobcw.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zggehdgq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2crwozbsl.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ogqmkuos.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2yotjtejs.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xyzwqwsb.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2daqjrzmg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2jklpodqd.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2ibeuzwtn.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2jgfbomby.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2smtzlvzv.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2uhvbfzgk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2rjupgast.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cazaywmj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2mmobchfa.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2scubicgp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2gudbgoad.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2eptzboya.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2sqosodax.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpgjevri.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2chmyujaw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lsyqcqzf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jriiptiz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bgjkjwfr.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fivfgaev.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xgezltpr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2aljqdsjo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2izlkekuy.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uvavpxle.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2lnrlewwl.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2rdlcphjo.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bxdojvih.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2pyoqkugs.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2lvydnqht.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2mphhwgry.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ryytfjgt.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2byhvurvo.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2azblgomc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2fvfsaboy.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ysrwyagn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2yejpglmt.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tvfwrvcd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2kcitgxbh.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2dcdjcble.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dugxyqxw.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cwrjdgvx.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2pwrxdhfe.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2qiqwonon.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2pzmaequh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2eweznueb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2wxrsbltr.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jslftkaq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2vdvqyseo.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2digebkid.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2iypxhads.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2qkszrcqg.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2rjgipxbb.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2wkkwgofn.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ifbhvgel.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2qdxvbwjm.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zgzuhwil.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2omvcyzzw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cynhwypo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bqcickoh.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2encalwdc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rqnrwjoy.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2mccuordr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2mmjjpgsz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2klaxrkll.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2fiiivdrr.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2lnfzzhih.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xkncukag.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vbafejnu.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2pyruonnl.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ghnxnfdz.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gqjkdnmn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ajddiwvw.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2frllnzpi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2fsnopjtz.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qiacfgeq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xczgxqhp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jpwofcxv.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2rurhxuoo.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2tlgfgohm.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2qztkyjwb.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2cvxwizaj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ohwlwgeo.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wmlnphvm.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2sottjipg.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bncgzgjw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2zbqpwlac.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ucdqfcqf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gwwsbhyw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2xbxbgqps.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2whktfeci.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2kuosgyda.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zssrmfcj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ywrwlepq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2kshhxwfm.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2nwobfjac.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mouxaijw.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2azknnvue.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2vykrjczx.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2doiymysz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2fzkdfzjj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2kjvrxlrr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2jfppnjvk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2cvkemnyv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2khwrpijm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2ioljotup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbveyqif.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2nrsxywoa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyedodxo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2qgfdkosw.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2bsqimprc.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2irherwpm.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cvqyydvd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pdezcksf.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2agcpjwpw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2gxfmjhik.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2iaulicwd.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zrhlqrzv.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vohrrlvn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2pudtotnq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2mmstkcxn.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ornyjinh.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2hxsahwpa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lftoxjpx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zjjjtcvn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2kasroijx.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kvemozkf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2dkmycrnn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2gjhmyyrw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2aotdbnal.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kojnduue.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ahkonzdp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cnyvtipi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2khijblkx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xiptqbch.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wctuvtua.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wjoisjlw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rfmxaxib.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2ynhskkns.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2libtskwa.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnjojrww.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhvefinj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2dzugzunk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2eykvhtug.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nqixffpa.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wsyufhak.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zcukhlib.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2oaxjlxcv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dyyrecwf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ipqiqsco.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2qaybtbtz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ugxqvuiu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xnjvndvx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ngxjvntd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2bjtsimaq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2vdaifipq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmktsmqt.html


<!-- 参考信息 -->