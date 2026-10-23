代发 wailian999

R. Bash 专题                   （第 18 节，80 条）
来源：http://www.ydjk.org.cn/Article/details/gt3pesdrkem.html

S. C / C++ 专题                （第 19 节，60 条）
来源：http://www.52xcode.cn/Article/details/gt3rnwpaaib.html

T. 其他语言补充                （第 20 节，60 条：Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hctszmmx.html

U. 高频实用片段                （第 21 节，120 条：Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt3ejugtrvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3opoxmgxa.html

A. 基础语法与类型
来源：http://www.52xcode.cn/Article/details/gt3ktfbeisl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qucymhjd.html

[A01] Hello World
来源：http://www.52xcode.cn/Article/details/gt3lchytsmu.html

Py:   print("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3jfebridn.html

PHP:  echo "Hello, World!";
来源：http://www.52xcode.cn/Article/details/gt3esdxuxiw.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3qfjgqajk.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3qercrzwo.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3zxhuwyfm.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3vkavfjok.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3khzxvwhd.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ahwytqzu.html

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt3pqfggwtc.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3iexdxurf.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3jradjdam.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ozprnwez.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qutktimm.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3xemhjqem.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3yflvsggv.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3orufbigt.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3uehrziiv.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3yfkhoxoa.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3ajexiqva.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3feqiteub.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dtlxucdt.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jmbkldlw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ekwptoqf.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3smngpuqb.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3iauiaelk.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3twumphbl.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3etbzlylt.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3stowwdqh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rvoxbhsk.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3lhihovjb.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3xqjwiqow.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3nyyaxftz.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3zawkfrom.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3zhtpqnrw.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3klhpusyl.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3fckzwalr.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3rwenxawn.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3spvuqdyf.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3opdfboij.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vgixozby.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nmpfzitq.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3nkrnofhp.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3eovgyrhu.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ytpklihj.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3xosxtzby.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3aillmztd.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3bxpivhlj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3beevabnd.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3fcovfawy.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3pwircjvh.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3rpkhscuh.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3sqyxwknf.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3vtrnyuxa.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ilakrudg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vmxbqzqo.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sinnhtoa.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3tlaocvuv.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3iwdatdap.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3tzeqhkvg.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3dgvkmrjq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3ajhovjai.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3mpxdjaun.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3tpomacvf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nkrdemvn.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3gzatwsfp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3lcuauech.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3zpjzageo.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uxbftmcn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3kvfcawlm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3sdtevupl.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qrfvnuzy.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ojfgkvsr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3umkoofzd.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nuzaojpf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3iqqlkgow.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3txmxphvc.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zartltgr.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3lgfwveui.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3jdyuluqb.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3zbiyfoqc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3wdwbvtdl.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3pmbhenpa.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3uqewxypj.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jjfzbtwj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dxtvhija.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3galucjzu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3skgzsmoc.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3lwsckloi.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3nzvsasuk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3pyluzckd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3apcqvrln.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qdymzyez.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ovnezbca.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vbitopjn.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ftudnqkm.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3zzxnmdod.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3cgwgntea.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qfdnbujm.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ogygccnp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3qvbksxag.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ivntmwuo.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jlepsyez.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3eduzosth.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3fnoswdnf.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3rnpapvsv.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3bdqfzbij.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3qakddzbk.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3ktyvbmqc.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ledwzish.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kzyuhcnn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nwftmpcf.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3khieysxo.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gbrcqsen.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jtdcautm.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jwkoedkq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vhwcrhcl.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3kyeckzvh.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3mekjqwcz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3oqulxmjw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ssfuvwje.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3onqitlla.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3irmzctxm.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3stahephf.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3iaypmkfy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3wcoygden.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3dvyogzfu.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3jyyickmc.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3obulypmx.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3ynitusbo.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3maqmytlq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3onbaruta.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3vwadfhta.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3bmnzmjmf.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3nsotkgeq.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3gdwianpe.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3uppeqnmw.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3jxgceeaj.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3qdrqfbsi.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3susfrcqz.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3ffzfcrcg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3uxrjelhm.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3guuuwweu.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3chtsztrp.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3diuypydg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yhliptta.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3olbvlzuh.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3xvzdqizz.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fuxlqpua.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3simhajpe.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pmvuocfi.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ptdmppww.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ggmvafyu.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3jeecbpwf.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3enblqzzt.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3avdnpzhq.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3cddpljlg.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3izmjjirg.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3xfjqojpr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3wxzwcxzu.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3alykyxjs.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3shpbsijw.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3dqyodsrx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3oyjkmaog.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3hgvfbrzv.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3qejwviph.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3nramkgzc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3iglyjire.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3stftdryo.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xdvtmbfd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3aextlery.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3cgoopvgl.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3hcbjxqrc.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3lmynarcb.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3oajpwyjw.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3sbmsicic.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3wddiajrj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3wsruhjxw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3rcolrdtj.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3akjizzpf.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3fenktlfk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3aascijos.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3updxejuc.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lliuyfwz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3huoupfzd.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3amrzqayf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3hlypwziv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3efvisfdu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3kielemxi.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ifajhqox.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3zytapfbi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3vfirhmoz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3ekiqulco.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3zwxyadpy.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pvpgmngn.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dprhzqng.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3kthulwbt.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3feojtqjn.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cfykzhhl.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3quoxmzvl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3tfusjxcm.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3qsrmdjhg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3puzhjbrb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zcwpjogf.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3palkptnl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3nsogbabu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3azgdptbe.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3tftqkvia.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3lwcftoby.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3qjjxhlsq.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dzxpreow.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3vcfboasp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3imfqyrmn.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3czkbrjos.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3zuqcanka.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3bsqjiedx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3yqjwmsvg.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3onwxmhyd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3hazpdwlv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3smflpxam.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3uqmpetfa.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ujxhuejz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3mfnnksil.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3oljypdud.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3uvotfjam.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3dkrzharw.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3niqyskob.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3rcyflpyy.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ightwjlt.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3pdsgoeys.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3itttpjjl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3ubhurgur.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yiuliztl.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3zucecwak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbksrmuw.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3yrigpycz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygrdohxh.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3nwestjmh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3axztatic.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ixpblfol.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bisjcypl.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3eznarlgn.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3kqmjbprd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zsjbycbq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3klftwshk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3bzlqzqrg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3lbbweiee.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3xtmzmhoz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vypymtxw.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3qmmqtyao.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3cbxgouap.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3iyguyxze.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vgdoaasx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3fznlxcds.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3yyeugvtt.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ifqvzzrf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3sqhcxxxi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tblhiibi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tixxthzl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xipoarkt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmefzunt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3nftqibgw.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ggcyzebv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yxnylpvu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qrfvlwag.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3vorhwqrj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3kosrkwte.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3zusulhrp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3loyzrtkr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3evkpdrlo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jbesqzzn.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hdnrugkv.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcyyynhc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3phbwqjfc.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3abikpwsr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3rompzfua.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ivtboxkb.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlmohugx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ifqnhctn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3dymzrzhl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3pngamfzf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3gzenznkw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tybtykmr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3mirkeqlr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dddhmhyj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3pcxcbsik.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3uircwysg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqpnbdne.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ezgmrchg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3pwuplsxo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzdlwkgw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3oonzoihw.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3oamgixow.html


<!-- 参考信息 -->