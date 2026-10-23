代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt3opmpyzbi.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt3szxhtyxt.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt3vwvfgbhd.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt3igkewxte.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt3rmaevwpz.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt3jhbepmun.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt3zleaziik.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3hckfxway.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dmcvsngi.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3yzrkpyyl.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3byblooqg.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt3lgnmrmef.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt3kredgqco.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3hdzomvtj.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt3mdnixxcs.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt3ojfrvacl.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt3lrvsxziu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt3njffdkiu.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt3wjueozdi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt3bldibydp.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt3osnjxyiz.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt3fjdpvtmx.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt3dphgifua.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt3jfecwphm.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt3vzuzgubc.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3hqiykiaj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3rzetrrsw.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3iaewimjr.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3zzfesuzt.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3pwkhuvzb.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt3dciovamn.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt3ertoauvv.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3yotcfkhk.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3haegkiqx.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt3riailiac.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3ybmxwlrl.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3vqaqekmv.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt3wzdrnvid.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt3xhyqkpla.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt3wvaqakzv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3qalhxmsx.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3umrxlksg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt3xnasyjmt.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt3njspdtpo.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt3sonzaxbb.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3dvhldlue.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt3lxunmeru.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3vlxffeml.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3eilcqnuq.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3ysvwypdz.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3oiwlppwe.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3wkqmwevm.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt3ujcfnygq.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3bkvqqyiu.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt3bhpidbqj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3nkaakepz.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3oyldhmsg.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3xhaonblu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uihtimyt.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt3alyoqfuw.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3asttfghr.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ctekmgym.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dbmgscmf.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3orjzuvqx.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3drjbvmwn.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt3pqtuncnp.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3lnfmstzc.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3cllnnaxk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt3ykdkqvmm.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt3egytircc.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3lynshazd.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3qmatumut.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3dfwzwfrn.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3azvoyjpg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt3nxakedmt.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3odbcvleu.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3gbuvxkvy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3xjcpshgu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3rfefmfnb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3bloopzvx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nvdywapt.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sbytrxeg.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3pkgdoyvg.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3kgnpjtok.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ljdpgdbs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3lslkmyoe.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3dnfsxgdr.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3fpjnbhep.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3sytlcdsd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3fdhkgqcz.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3dsuimuuh.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt3fndgotoc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lwjivnig.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3yojaqydh.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3ixkuvzrt.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3xynrfgnm.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zhsrpkwp.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3uwctrefm.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3gtabqjro.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vqyhpkek.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bdilgkcy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3utwechiw.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3vxtnnblj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3dopbqmni.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3spgrjhfd.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3mcihejwx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3akfojlky.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3wsaumwhb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3okladril.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt3kwaalzvs.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3dhkyvigy.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ispmytvf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3spkxadnd.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3qvqpverb.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3megcfvza.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qgczenhy.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3xmpwepfz.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3vfmaxpae.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt3gdtnevkh.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3hkjdyrrp.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3punwtdkq.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3okuxneuy.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3wvtdsgwp.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3exhgfkhh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3mcamnssa.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3itnpnmea.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqzsmxmh.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3fbkmijmx.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3ryxvyeia.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3cnpapecg.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqnvwfje.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3kjlmwcch.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rwxvmsoh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3saakmbnm.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rryziwjn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uftbpisn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yitjviyv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3lkgrynan.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3pwkerrbi.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yiardgzd.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3pujpfbbk.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3ndjiscyu.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3cdwzagdb.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3xtwjilzl.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3uijksbpt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3rpjqscdl.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3xwfbigte.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3suihjpsj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3ocmkkhew.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ifqvmqkx.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3blqyhvcx.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3nqotcrgn.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3smubgvdo.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3eecrcpvh.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3tvytuqww.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3emyszgif.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3puzywwxy.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3iivoudab.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3jfeyhtza.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3xiriazcg.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3ovqqlivl.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3zsbltydf.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3etdkmvyt.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3yrlufmzw.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3zihzczjb.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3cqphmkpl.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3ntdaewtu.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3bgjfnlwq.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3rfgiwijw.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tiaarbia.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lycvzxud.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hivdkiqw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dnyemoia.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tlfqkqos.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3wxzntkzu.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3lufkoiiy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tfvkyioy.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ncgjzgic.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3xatpvbxm.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3yqjblhjr.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3sytywwjl.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rxfsikzu.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3fmchufia.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3qwiapshn.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3kgrnsfbf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hyrqfany.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ozerbktr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3mewxjtfo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3aoxxvdlt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3vovtmclp.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3uwdboiit.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ymvovejg.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3uwrncbat.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3jgeisyma.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3tsizqgjz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3emmpcwha.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3tdomaejd.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ozflfxzd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3uhfaoutq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3nyefnnhp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sepycjui.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3oiqhcscj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3aaqgllmf.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jegpsede.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3osfpzvrh.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tmiihzuk.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tdmciejo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bhozyeze.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3layfmmuw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yucyednt.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3hxmtzrrz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3egasrjcy.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3cqtvqyuu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3uywfgoxn.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3lmjfwmxf.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3krngksaw.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3mczcpxjm.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3aexlzhvl.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3fedchznd.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3vxrkoiuc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jhnlbkos.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kndmjjod.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3clzjwqrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wejvbmfp.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3yhyrqlsi.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3yhbafgzr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3rrfmjlrn.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3sjfbecje.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3fuqukpeq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3evkaaogn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3qmmiqzrj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3eokupvcy.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3agwvhuod.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3icttcggg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3rcanocer.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfmawvrx.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3lvjxclau.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3makaoehi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bnxxmzri.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3nepvucgl.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3xeaexcar.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mxhlpppy.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3fpfavslr.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ebkyjsxg.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xatgbuhb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxamjwqs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gwgeexpt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3prtibhee.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yixfqffk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3wdlfrdgu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3aoogmrfl.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3evafxhqh.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3evtcbnwq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljnhtjjj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgfopiwp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3msutabqg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3otslcofb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3oaphzmtc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3khzaxiuw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ciaynhls.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rbzcitiu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3dordzihj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3omfjunqu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3wciqhddh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kwwkvkhb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3dupfeauh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3bbcwppdy.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3rqzlzzmu.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3lgawdvbb.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3clvjczxf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3wwuyvner.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3chygtauf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrsjaszz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hywxcjhw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3qukfrjhe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3apxiciuu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ipxpbdcx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uazyqcal.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3qxsugoly.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3faewndqp.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3afuxugyc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qnagitxp.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3txiajdja.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zjyoksfd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hpwzmyqv.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3thkicjgr.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dlirpvrl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ghkacagb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3glkblnti.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ompqwzxk.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mqreulok.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3plxpqfgr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vwrjtmho.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3wxbkzmtx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3zqoiunfq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3niutotwf.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3sgqkujws.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3jcunzxjs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uarjyooz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ilbgtpdb.html


<!-- 参考信息 -->