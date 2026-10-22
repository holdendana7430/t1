代发 wailian999

Java: System.out.println("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2yntgchth.html

Go:   fmt.Println("Hello, World!")
来源：http://www.ydjk.org.cn/Article/details/gt2vtakagso.html

Ruby: puts "Hello, World!"
来源：http://www.ydjk.org.cn/Article/details/gt2knaymdsu.html

C#:   Console.WriteLine("Hello, World!");
来源：http://www.ydjk.org.cn/Article/details/gt2weoiasuq.html

[A02] 变量声明与赋值
来源：http://www.ydjk.org.cn/Article/details/gt2xlxpcark.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.52xcode.cn/Article/details/gt2kehjtjws.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2mayeebqp.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2loskneue.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2tqikmtvg.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2vzifbbnw.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2aachvnwo.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2mtpawurd.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2akwbpfxn.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2pnlitggc.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2iabxbeww.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2agkuieaj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pgseyngg.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2dgnnguvh.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hetjxdtl.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2spvzdbii.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2yebpgklx.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2onafkbsw.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2vpliyvnr.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2hofphxvw.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ypdzggni.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2nnfuzkzg.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2bgykdxbt.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2dtcmexni.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2pmwrlkuo.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2lksrcsgy.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2yovprxty.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2muclzjyg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2mvgcksnc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2cqbamgbm.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2lgzxzlck.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2tswjwxiy.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ttavzkeb.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2bulwtupu.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2cepioihv.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qcegvjcq.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2siwdarfr.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2rildcdop.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2rlgllwsg.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2vbcxwcif.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2qeuntcvw.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xnvcgevz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2npoodlus.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2xtprvxtk.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2urcbfwwf.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ajfiikih.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tqnoiwqd.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2pmsstdgf.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fuchtlrl.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2ngdqjjcs.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2tbhoewmv.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2utlahxzn.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2dqqvsupj.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wjasulcn.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2jmymqekk.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nvnwftmv.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2herlampw.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ikubuwji.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2mivccvxd.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2oukmxkye.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2psjzfcxe.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2jauidkzv.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2bqyjwgyr.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2lxblvetd.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2weyvqytk.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2etjlywbu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2vtvqlcci.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2brmtllff.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2bdvgvxeh.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2bmkfywvn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2qlqknsaa.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cyfomxxh.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2wtzdmhsb.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2oumfucpw.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2yuksmtfh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2dwstqmey.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2qsoxzjff.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2esdsbxeu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2oihzmfxl.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2skasvilb.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2yuhmdagd.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2hlckgqeu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2urspgdud.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2gruuusan.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2htyurqcd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vntwrywg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2exdooyxu.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2gsxpglic.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yvwyucnh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2aarkyfcj.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mqzxegjh.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2bajxnapd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2rqqccukf.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2kivbiwch.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2akkztlzv.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2gzytwaew.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2voeurzzw.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2vcwdeiwy.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2zwtnmtri.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2fdvhxhhu.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qgfwnwex.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2igcpxqqn.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kuzfdebz.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2cntcanws.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qzccpyij.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dqrtyiyi.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2aubwpram.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2sniywlms.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ubmkrnlb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qxbdjekt.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zbmwqjbu.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kebsyrki.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2pphuhwli.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2prvzgvle.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2sputzmeb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2gvkgzlrv.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rshnibel.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jihgjuig.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2yvorbmgq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zhcksavd.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2szatwifw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hdpdunti.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2reiogdsq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2oksjykvu.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2nibxgumq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wmosmdju.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2hgwldjbu.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ybgwatil.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2axfdgviu.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dtptlcoc.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uvbdopev.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jilkujyr.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2pdyswhom.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2vevrobsq.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzknrfpp.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ropvdokn.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mkifxpoh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kecdlans.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iuqylhyv.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2voimqqwq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xdjietxm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gmnmwpss.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vbencerh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dqrhradn.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2dcxhdkmn.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tyuulyzy.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ykjmtcrk.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2izqietwu.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2iuktggah.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2buwemdxx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2xdmblokk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2yvdkelfc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2kmxsvqok.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2huvyswhi.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zqnyjisw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ilmpcfaq.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2djhqorzf.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fxjlsagb.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2swqvbmab.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2exdbemep.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2kksbwuoi.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2xrtmitvq.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ygwsivpa.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2xwnyuslq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2fzucurig.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2zissjido.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2obevivyg.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2tdpxprds.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2eccdxgkv.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ffkynnax.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2wqmbhsqf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2gxbzpfbw.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2jwygucou.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gdumyesj.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oatlwaos.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2mfdaojls.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ismylztk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2puaelsdo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jfedbsux.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2zagqoimj.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2odpgckus.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmvnwkxj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2rsjljyvn.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2zcvjvbxx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2kqscebfg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qxsvozgf.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2hajrwumr.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ljuaqaud.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2nlbqwzrx.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2konqmnxt.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2cwohxesl.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2hhyzmszd.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2amtbcgqk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lglybixr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hmfzwjfw.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2siqzyxnk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nkbhphbt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ivyeeboe.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ejrawjil.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2iijzvrkg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2quctseul.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2zaydorxd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2pfmtpyts.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2kepgnmym.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2fhwxzhlw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2mpqrhhst.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2suqlzdbb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rqkfvens.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2dstqljyq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2laetnlny.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hfiwskwc.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2xnimhnjw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2crysexud.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqladkrg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2drnjmcfz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lraeszil.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2pmficahf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2nhfqlwah.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2agnudbhx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2noomkaqh.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2kkdhgvsu.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dyhqzdng.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2usrhqayg.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2mufcbatz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2xavzrreu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2urtxwfyc.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2iecfmjlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2onbqkela.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jnxdbksv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2cdayslwr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2czqegngv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2upespobk.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jmdmykua.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vjpkjxox.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2qlhccevq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2kkzjzgvu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lvcyhsoe.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2eltdopru.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2fjegwhzw.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkwywvtc.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2eexasypi.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2seyfleqc.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lqviawwo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2sqtafmxt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vzfejwgw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2odkqztsi.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2scdswwrj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2burdcgwh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2raozcebr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2yftwlygd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxzozujh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2plwndmfp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yvtcdmum.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2shdzuvdb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2gvrquewu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2zbzlofvu.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2kucafvou.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2dqphjhcf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pfvgpcir.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2betlkvrp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wcsrtnos.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fdpxtmbv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ilsyuhxb.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2yxfcqkpr.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dvwkydwj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2hgljhqug.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2bpzrfzps.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ffliorgd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqbemqhi.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2rzeoyodh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2oxjyvrjy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ikyqyhqu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2wjjqlrzb.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2hokmsnxl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2zlabbkca.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hquoocpt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2bobjidlx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2aujohkww.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ayheedkq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2bbuhatqy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2dlqsbmzr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2eekqblxb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2rrfnsvnd.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2sqdloxtd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2srgddbka.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wqluihvk.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mdeaxsxn.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsgboyte.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2sufcaefm.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2usfnqysu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2yienfzma.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2rysfxknr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2miazjzyw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vzhuwwxo.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2quyjqdjm.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qiudszcs.html


<!-- 参考信息 -->