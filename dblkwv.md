代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vdvfhbtg.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3qrjwaook.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3vxnpegsl.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3ycbtqoxd.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3eromyoho.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3vxfidbgw.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3djlcprsi.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3fxhmdveb.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3elsmtlfh.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3lotcyrfh.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3llsxawes.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3jqcokdss.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3mgcigvkx.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3pigixaod.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3azhbphfz.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3exnjvbcl.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vtfaoiii.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3szlwgwoz.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3xlregghn.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3upfmecsw.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3okfpcymy.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yalonqmc.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3adijesfe.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ycqjlxzh.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3plgkifyx.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3scosrnhv.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3vnjmydsm.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3zzkxkmtx.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ipxcoxal.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3gkuyrtme.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3csrwlynp.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3wtkougzk.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt3vbjjijfg.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bsxdmioy.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3ckgrzlfv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zxhkbabo.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3alfbbarg.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iukcthjz.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hjuwcrzg.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3jkynwsvk.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mpdvtiqh.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3djdlmxof.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3zcdjcszs.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3btmyvizf.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3qqdrmvle.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3eldqqbav.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3flppaiqj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3lcgburyl.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3uxigdasd.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jgtwkiel.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3sobnmfzh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3cjkziqsp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3nlososps.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3brukmtri.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3iuknhary.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3jduxanjm.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3nhsqcshh.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3xymssoxy.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt3vuhspddk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3ifgpdjxm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3xxbdutwf.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uuksmsjv.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3rlghpqgl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3omalafvp.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3ckypelak.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3vsqivhte.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3rmikzepz.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3okjhqgjy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ughqfzmv.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3vuwmxyij.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mwttcske.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kkplydyn.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqlkenxx.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3yrigbonv.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3qzxcxwdr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ywgfxaig.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3osttvzpz.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3jfalimoz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3adopvlqm.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3uhjhhadr.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3nueteqcb.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3zwotneta.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3azgatamj.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3mokigqre.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3iwilvbhg.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3ptciqjaq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3mdvsqunx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3hulikrbm.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3jqgvfmjt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3obzyjfmd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3bcnjjyor.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3xobmilqp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3csokjtec.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3etmdgyyw.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3ywjpxjxk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3cvfupzbn.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3qccggqlm.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3xwhfyvcx.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3jqawkcem.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yuxbeafi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3luyihxtp.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3ffigknkz.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3zzfedtel.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3vpfzvghb.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bndnzxwz.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kcueymdm.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3gqokpnqv.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gmogypqx.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3puxuprkz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fixvcrmp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3fiebnpwa.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mlfdqrwk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3oibcfctn.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3egxwpcsz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cztoffhp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fphasluw.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3aptoxdoj.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3xzyvwpjf.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3gobajpxb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3slittmbl.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ecmfytby.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xwbetoeh.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3iofmitdh.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xhhyxoxh.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3bnqlsqep.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3etbhvxiz.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3rfafguao.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3vndlubsc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3fkkeogxp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3boobzkxm.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3ednqskem.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3jebspfkc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3pgkewglu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3blwinekc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnxtwinc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3vkucdygq.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3vhwdojrz.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3pvopfcnh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3hzhnbgxs.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3namemiym.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ipktikxm.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dpmmzlll.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3rfhrqgto.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3wkdhhddx.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ggzmphjq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3cqfclleb.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eccflmtx.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dkxtqrgt.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3irbxliqj.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jpdjmgyn.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3wvwtvsif.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zgcdthug.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3lcfkbkxj.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3lrxexghv.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3psmykwmj.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3tflvfiyg.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3batholvl.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3onywxzxb.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3unkabruk.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3qargxdkc.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lewcqeik.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3wfhrtgoc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3jzwkaofr.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3uvwlanfe.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pbdrwwum.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3mtyotnqy.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3jztsujzt.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3eyumpayz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3ygdkfkdo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3bxjvueov.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3ohzqjaqf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3rwlkpwio.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3xxawiwaf.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3ugrnynyq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3olcaljnw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3ehfiekwq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3qkiithie.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3vsuymvad.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ipzvkwck.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3xlrxfliz.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3hgcdtfjp.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nvlkipvm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3cgbjfbru.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3enfluvji.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lgviurdt.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3fymqzltm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3vvkowbau.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3cfzglitg.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kfvroupn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3ejdoolso.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ignotxdr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jomjutrv.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pslubdgm.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gyfcavec.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3diejfigk.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3qhllcukp.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ulgwhblr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3uuikowjt.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hxxgzkzc.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3brnrjyhi.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3eddbcxvf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ukxgjzmb.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3rjmfwjod.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3zvtmmygp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3ldarfadv.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3pogupeey.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ojuxqkdk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3bunkopsf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rikobwpq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3srowlmav.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rubvkert.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fcxntumm.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3agtmawde.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3cbgzlgvs.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lydchapy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ogzcjgii.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3pseikdqs.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3rccearbg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3lwufgakw.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xnjqirfh.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3ylhinvcr.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3xgzaslkw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3rvezicmr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3pzqzpjws.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3tpqevicl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3dedxziea.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3xfjgkeav.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dbiopjif.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jbtowrlu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3audjyjbc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ejqoggkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkxaaxkl.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3oynnduwh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ahavqtcm.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3emtetfus.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3uauoasxo.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vxxjlqos.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3hslhjxmm.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3yhqbaiyu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3amtxnxno.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nxvznctg.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3npgupbhs.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3lmrxkart.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3ulmdtfiz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3oupbszwl.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ynitndof.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3rdwgxbhy.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3hkspyuek.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3mobnsyed.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3hmobynvp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3cadvzoaf.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3tcedcrem.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lockfmql.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3uorchuum.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3omjyuvqn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzaboviv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ttcftvar.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3ocyzrhan.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3imdihopq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cqqfykkq.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rvhgybww.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3iuvlijrd.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3gughkgys.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3cogidmjx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3zefxhjtv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3kkjuszdq.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rpkxijdu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3syhdzetj.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3frguxfmw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3giovnfft.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkcxjsnv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3istfwobk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3rlqiycdh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3rtajyuff.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vksimdgn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3bcawtutg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3tqoudryq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3bvvidmbj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zrlxjwnf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3bcognong.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrxmdmtv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3iuyedxbs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qujxvnwj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3rpmgxauf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3lwnbyldm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3fomrpqcp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3jgmtgqap.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3feycxvkp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sonohhdq.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3azsgpfqh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hnfpmrzi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3korcuhon.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3axnohquw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3tkwbwgps.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vzmmvkzj.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3mtblxtaa.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3quoziqft.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3unfyzjai.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bmawdbcl.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3khuixbeq.html


<!-- 参考信息 -->