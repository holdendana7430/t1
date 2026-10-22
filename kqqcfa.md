代发 wailian999

[A02] 变量声明与赋值
来源：http://www.52xcode.cn/Article/details/gt2exejrlpa.html

Py:   name = "Alex"; age = 20            # 动态类型，无需声明
来源：http://www.ydjk.org.cn/Article/details/gt2jbdvcsxp.html

PHP:  $name = "Alex"; $age = 20;
来源：http://www.52xcode.cn/Article/details/gt2otsuaktk.html

JS:   let name = "Alex"; const age = 20;
来源：http://www.52xcode.cn/Article/details/gt2bsmhucrd.html

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.52xcode.cn/Article/details/gt2llzpdiwb.html

Java: String name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2kcaeuuxy.html

Go:   name := "Alex"; age := 20
来源：http://www.ydjk.org.cn/Article/details/gt2ljqipuyo.html

Ruby: name = "Alex"; age = 20
来源：http://www.52xcode.cn/Article/details/gt2oplncfwg.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2zoizbobp.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2qhrejhsf.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2oifhvxvj.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zplsaumg.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2yezvhpiu.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tovmcfhd.html

Java: static final double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2olumskze.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2uxctskqz.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2xdnrahfy.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2udrkczoe.html

[A04] 判断变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ivvsezpc.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2lohsgysz.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2fyetjabu.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2jfbfpnds.html

TS:   typeof x; x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2btjspgrl.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2mklovibb.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2mtaffpre.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.52xcode.cn/Article/details/gt2sjstrjtg.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2sacrnfji.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2dbcxdopg.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2kyeuekks.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kwbvzjoj.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2fkdzjqyh.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qxofyqlf.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2jjalrfux.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2kioxbhsv.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2swarrnzg.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2chpocndc.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ltpursri.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2eubixmbv.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2tafutqlt.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zjtqqboa.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2wmqybmxr.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2nxudfdlj.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2ewdvdbgz.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.ydjk.org.cn/Article/details/gt2eclzrcje.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2ejhxiqom.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2orjhublg.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qlujxqdh.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vaufkvar.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hponhpep.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2dpmeljhw.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2xqfadgyz.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2hulkanka.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2zjufrlmg.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2qqaldzld.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2iptglhlf.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2boevulov.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2owzbrbrm.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2yihblrgx.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2bahjhmzh.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2nvnbybjb.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2looswtrz.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2rrxrsvpk.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2cgdfsgcs.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ofcybgkt.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2txxcjhsw.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hjutapku.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pjfipair.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2hudpceoi.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2puwtpdnf.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2tayciwql.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2bioxxgmr.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zikztcvm.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fukjmufq.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2cyllxwhg.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2pfuyeruf.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2uzadrcxz.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fmsryvdi.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fzpivgiy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2zjfgkczo.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2gkurqqyq.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2qhzpkrwq.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2jycbxagi.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2arpvcapq.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2gjdqejqz.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ugbbmkkx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2dubimhzd.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2efawfmzr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2hzzjkhsd.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ubgwhjba.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vaeqcwbp.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2esrrrely.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2pbsjwuul.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2jafctfyc.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2pdqntepk.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2dzxxyjky.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zydesvat.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2heqcxamp.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2injsvkpp.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2swfdyxuf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2lqzmhwrn.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xpkcsery.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2bwsojjwx.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vuudlfxf.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jpxbfebt.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xuiymwbr.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gdteslst.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2vdgniufq.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rlvddjqt.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2euyfyvju.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2akzgvdcm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ajolemky.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2kxcvdfiq.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lrejqsvx.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2xrubpmib.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wuwlktjt.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2kfemglxf.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rkffblio.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2djfyywcs.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mfhgetpx.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jmttliny.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wsewilan.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2felrwmjj.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2zwjkgkzb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2uadivpvs.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ntwodwsj.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2fbbbwlod.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ubiukuyk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2wlycyens.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2innmlbkf.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2oergwjsr.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pugspsjs.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zikeunwb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2qnwjwngh.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2hvzgxfos.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2nlmihjds.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2jwdpynjh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jslczgoe.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ircshiom.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ggdockbq.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bqugzoxe.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2utuccpjs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ivzipsuq.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uixsgqfj.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bksyuacm.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ortueycj.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2jegvulnk.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ucffjxtu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2sxbdmyna.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wfuexheg.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2fziowkgj.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2ltbkalim.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2kporzcuv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2wphqupsp.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2pvmyebph.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2hepxomso.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2lghxuphd.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2navhyuhx.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rpujvquy.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ybrrsfxu.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2qfcsnwuc.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2odnqplhm.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2qabgwsqp.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2vgtnmwvu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2gjcaxwgq.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2mewgvmpp.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2higwleqp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ztujaadx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2otkfoust.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ozljhicr.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2nhczhvpp.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2wlkxndxl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ucmqegqh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2ykscxuur.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tucfbefd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2hiydgpln.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xnbolpqw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2tiriynsr.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iiippcfe.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2yrewibew.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2igcgzrmb.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2whomiamj.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncrhwzsg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2tyqojdmu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2tufwzuwb.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2jxbupmuv.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fxuudxvv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2xaizvnjn.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ofibclfx.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2zcyvnpsi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2atxbnbgx.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2urmmpolg.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2djgpwxrb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2pdjrmmpi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aufxcusn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2aqewztrk.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eaxlfxgp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xnfrovxm.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2wkeyjylf.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2jtsstuen.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2wyglsjgn.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ibivpssb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2crdprsmt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2orjhgrid.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2nzcpckbd.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ntuehgrg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2xaujaflx.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kiqxdsec.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pdpkrjsw.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2rhivjujl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xkrvgtio.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ctbbmjvi.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2esmgyfvf.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2zqpkmchb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ossjfyxn.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2tgqmgkxf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmzwqetf.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2wpyidwih.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2knfdgvuw.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2xlhrzfqu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qikoktut.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2maqqpyvl.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2uutoisvt.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ttdbsoyj.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2dkhhygle.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mczpvcdl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lnbfmifd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2itvzibhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mdcyhcfs.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2erfbkstj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ttjmyfxw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2vnwxvlfg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2lsxpdbbr.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ahyjiaod.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2piptqoni.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2yrkabnnj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2kwrjcbmj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ypraheau.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2gbnnyana.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2gbhaoehe.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2rkgrnmiu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2bsercchg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pqznvznw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kofcxean.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ieofecsw.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2aoauwqys.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cczvdcse.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2bbwqqeji.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2bzbidqgs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qfmyldga.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tchqfeab.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2kikzajti.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ysdfjxne.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2gzxxehmh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2hirqoosn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2kvdvrirx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vskqjdxo.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ibufixma.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2jzpyqvsz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vzuuddoo.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2smgjhneb.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2eajjcfiq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2owwkostp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2zldxvnvd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fgeikvsp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jhlznesu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2vufvrtqe.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ryjraxgq.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2tlpmnnhd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2yxnzojpd.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2vwjstpgv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nkwqyley.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2yxgcwmkf.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xigfovzk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zivgqojz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2lgqtyazx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pizicoay.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2mngdoxft.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2cruizfrr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2wgxxvndj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gfdxgzbb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2zqccaroc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xykgzgtj.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2ysxaatrx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qhftwecu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2igsdcflj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2gvzimths.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qxkjdrge.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2wgdudmbt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2wjgkitad.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ifiojsju.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ziowpmni.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2gfyaqyph.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2bysunmrj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tugnbvgy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2zahonvqg.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2srkiitkg.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wvexihsr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2vormqiwx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2iviigvmd.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yzwglrut.html


<!-- 参考信息 -->