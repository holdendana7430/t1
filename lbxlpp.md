代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bhnqzhco.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2tsitzrkq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2ohrwkvlv.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zdkjdliy.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2usflyueo.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kckppaee.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zstejzrq.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2onlpokim.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2hbduinyu.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bwekrzjv.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2tbpmheaf.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2ujrmznky.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2lhnuilqf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2awrxorno.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2xkyecmur.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2jtbfafap.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2yhmucvbv.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2ympsjsvr.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2yybhafzo.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2tyrmjfut.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2hajrkrno.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2igmxqfxo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ntnvgylv.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2djeesfxr.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ghywatbl.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2rumjaoam.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2spxsiflt.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2evstjtzc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jxzathzv.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ezmrwsbo.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2daskdoti.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2rbwqiwpp.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2artmyuel.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2asydyhfx.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2axvkwcfc.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2jgfcbety.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kwayuigw.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hvlajdyf.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2yvetsxoj.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2utsabiiz.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2pieconpz.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2dotwboov.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2ylhjwxbu.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2tuyyrwbc.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2cfjruftb.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ziiobiom.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2xmfhehwg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2leihwgvk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlawgoag.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pbqukwlk.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2tnncyask.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2dxphpfhk.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2sfogwmyq.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2ldgkvupt.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vjrhnnfq.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vaezkukn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gdlogegq.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xazrpecl.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xxejmfse.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hlycxdop.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zeewwyti.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2buuqwctu.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2hfkgsscz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pexxabzd.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt2dtnsiesa.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ywfyfotz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2cydwivfh.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2gdkrzaxc.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fhkgagpz.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2faarowlm.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2csshnpwh.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2ilynjqkt.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2gvgjkxvr.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2jlcwlhno.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ykhhvwfm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2oamaglvk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ckxvysuu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ucfblfum.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nogjdgea.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2fdwkvedb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2izybruoo.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2paiolvtr.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ziyqlyic.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2zbngkqxm.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ptcjhlhh.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2jcopqdtp.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2zvylflbx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xuuerbgz.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2zzlklxcs.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2ehlxvyya.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2pdtjhgok.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2anariwxr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2idpobllv.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2samjgxyr.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fmoeylwq.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kffzttxo.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2svwtjymy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fqpctksi.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bcwqaddu.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zjqbfguv.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2ypkgwstf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2jkqtuefc.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2dhjhnyei.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fxmjwhvk.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yafsfxac.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2xgvgqohm.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zcsxjrlc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2wpeldahj.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2zeeoatlj.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2jalwfova.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2dvizasza.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ienyqgwf.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2nwwcgtda.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2kwqkjbcq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2wxutaumb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2lxjfwvbx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2bprjuxex.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2vcakyupn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2rtdjhdqo.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2lgkejndm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2zunbyxwn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2teorpexm.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2dpxrazft.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2tceztxyl.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2jactvzra.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2tpopvqam.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2guiwkjsh.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2wqvjikoc.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2cggujlre.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2effgwhuy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2uexokgul.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2fehugznb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dhsapemr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2oriusdju.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mjvytmqz.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dstexpnp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2gtcnzifq.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ovfsqoor.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2sbmlfkze.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2kryjpeir.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ogiayohb.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ltvsnqxt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2pwodupfe.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2ipqmamxo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2iceydxgg.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2qsutccdb.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2aignqlhp.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2mbuixrer.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2aomqnblp.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rwkbrtym.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mhtfjpko.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2lpflssdz.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2csvrdilz.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2dedieeua.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2qvpjmfvu.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2tcmegelh.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2xqxmwmbt.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2ggwdeicj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2alxuchsi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2qrddjiov.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2vhdwztgw.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2pgdjnedf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2fwecbuez.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2whjbuxgv.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2lmlxxhvd.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lbmjdmzv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ztfecnol.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2obghqcmg.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2oothovop.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2hdozlvty.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zqwaqllo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2sjjxldac.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rdfwisha.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrxvlbsj.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2ujunhkei.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2qsygxsmz.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rqoickag.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ylxqexny.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2axdwyjqo.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2fonycnqj.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ygcehcql.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vcgwwwoc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2eedibgnm.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gowmwcmh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2vlcytzkl.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hjvfdzur.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qsohzufr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2bjjpagqy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2avyclvjf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2lvqsktki.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2ptdlfqdp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2nbbflxpp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2hubwtvou.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2lznbyeqw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ahcctccn.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2jjwxzpus.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2bldbttjh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2ggqdjtzm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xvqlrymb.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bxnhrgep.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ergzzcwp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2huxiydru.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2yggmkqcs.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2qeovddtl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2slkswudt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ltykftgg.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2cqyvuhoz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2tptslywt.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2tqbdmiqf.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2jnohfjbi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xahsntmr.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2ucfacuuz.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2gdtmkomv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ziipwxtc.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2dkxvldso.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2szdyuzga.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ptdbspdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ahidfeql.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ofofzwzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dclchred.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2abruetds.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ccmqxbrh.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmfvggir.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2zngenpdm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ztpzxtwm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dhrbhjvb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2pysdcmqs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2ukhklbut.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2szmkkchv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2fgvanffz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2qqrumbtk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2adzkrpmh.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kzlevwpv.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oxnmjdkg.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2owufarpo.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2bicetwuk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2hwdtrwba.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dwkqoqvs.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2nnkczmis.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2lyskdmwc.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2gazruqrw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xxwikysm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xfkyfrwy.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cgjpolvi.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vokqujzl.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2fammifuo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2xudfbjfp.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hzfwanvb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mhilwvcc.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzhpdztl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymgizcps.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwfqgnsq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2peofvsxk.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ojupxgub.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ngzdjzvx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2vsjqnets.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2urtodsmh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2atnzyuxq.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2rzlwxmqv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2krpbhqfg.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqdfuhzd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2bhixbxhw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2grffqfoo.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2uzsscvin.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2xnmybbxx.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2nkndogpy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2azralien.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2eqsturqt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2xoskgzya.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2orzjjqfs.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jofskwci.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2vqauszfo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2bpwusamk.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2akizsggw.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2xvfxmnlv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2efaqqvxr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcettzsb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gesytbix.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyuyviay.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wsbggoui.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2itnyedms.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2jkpxgoiu.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2busbxddd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2jlxjcmwh.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vkfucmzv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wyjcjswz.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bsjxysbq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lczrgwaq.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mdwsrcvm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2eimmivih.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2cqwjboob.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2naiermhy.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zejrlbwb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2joitxoid.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uuatgijk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgqdwdld.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2zelpvxat.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jlcupvos.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2slxyxfdz.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ancfsafz.html


<!-- 参考信息 -->