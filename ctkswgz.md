代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://mobile.zdbjq.cn/Article/details/gkuvqepnm.sHtML

Go:   fmt.Println("Hello, World!")
来源：http://read.share.fehbvm.com/Article/details/gjwrgehsk.sHtML

Ruby: puts "Hello, World!"
来源：http://baike.fehbvm.com/Article/details/goqzghyiw.sHtML

C#:   Console.WriteLine("Hello, World!");
来源：http://www.share.zdbjq.cn/Article/details/gqqseiorf.sHtML

[A02] 变量声明与赋值
来源：http://www.blog.zdbjq.cn/Article/details/ggeeloctn.sHtML

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://3g.fehbvm.com/Article/details/gfhrmdlcv.sHtML

PHP:  $name = "Alex"; $age = 20;
来源：http://www.share.fehbvm.com/Article/details/gewbjddgc.sHtML

JS:   let name = "Alex"; const age = 20;
来源：http://m.share.hesvh.cn/Article/details/gkrthassm.sHtML

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://wap.fehbvm.com/Article/details/ghcjgnghm.sHtML

Java: String name = "Alex"; int age = 20;
来源：http://www.share.fehbvm.com/Article/details/gjrugzumo.sHtML

Go:   name := "Alex"; age := 20
来源：http://www.m.share.fehbvm.com/Article/details/gcbfwdwhn.sHtML

Ruby: name = "Alex"; age = 20
来源：http://www.share.hesvh.cn/Article/details/gexmibojj.sHtML

C#:   string name = "Alex"; int age = 20;
来源：http://3g.hesvh.cn/Article/details/gdhswebbw.sHtML

[A03] 常量定义
来源：http://m.share.fehbvm.com/Article/details/gpujtoxeb.sHtML

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://m.share.hesvh.cn/Article/details/gzbipjzup.sHtML

PHP:  const PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gnfshsznm.sHtML

JS:   const PI = 3.14159;
来源：http://3g.fehbvm.com/Article/details/gpnhiacly.sHtML

TS:   const PI: number = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gckgcubhr.sHtML

Java: static final double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gthrmqlkb.sHtML

Go:   const PI = 3.14159
来源：http://wap.zdbjq.cn/Article/details/gtpsydble.sHtML

Ruby: PI = 3.14159
来源：http://www.blog.fehbvm.com/Article/details/gaxqilixy.sHtML

C#:   const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gncpflphp.sHtML

[A04] 判断变量类型
来源：http://mobile.fehbvm.com/Article/details/gpdlkconc.sHtML

Py:   type(x).__name__; isinstance(x, int)
来源：http://mobile.hesvh.cn/Article/details/gnhdqlfmu.sHtML

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gbkpnyosu.sHtML

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.blog.hesvh.cn/Article/details/gbtxybaca.sHtML

TS:   typeof x; x instanceof Date
来源：http://read.share.fehbvm.com/Article/details/gyeeshlnx.sHtML

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://blog.hesvh.cn/Article/details/gvlptyoph.sHtML

Go:   reflect.TypeOf(x).Name()
来源：http://baike.zdbjq.cn/Article/details/gkhvlidlq.sHtML

Ruby: x.class; x.is_a?(Integer)
来源：http://mobile.zdbjq.cn/Article/details/ghrupiirt.sHtML

C#:   x.GetType().Name; x is int
来源：http://www.m.share.zdbjq.cn/Article/details/ggvmdobkl.sHtML

[A05] 整数除法与取模
来源：http://3g.zdbjq.cn/Article/details/gwikylcnj.sHtML

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.m.share.fehbvm.com/Article/details/gcddqfhrv.sHtML

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gulbyylhb.sHtML

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://wap.hesvh.cn/Article/details/grczgakcc.sHtML

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.blog.hesvh.cn/Article/details/gsrgslsqc.sHtML

Java: 7 / 2; 7 % 2
来源：http://mobile.hesvh.cn/Article/details/gwkccprik.sHtML

Go:   7 / 2; 7 % 2
来源：http://www.m.share.zdbjq.cn/Article/details/gridofycn.sHtML

Ruby: 7 / 2; 7 % 2
来源：http://www.blog.fehbvm.com/Article/details/gcoyivsjc.sHtML

C#:   7 / 2; 7 % 2
来源：http://3g.zdbjq.cn/Article/details/gertsonuy.sHtML

[A06] 字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/glbfntjmx.sHtML

Py:   int("42"); float("3.14")
来源：http://blog.fehbvm.com/Article/details/gprmzufgl.sHtML

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.share.fehbvm.com/Article/details/guystwzvs.sHtML

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://baike.hesvh.cn/Article/details/gmbhaktjs.sHtML

TS:   parseInt("42", 10); Number("42")
来源：http://m.share.hesvh.cn/Article/details/gxfobdgkn.sHtML

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://3g.hesvh.cn/Article/details/gbfthogvd.sHtML

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://baike.hesvh.cn/Article/details/gprrzvhsn.sHtML

Ruby: "42".to_i; "3.14".to_f
来源：http://mobile.hesvh.cn/Article/details/glbyjivpq.sHtML

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://baike.zdbjq.cn/Article/details/gbwbtrkar.sHtML

[A07] 数字转字符串
来源：http://wap.hesvh.cn/Article/details/gadlnwsyp.sHtML

Py:   str(42)
来源：http://m.share.hesvh.cn/Article/details/gtnqcrtet.sHtML

PHP:  (string) 42; strval(42)
来源：http://blog.fehbvm.com/Article/details/gxbtsiggx.sHtML

JS:   String(42); (42).toString()
来源：http://baike.fehbvm.com/Article/details/gmkgkssix.sHtML

TS:   String(42)
来源：http://read.share.zdbjq.cn/Article/details/gebcsjiok.sHtML

Java: String.valueOf(42); Integer.toString(42)
来源：http://m.share.hesvh.cn/Article/details/glasdigtv.sHtML

Go:   strconv.Itoa(42)
来源：http://baike.hesvh.cn/Article/details/gdoxdmopj.sHtML

Ruby: 42.to_s
来源：http://m.share.fehbvm.com/Article/details/gjrbzxbev.sHtML

C#:   42.ToString()
来源：http://read.share.zdbjq.cn/Article/details/gdeuykbjj.sHtML

[A08] 取整与四舍五入
来源：http://www.m.share.fehbvm.com/Article/details/ghfrrhcjr.sHtML

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://mobile.zdbjq.cn/Article/details/gxxduiwqm.sHtML

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://blog.fehbvm.com/Article/details/gzvuckyac.sHtML

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.blog.fehbvm.com/Article/details/gihzoqewi.sHtML

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://blog.fehbvm.com/Article/details/ggfcvxtzq.sHtML

Java: Math.round(3.567); Math.floor(3.9)
来源：http://blog.zdbjq.cn/Article/details/ggiuvlicq.sHtML

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.share.fehbvm.com/Article/details/gxwenzapq.sHtML

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.share.hesvh.cn/Article/details/gmowqjytq.sHtML

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.share.zdbjq.cn/Article/details/gbwlsbpqa.sHtML

[A09] 绝对值与最大最小值
来源：http://3g.zdbjq.cn/Article/details/gvfelqvxb.sHtML

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://m.share.fehbvm.com/Article/details/gljhcnmie.sHtML

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://3g.fehbvm.com/Article/details/gxelkadhx.sHtML

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gdnfskhlo.sHtML

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gfzkacupx.sHtML

Java: Math.abs(-5); Math.max(1, 2)
来源：http://read.share.fehbvm.com/Article/details/gauymufyy.sHtML

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://m.share.zdbjq.cn/Article/details/gpbilfwbv.sHtML

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.share.zdbjq.cn/Article/details/gtiaqfulb.sHtML

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://baike.hesvh.cn/Article/details/gbjztavbt.sHtML

[A10] 生成随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gleidqsqy.sHtML

Py:   import random; random.randint(1, 100)
来源：http://wap.fehbvm.com/Article/details/gnmvthqiv.sHtML

PHP:  random_int(1, 100);
来源：http://www.share.hesvh.cn/Article/details/gktfplpud.sHtML

JS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.zdbjq.cn/Article/details/gejymqgoh.sHtML

TS:   Math.floor(Math.random() * 100) + 1
来源：http://wap.hesvh.cn/Article/details/giorktlnj.sHtML

Java: new Random().nextInt(100) + 1
来源：http://m.share.zdbjq.cn/Article/details/ghckckxle.sHtML

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.m.share.fehbvm.com/Article/details/gylphlwyw.sHtML

Ruby: rand(1..100)
来源：http://www.blog.zdbjq.cn/Article/details/gvsjsqyie.sHtML

C#:   new Random().Next(1, 101)
来源：http://www.share.hesvh.cn/Article/details/gtplsfoit.sHtML

[A11] 条件表达式（三元）
来源：http://mobile.fehbvm.com/Article/details/gaoqqqxtp.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://blog.fehbvm.com/Article/details/ggufvgrou.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://read.share.hesvh.cn/Article/details/gdwnfviwm.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/ghixwjunl.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gaixubpwp.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://m.share.zdbjq.cn/Article/details/gkqxbapgb.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.blog.fehbvm.com/Article/details/gmidefntc.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://wap.zdbjq.cn/Article/details/gdefbcsno.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://mobile.zdbjq.cn/Article/details/gcslvlpqr.sHtML

[A12] 字符串插值 / 格式化
来源：http://wap.hesvh.cn/Article/details/gbkscbiwb.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://m.share.zdbjq.cn/Article/details/gmkzxcyjj.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.hesvh.cn/Article/details/gdetakirq.sHtML

JS:   `Hello, ${name}!`
来源：http://baike.hesvh.cn/Article/details/ginyhdfgf.sHtML

TS:   `Hello, ${name}!`
来源：http://baike.fehbvm.com/Article/details/gxrqjgugy.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.blog.hesvh.cn/Article/details/gmrtzxvjk.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://m.share.zdbjq.cn/Article/details/gubvweihv.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.blog.fehbvm.com/Article/details/gcpfpxmlr.sHtML

C#:   $"Hello, {name}!"
来源：http://www.share.hesvh.cn/Article/details/gfnzvlzcd.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://www.m.share.zdbjq.cn/Article/details/gmspocfzz.sHtML

Py:   "第一行\n第二行"
来源：http://baike.fehbvm.com/Article/details/gxgwvcrsq.sHtML

PHP:  "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gkygisrhd.sHtML

JS:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gpigbojxd.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gihqwhhbc.sHtML

Java: "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gdgvvfvkb.sHtML

Go:   "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gdvsnpuuh.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gpdvbgtrx.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/ghthazgpi.sHtML

[A14] 注释写法
来源：http://www.blog.zdbjq.cn/Article/details/gjoemdqxk.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.hesvh.cn/Article/details/gwovhhqcj.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/gdaoadxnc.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gwsonwtbq.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.zdbjq.cn/Article/details/gichzaoln.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://read.share.fehbvm.com/Article/details/gskikooyh.sHtML

Go:   // 单行；/* 多行 */
来源：http://mobile.fehbvm.com/Article/details/ghuxuokgf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/gzdcpisdg.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.hesvh.cn/Article/details/gvzricoek.sHtML

[A15] 空值判断与默认值
来源：http://blog.hesvh.cn/Article/details/ggrzakmfz.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/gvsfmcyjl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.hesvh.cn/Article/details/gundmhwte.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gerdgmudv.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.zdbjq.cn/Article/details/gabkeyaqv.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://m.share.hesvh.cn/Article/details/gifetnmrd.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://read.share.hesvh.cn/Article/details/gfjqmyopu.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.zdbjq.cn/Article/details/gickagwfy.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/godqdffdu.sHtML

[A16] 真假值判断规则
来源：http://m.share.fehbvm.com/Article/details/gbbzknkxh.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.fehbvm.com/Article/details/gplqtmhit.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.hesvh.cn/Article/details/giyxrmhij.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gdviopawk.sHtML

TS:   if (!x) {}
来源：http://read.share.fehbvm.com/Article/details/gomliflaa.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.hesvh.cn/Article/details/gzsjuwqyx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.hesvh.cn/Article/details/gkaxwkmra.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.hesvh.cn/Article/details/gkpqboqgl.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gybyixylf.sHtML

[A17] 位运算
来源：http://www.share.fehbvm.com/Article/details/gvczggtft.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gjhxiahuc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.hesvh.cn/Article/details/gfzrgodfi.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gzucvollm.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gylqeikhs.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gjepnxheh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gwlhyydwe.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gnhggnvbj.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gewzeqzkk.sHtML

[A18] 字符与 ASCII 码互转
来源：http://wap.zdbjq.cn/Article/details/gghmpnstn.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.zdbjq.cn/Article/details/gcwaclrzb.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.fehbvm.com/Article/details/guuymhdkq.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.hesvh.cn/Article/details/gohredepd.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gpcljxbht.sHtML

Java: (int) 'A'; (char) 65
来源：http://m.share.zdbjq.cn/Article/details/genbepwbj.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.zdbjq.cn/Article/details/gcuzbchoe.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.fehbvm.com/Article/details/gupopbwvw.sHtML

C#:   (int)'A'; (char)65
来源：http://mobile.zdbjq.cn/Article/details/gpxegaztq.sHtML

[A19] 交换两个变量
来源：http://www.m.share.hesvh.cn/Article/details/gzankmdjz.sHtML

Py:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gmchhegop.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.share.zdbjq.cn/Article/details/ggenbhzak.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/gwpwgchvr.sHtML

TS:   [a, b] = [b, a];
来源：http://mobile.zdbjq.cn/Article/details/gkncoojtn.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.share.hesvh.cn/Article/details/ghzzgwoqs.sHtML

Go:   a, b = b, a
来源：http://read.share.hesvh.cn/Article/details/ghvtuvqoa.sHtML

Ruby: a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/gmrahhsnt.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.zdbjq.cn/Article/details/grhxjknnm.sHtML

[A20] 读取标准输入
来源：http://www.m.share.fehbvm.com/Article/details/ggedxnuot.sHtML

Py:   name = input("请输入：")
来源：http://m.share.hesvh.cn/Article/details/glkdnvpvh.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.hesvh.cn/Article/details/gwiyrdzpd.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://3g.hesvh.cn/Article/details/gkepmnhsk.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fehbvm.com/Article/details/gzujkhkmf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.hesvh.cn/Article/details/geccmsjyo.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.zdbjq.cn/Article/details/gudrqculg.sHtML

Ruby: gets.chomp
来源：http://blog.hesvh.cn/Article/details/gntzkatfl.sHtML

C#:   Console.ReadLine();
来源：http://baike.fehbvm.com/Article/details/glpsatzcb.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fehbvm.com/Article/details/gfdduukdx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.zdbjq.cn/Article/details/ganumhpis.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gsiqjrzhu.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.hesvh.cn/Article/details/gxefwmjqt.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gnmpixzji.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gkqexjyqu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gqvucmzty.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gngniffsw.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fehbvm.com/Article/details/gkrccgwmi.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/gxtihxdcm.sHtML

Py:   len(s)
来源：http://baike.fehbvm.com/Article/details/gpylavlmt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://blog.hesvh.cn/Article/details/gsllzuoed.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.fehbvm.com/Article/details/gvzgcgjsg.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/ghhknuocj.sHtML

Java: s.length()
来源：http://read.share.hesvh.cn/Article/details/gunjlxclz.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gtnkkdhwi.sHtML

Ruby: s.length
来源：http://3g.hesvh.cn/Article/details/gniobywcc.sHtML

C#:   s.Length
来源：http://3g.zdbjq.cn/Article/details/gdrxcbipe.sHtML

[A23] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gwmqnhtkh.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.hesvh.cn/Article/details/ghsdmcxte.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fehbvm.com/Article/details/gdgvyxpuz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/grmbqjbhw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.fehbvm.com/Article/details/gkktvqoai.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.share.fehbvm.com/Article/details/gxpozlywu.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fehbvm.com/Article/details/gafwmjxaf.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gghcjtmrh.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fehbvm.com/Article/details/gcuubztbo.sHtML

[A24] 去除首尾空白
来源：http://baike.zdbjq.cn/Article/details/gizvcaubp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://m.share.zdbjq.cn/Article/details/gylyjtpak.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.fehbvm.com/Article/details/gappfyikw.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gdhfzidig.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://3g.hesvh.cn/Article/details/gzckmtxwi.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.fehbvm.com/Article/details/giflfcexm.sHtML

Go:   strings.TrimSpace(s)
来源：http://wap.fehbvm.com/Article/details/gkrmsvzrt.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/gzjoqeaih.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/ggvzicjbl.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gmqjplace.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.hesvh.cn/Article/details/ghnaepqds.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/gnidpycec.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.zdbjq.cn/Article/details/ghlmtsngv.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.zdbjq.cn/Article/details/ghqjaccys.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.hesvh.cn/Article/details/gbmyursys.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.hesvh.cn/Article/details/glgnapbic.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.zdbjq.cn/Article/details/gkzntykya.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gfkwqendx.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/ghbopasvp.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.hesvh.cn/Article/details/gujdkjyaf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.hesvh.cn/Article/details/gojkiekpe.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.hesvh.cn/Article/details/gdpqvohuv.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.zdbjq.cn/Article/details/ghgogrjcb.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gkpsyvlvm.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.zdbjq.cn/Article/details/ggfjckjyu.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.hesvh.cn/Article/details/gxxztrfcz.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gjfvjtuqu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gdtuccvro.sHtML

B. 流程控制
来源：http://wap.hesvh.cn/Article/details/gbcavvtvd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grqnssaas.sHtML

[B01] 条件判断 if / else
来源：http://www.blog.hesvh.cn/Article/details/gzbmrlcgu.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gcmmqtbib.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://m.share.hesvh.cn/Article/details/godfiqguo.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gbvxjbnvp.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/gasefdqsi.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gpklluxxb.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.zdbjq.cn/Article/details/gcwpdvzej.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/gdvvsjiff.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.hesvh.cn/Article/details/gniorytwn.sHtML

[B02] 多分支 else if / elif
来源：http://mobile.hesvh.cn/Article/details/gngzylnku.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.hesvh.cn/Article/details/gqqumvjgh.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfonvwxqd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.zdbjq.cn/Article/details/gvybqqqbj.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.hesvh.cn/Article/details/gfnklport.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gkqfmpuuz.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.zdbjq.cn/Article/details/ggmhycfjq.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.hesvh.cn/Article/details/grwzkagpb.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gfpxhurmx.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/glxktrlqd.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gbrglyith.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gzitiluzi.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdikgneba.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/gtcnhodmy.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.fehbvm.com/Article/details/gvzfvbhfr.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.hesvh.cn/Article/details/ggjgbtnxs.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.m.share.fehbvm.com/Article/details/gvvkgjres.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.m.share.zdbjq.cn/Article/details/gfsyrebpi.sHtML

[B04] for 计数循环
来源：http://baike.fehbvm.com/Article/details/grkahhbmq.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.fehbvm.com/Article/details/golsvsznb.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.fehbvm.com/Article/details/gvsehudnr.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gdrybzujh.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gdsldjnfq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gtykupipp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://m.share.zdbjq.cn/Article/details/ghmapltvp.sHtML

Ruby: 10.times { |i| puts i }
来源：http://3g.fehbvm.com/Article/details/gyohrmgut.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fehbvm.com/Article/details/gutvmztlr.sHtML

[B05] 遍历数组 / 列表
来源：http://www.blog.fehbvm.com/Article/details/gqmklmfft.sHtML

Py:   for item in arr: print(item)
来源：http://baike.fehbvm.com/Article/details/gvkswkfxa.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fehbvm.com/Article/details/gzojzlycx.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gcyiagxzz.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.hesvh.cn/Article/details/ghcwghtqa.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.hesvh.cn/Article/details/gywqacanb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.zdbjq.cn/Article/details/goevqjczl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://blog.zdbjq.cn/Article/details/gogltqjqk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://read.share.hesvh.cn/Article/details/gptmlacbu.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.fehbvm.com/Article/details/ghshluyfz.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gayonsgyt.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.fehbvm.com/Article/details/gtkfutqum.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/gyldftgkx.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gunjbnbiv.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.fehbvm.com/Article/details/gxnixhiel.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.share.fehbvm.com/Article/details/gclnzclfg.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/givvborpn.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.hesvh.cn/Article/details/gbpypubnn.sHtML

[B07] while 循环
来源：http://baike.fehbvm.com/Article/details/gcqhjngfb.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gbiwcytfo.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://blog.hesvh.cn/Article/details/gzpyimxkh.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gmjngodyv.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gntyuispn.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.hesvh.cn/Article/details/gemotyfgx.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.fehbvm.com/Article/details/gxzuanbfh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/gptvyojeq.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gewufmyoj.sHtML

[B08] do-while（至少执行一次）
来源：http://www.m.share.zdbjq.cn/Article/details/gfecdabii.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.blog.fehbvm.com/Article/details/gtkarzplc.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.fehbvm.com/Article/details/gffogkzof.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gsgohcwes.sHtML

TS:   do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gwoajtxgd.sHtML


<!-- 参考信息 -->