代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.52xcode.cn/Article/details/gt2qwalhgew.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.ydjk.org.cn/Article/details/gt2kjztwioy.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2rpehvbgs.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2lvzhagxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2diffuano.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt2siqmotxy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vusclwao.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt2qogiwwdk.html

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2wtrjtauy.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt2ddcantcv.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt2kmwcyaog.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.52xcode.cn/Article/details/gt2llujdsgc.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2tlyyeouc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt2duvgjsyw.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt2fuztakkr.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2kvwdzlkq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2qpcgxkgp.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2xpdlptjd.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2phgaatis.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2pkuiycug.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2niudeqid.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2hpsogksx.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2ucwdqcoy.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2vnnbfnts.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mqxfnkoy.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2jwismsrh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2jduzpxik.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ojxeyjch.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dzfppinx.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ecmsucey.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2oagtjjbg.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2hjjkfhas.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2asnxuyyg.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2pkwljhmg.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2mtgeifzq.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2lbiwravj.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2iqzprbjo.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2wkrgcnth.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2vinwqzzt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2dmdzdetj.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2lstdhosb.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2vsansjnq.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2joxscgot.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2lbcrxpcr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2gyvidjbf.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2fxxvdaxn.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2blzrqtbx.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2etvrqist.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jouwvpqv.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2aeptqeqm.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tlixiomg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2sgwulurq.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ejxutqjm.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2cmawjbld.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2myjswtvp.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2elxtvpol.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ydifbwdx.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ininbvlw.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2bbdzzpjc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2hwvwsphv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2tzvliwum.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ymlobaxe.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2knwwbuqo.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2imcjtkbh.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2lhabjvue.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2evlcwoie.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2muybgsmt.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eqrvmzdv.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2zdchgxwz.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2oxqjwykx.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2mccfbste.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gjuqlggv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2irleupkn.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2cyfgoosd.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2czalunxn.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ttlcmvyy.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2viefnrdv.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2grckcyhv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2wxhwfxce.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hxhkoybm.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2kthbxelr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rftijnrs.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2uuzasmsi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2efncenul.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovzrdoxk.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2npbasqqj.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2mmybvyut.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpqmkaqf.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2tojmksgg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2wrsiovbx.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2zgiridme.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2jyxqdefe.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2fntvwaom.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2hbmjriyf.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2iakatpic.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2jnszduir.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2kqbcxxbf.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2qbhcfmqv.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2sbvttlik.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ogzqyplm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2bqzrvcyq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2beeqjeuu.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2quggvebc.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2nigvuirc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2veyozdjp.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yffopbyg.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2donetrnm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2jyotqnbs.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ntkmrhwq.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2prbuheba.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hteqfmrd.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2semzyhls.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wkcyyorh.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2halyeumq.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2juonipaw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2epneusbv.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yfkybdon.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fxiitzwk.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2imlqznnn.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tnuslwau.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yajvutzh.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2rkzviaar.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cidvcrbr.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jiqkyknb.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2sozkdbof.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2pxxpjqhh.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wysmwkds.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uofsqmnb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dxoyrwdh.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2lknqsizm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pareylna.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2lilnphap.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kpbnwphi.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2pejxixas.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lmbahuqn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2sqsrozad.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jnqlccib.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2eydoscpm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2kcrqlghc.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2gfbfomvk.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2rbpvkepa.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2luffsysa.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2umbzmnzp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2evpucioy.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2eqcnaoyc.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2nrpxutoh.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohclxigt.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rrilogvb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2tmyefhri.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2xdnyawnu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nlmekcxq.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2hjverqrl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ozfipipj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cchidvzd.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2olfklgmt.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zauqdoor.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gztaiyvf.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oxbkpbvg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rywlfajg.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xqiwjfoc.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2foibhqpz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ufqbyidn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2oqzuisvr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2saakytif.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2oamagmlb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2pmztqwiz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2dzqsvdou.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2hhtlnshh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2jpvxbfwp.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2mxridzma.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2mgiuvmcz.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2crtikfwn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2akwxdihy.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2wseecwpb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2ujemukyc.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2stqrckuc.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2lnvqvryi.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2bwbsntqv.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2uudyslwi.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2vrigigby.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2houcoxxn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2xkipzkuq.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2quvylwaf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2mobwsayc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2dfnmdcso.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2fneztotd.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2iyksytaf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2egojxtny.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2jvkacbxx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqhsjyr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lpldswtx.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vowtmcni.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2egnlxzxy.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jpomzlrp.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tmmtfsbw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2nrbzjrzc.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2kgecggjo.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mmpmqhzm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2nwcxbaaj.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2tanfcpkm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2biixhslb.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2zakbfcze.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2imfidywp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2bpxpfcmp.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2gbkusgoe.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cvbiitrb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tlqupxhu.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2dapoxzlb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pvsovbip.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2irerxqig.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qonttasd.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wfuxmpxf.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2trtkcvnd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2zrepnumu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2sekvsyvy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2hrbntsrn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2lmxkttqp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2sbojeryt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lnmcslsv.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2offtbqpc.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2witzescy.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2vhgbpgez.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tebbwpyh.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ytejabsj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2iubzwzlt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2kbmswcmn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2capkserx.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2frzmppgt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2gvlrcarr.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2feecjrtp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2mtslteht.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2xdmjxdoc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2uqijqfsj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2bjgjbpsl.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ckeothby.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2kkhcyhdm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2txjsogfn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ntjgaxup.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jamsdmuu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gkqtjllc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2werddxtr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yczzmxyh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2eeiguitr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dsuvjczr.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rlltkpve.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2begsourx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vhllmudz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wqsbulvj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bovjlbpx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kznvkqlx.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2gabyagym.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2pxyuktcs.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2pwgyuxsd.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2nyerwkjz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2cxpwkcqu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otdstjpw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vuqtwrad.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oxrateos.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2biddmhtn.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2spawmxgu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2kifqqxhk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bkbyxexq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2qcvcnrvs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2hiaiwosq.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ceoejnnw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fsfgqtyy.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2klmdbokg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2wxcqylfv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2kdzvgiji.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ozodpfmi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2cmwxyyup.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ogugtxfn.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2vrritihs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2pksfvkiw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2svjzbjgy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2chrsehwo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2okyjqjpe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2lqjyerne.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ipqbamfc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hzhmhtwa.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dcoblgaz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2latiqotm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwbuupqn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2dnbxbubs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2papfdghq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wjnhvcfh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2hjoundyu.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2yzogmrqg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cviyovua.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2zpqgfixh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ihkgpuqu.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2kimutlqh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ssnqpvdh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2yihidjoi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2dotnqmrd.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2fgljdzyt.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hnabbxnp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lbjglbvh.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2lndmapdd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ilqycsmp.html


<!-- 参考信息 -->