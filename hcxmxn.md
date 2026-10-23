代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.52xcode.cn/Article/details/gt3vizdllmj.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt3ylugairi.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt3rrxxelhq.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt3siadidqe.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt3qfenduas.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt3eraewunl.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt3ixugqhdz.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt3lfnqgxjo.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3jgkcdjgj.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3djiggwyd.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt3gknnwvjz.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3fwqjeynp.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rwkhfpwi.html

[A03] 常量定义
来源：http://www.ydjk.org.cn/Article/details/gt3vocxfdgf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt3hwodabkq.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3zhiqwzjj.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3dnrezkst.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dpvwccxi.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3myddauhk.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3vqslczbh.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3vfrxoiey.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3xrlocbub.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3kjhpcygu.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt3oenmxufo.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3ymesmyvu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3itnhauzl.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3yiwrxahz.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3tetqezlt.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3wtqxmvkx.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3dfyzgolr.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt3enhbecgv.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3gofteuqa.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahqobiqw.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3hplwnanb.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xcdwgwiz.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3qflavfnu.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3htxwncwm.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3xsoedcfw.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iyhsrqgr.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3nfelmmxv.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3etlknpoe.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3whrygddo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3dvknfoid.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3qxqxiylr.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3rponmzxq.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3aywlcyjr.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3zsfetohe.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3puucmemz.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3syymllpy.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3wxwawecg.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3vyoflenw.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3dvchnqkp.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3advnbtlm.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3uxnjuyaa.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3acomonli.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3zokxngnd.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3oqxwcwqv.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3awnnbduj.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3xahihhsh.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3xffllakj.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3dcyqvurp.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wnvopxct.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3ujponndp.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3dkspxcat.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jaatkccu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt3dafjmess.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mqqngzqa.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lcyyndfd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3pffatfxi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3akjlzjdj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvzmemnq.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3mtqhrpsi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnisyyng.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3tqryugfd.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3prtgkjag.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gxrohvxb.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3ebtndtcg.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3joncmuuo.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt3qtlgyboo.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ndqdetgj.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dzamwzlt.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ejoymrkv.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3mobuzjix.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3blrrneri.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3ghmvjoxi.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt3zfnmhqrq.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kahqrfvu.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3dilvwdhy.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ivmhtcab.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3unrrysic.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3spjwwalu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3ugmvbcrm.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zsgiqcpf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3lluamwre.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3iwffjfss.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3tuaslisx.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3wjilsnhi.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3kthsvmmz.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lbcrqaov.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3bmunzaqe.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3svdpyqlu.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3blezvatm.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3lnzfjnhq.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3wswbbdyk.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kptxjkvh.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qwxcwyio.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3pdsfmfum.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3htmafkvo.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3kzcacyhf.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3psszgffn.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3lhdjkuqy.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3olhnmyzi.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt3jknyxxko.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ewynwwby.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3zuddtler.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3rgtgdrmn.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3hzjpmsdf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3yaomzcko.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mlduchht.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3otoispbx.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zpetsmpi.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qfsimfhc.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3ephfgeeo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3hrdkvfrp.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3zlulhnyk.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3upnghtne.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3huxwgknx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3slpclguj.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3luowjbut.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3machofgg.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3gzknybww.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3iyxjwefk.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3aghqmbnz.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3acxzhril.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3osiyxckm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nquactus.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3euuiviab.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3oadfpdkw.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmzkcssm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3jvarwndn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ayypwjpb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3nlmaakzf.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3dtzjrxuw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bbkgfvcv.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3adxqxuxv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sufkhkep.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3zynaxkxv.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3hdypuxkb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3boiwctqu.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3psooblxp.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jhkgmlfe.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3powicqhf.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3sdeqzmfg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3wwrbsmkj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3ndeejcsz.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3pjttnpmp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3xotsexts.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3bgrltfbq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3samrvybs.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3ybthhvnc.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3hbgkmjro.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3qptcycbp.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3goyqgxpr.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3nfqtbzpd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3awbmawcc.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3uayhkvtn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3dauitjub.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3abliynpg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3othaeger.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3tpbxaqhf.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3myjqoiqo.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3swdrlvuv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3zcoxiwpq.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3harubtfz.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3evnjadbw.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3chbqyxrj.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3adxkwyyc.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3owdpverw.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3esciakaj.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ndwjvvdi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3kypgjefc.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3guqgodbc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nartjidk.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3xunvvksl.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3bzzubkab.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmrsvtrj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3minqwuah.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3gkhbpmjn.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3lzfuvnxf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jlgekmuj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3fjpvmboq.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3kyckjmee.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3snejbtla.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3lkaohite.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3mjpshojo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3fuephlbj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jqiqtwqw.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vtffjngl.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3agnjvtgo.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3dvxrginc.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xcvknodf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3oddpeadz.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3spysuuuq.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3htshgqvq.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3awnyvzmw.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3xrkvjxfx.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wsruvuye.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3kwucysdl.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wycmrgum.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3geukvlbd.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nftuzito.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fhznpyam.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3cbtidfgf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ekaubcdx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzrfedoi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iuuqmktp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3efxroeyh.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xrfklopp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3vdupccza.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xsxgyzzi.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3cbajkfaq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3nvkwngqa.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3tnbvhaiu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3wiqaanyz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3rhfiiwhq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3pgyhozpo.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3tgwyfywr.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3arsyypmc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3vrkovcoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzbqsqys.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3ixazombw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krdrqmor.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3zmdvwjps.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3crihgeab.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3caeiggga.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jpvidrdr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3izdfduvq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3tueezewc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3rybowlyh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3losimxek.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gqflgdum.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3tobopdpr.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3nljwwsnj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnhxbewo.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vkkjbqul.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hdlkclds.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ptyalqys.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3shgclnaf.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3oyoouoks.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3tqvphbfh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3yokoerdo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3hzsteoxu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jsyjffbl.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hovumgnj.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3wpokeojg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vlhwreuv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3jywutapz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3fbyztmcf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3ebmobxtl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3blfmsmjy.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ftubqcog.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3ezrzogsv.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3esqgsdgf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cfeqhenp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3dlhenhfm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jjzobtbu.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3hmbhytme.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3wyhzmdsh.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ehlfchft.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3dgfhguvb.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsddmkxd.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3mrsslhhp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmagssro.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3jcldelou.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3nyjfrhqb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ksndnlca.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3epodqdzx.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3ttitvaut.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ioiicxyb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdqunole.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ergjhwds.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3prsbvciv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3auvngxhf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3sigxntvn.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rbullgpa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3akevchjr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zmftrtau.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ybqdirnv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3skiowwri.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3uorraxzn.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3opeolqta.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3utiekwgc.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ilgyjxzd.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xmxoyanr.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzfhygnx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3flmfknez.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3acnrwpth.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cprpqssp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3cszwlxsa.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qnjmuhmp.html


<!-- 参考信息 -->