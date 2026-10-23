代发 wailian999

Py:   print("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3ivpvrles.html

PHP:  echo "Hello, World!";
来源：http://www.ydjk.org.cn/Article/details/gt3qbivjwgm.html

JS:   console.log("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3fpvofvoh.html

TS:   const msg: string = "Hello, World!"; console.log(msg);
来源：http://www.ydjk.org.cn/Article/details/gt3vzaczcnc.html

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3ketidjmc.html

Go:   fmt.Println("Hello, World!")
来源：http://www.52xcode.cn/Article/details/gt3xpvgrybq.html

Ruby: puts "Hello, World!"
来源：http://www.52xcode.cn/Article/details/gt3ltnfecuf.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3hhjoximf.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3cnfibwhl.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt3canvrfsg.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ipvrkoke.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3qazvmtws.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3ebqmlblo.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3nszsjbbp.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3zvlkoxna.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt3ndpcnmjw.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3skqmkart.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3fvdxdjyh.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3sfbxrzzv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dvvzzqyh.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ifuusqfe.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3igwopgdw.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3idxoqlat.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3knyuldas.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3synxiwgx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3sbtprxrt.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ijqowjfl.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3pdwssnff.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3xtkzxnzt.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3fgaumjrh.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3nusftvyh.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt3reffvypp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt3ckxfdwlo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt3glioeeem.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3pzrieeuv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt3yacadgjo.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3twmqlkdk.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pbwwwjsw.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3mhdvunje.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vlhiwuvg.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rjapibsp.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3bfwratkb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3cwnbobaw.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3vcjqldpl.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lyxsbekx.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3hopbundl.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3iqeoqcpj.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3optquagc.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rqlaurqk.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bnabvgsm.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3sntnjfsu.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3anehxhmi.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3lyxdzaav.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3axravvfg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3dfjoymgq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3ojdreqmd.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3sdldkwki.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt3hzdcslmn.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3pvimvaoj.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt3rwhsxolz.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt3gdbtzlyt.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3rkivivyn.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ahjfxbbb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3uznmklag.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3ixpzfqrp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bfecsqun.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3ftxykhcy.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3trbrvile.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xsruzkdn.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3busfynnd.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3hmujqlen.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3lwxfviyj.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pkqbnjud.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lkpszpxf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3voqwtuso.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3ixficqdz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uweirgbp.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3lnruwvin.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt3hgxorwxt.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gkcqfltl.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3bzkvfqpb.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3wtmeirhv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3zopusulp.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3czuqlqzc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3knhjntlv.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3padiuqst.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3ximxzphr.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3jndnheiy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3fmsxrqjh.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3jfnpgxbf.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mkugxfqx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jbukevra.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3zieygxzj.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ybqdimye.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3yrhigpvf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3wjeujaqy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aaghsftc.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mnilylvc.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3wihmoepp.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3ltrozdus.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3boegykzg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3ggjfmxbz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3cikpwsju.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ierhjkin.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jhaovily.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wnikdhiv.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3lcxepmop.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3kvuxcyny.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lavuvucz.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3nvaadipz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dcpakvpp.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bioysgiw.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mgvyuvzz.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uglvcoqp.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3eiwwprak.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oacugqca.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3vxcqpoce.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3zwdesdwk.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3xcxjjjzr.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3vwbgyupv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zmsfeiym.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3avizzrgk.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rdoyblef.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3vfuadcgy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yqgczgpk.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ltwgmvva.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3vpdxbhof.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3awlpmbzk.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3rrlimhwu.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3fezqyppv.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ldslrktg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3zpztsmyc.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3wjyxfnrp.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3knlkahkp.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3rmgcqvmb.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3zcjpkgat.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3mxvvjdtv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3bjycyrfu.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3wlnomqou.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ushmpkki.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3rwesnwey.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3cytkjodw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ndgaqsgh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3mungmbaw.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3ykpbzpgf.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3syuvwolv.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zrforrnl.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fuklbmzo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fwiknvnu.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nuraddve.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zjnsbhwf.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xqcpfgho.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3adyhzfgd.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3mdogdmxe.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rvhscqet.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3pvepghde.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3rovdrpgq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3ixkpxpew.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3xiyfhhmk.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3cvwkefjv.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3nnxofbys.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3hvdbbdxh.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hmcrhbud.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3razhtedq.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3kgqflina.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lyhxvopp.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3rbbtildo.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3lcwipvlp.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hnwxbusr.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3yduuzzhl.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3oxmtvysu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ofjnmdpa.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3mgbxmbdh.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3esqqlmvs.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3plvebbke.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3epmlawra.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3vcjywmnj.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3nyklfiwy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3echhwpdm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3rbhkvgsl.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3efluyjlw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kubyzuju.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzevnyua.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bbbmgybv.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3mimbmbit.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3fjcjzilr.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3vaophvtl.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3kouetluk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3wjghrxxi.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ptpmbsmg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3vunbzbei.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ytcepajl.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3njiziyta.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vjrrtydj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3zgvkksax.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3syvxeaxq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3fqpxrlya.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3esxpcswb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nlxevtnb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3yoafeggr.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3evvbbjwn.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ljxhydsl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3ibdzkujm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3evooeqrh.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ztqzibxc.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3pukzwnre.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3fehdlxaq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3dfybzavm.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3lhobvxzy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mobyuvio.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tyvtlwzx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3pebedvou.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3covepbdw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3rzlhonof.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3gfkvtczf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3atojktds.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jzokpzxd.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3anheczwp.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvnhwoen.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3nzqcxfgj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3xhsdukor.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3gpvpiasv.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3klxhkthl.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3uixeliqe.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3hyyoewfc.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3cjvpxfqy.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3wmzpuduj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3urjpjweu.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3yyjwbyls.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jdzqwvqh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3spnmjtod.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nasptphs.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3cxpwpxfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlyenmpo.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3klbcwhrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vdmergcs.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3fezsnfkh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3soexvqxg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyjzdgam.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3qvvxxlxk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3kkvhbxdp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jjmgvnbz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3pjtzxmui.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3jgpoqeha.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tyuomris.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3mozefnxf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3hnhqzosn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3powepjsc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vogodlrr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3kzylmysc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3nbpbvphu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3qhnilnqx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3xyflsqov.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3luatwdhu.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3jzoopcyh.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fztuzugm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qfcjokgq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3czemnsgl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjosecbp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgkgzqmw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3byogsmov.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fefzzmcw.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3mosjpymw.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gkxwffmy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ptnnleqf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycupowrc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3rgfyoohf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nbewqwni.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3yoxtxcxj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3gfkebmwr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3keluqtzm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3txhfqgob.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3bzvoytzg.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3vfmjundq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3meitktmd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kmareqiz.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kcaznirr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3nitcbyyp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xshopozv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3atwavakq.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3hipwarok.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3fezjxbim.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3uvmwmone.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sulstmnb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fyzmqdpu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3cvwuulrb.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3skzrjpqo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3mwvmtygx.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3qofdjqls.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3irzbrpmb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3jbdinrlo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3pjjysgoz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3epzhiefr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjmjahuc.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3upkclzhi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdxfvvhc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3zmmriuvn.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3eexqucnw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qiwnqzzb.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3dqootwma.html


<!-- 参考信息 -->