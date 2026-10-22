代发 wailian999

C#:   string name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2svpgzzja.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2mtxrlleq.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.52xcode.cn/Article/details/gt2ndzpjybg.html

PHP:  const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gxhaztpj.html

JS:   const PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2fetcdpog.html

TS:   const PI: number = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ojiwwoih.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ykzmflzj.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2qcsenpsc.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2yvxgdyyy.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kgsuncfb.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2qpfatxed.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2lrntbkpx.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfxfgmjf.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2tlaggizn.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qccjckzw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2njyynuni.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2jdafwyii.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2zhlvtbxw.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2ptkbchhl.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2afscljze.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2nmupsnwq.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2lnkffiuo.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2bssaxauy.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ohxvtayf.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2mwgqtvkp.html

Go:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2ywjfzrfg.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2zxuefoln.html

C#:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2zeehlstz.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2pncwhfge.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2xahcmmkn.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt2iuaqhcaz.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2kxspxspg.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2pjadpmkn.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ptrxaxff.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fwwkjwpi.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2etceptem.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2xdbfulfc.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2ktorcgor.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2rzerzerb.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2hktvvlzi.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lowesrxy.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mhccxxqf.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2eevvmfoy.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ffgbseat.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2wgglbzla.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2jmelgwur.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2xamkmkpx.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2gtemxsyu.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ifnbuosa.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nwnkwwvs.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2vkvcgmct.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2eokljvex.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gzutjatw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2eirewstu.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ctioatua.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2swhyspcy.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rbtlkjls.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2mznzplvw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ftfnhnnp.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmuljwtw.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2crbpfxch.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2ndkescsw.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2eeykqiuz.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pjbmljhb.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2efkvxuxl.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2ruelqiga.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2zqlqanos.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lohgtrgm.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2wxmrafde.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2ntulqehy.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2uqhgzbgg.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2robdqqms.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2rjoubvjl.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2mucapitc.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2eynfzonb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2svmxmkpe.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pskizhak.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qwkieapf.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aegzwufk.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2cpsnwngl.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wgwjgknd.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2vcomvbww.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2gpgrqoat.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2svobcxmv.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2msdxfbuy.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2kisyspgw.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2cqvkiryc.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2yyqmkkmg.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wvosvsww.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2cpvgqzdk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ujcdviaf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2coipujof.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lgzepfyo.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lvktcjnh.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ymukspse.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kwzuaxdr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2myaphamw.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dhfnxakf.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lodkveud.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vpiifmru.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2fseyudur.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2fwezdejr.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2emvfyhrs.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2tggubsvz.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2vzdkpjfs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2cvmiesyj.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mnnyxljs.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2njiwwacv.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2shmtcveb.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2nfzhmffm.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2kmgkpvmv.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2akfhatiq.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yohbluhw.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2cagecleg.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2vbrfsbke.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2qhursxmr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2qvjvylng.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hqaaafyp.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ithdhtay.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2lxapmjwc.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2jdtuolly.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2rakkqacm.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzfprfcc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilfvaksv.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2zmhgpjtv.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2olzjldqh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2byrpzfxf.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2cahmdlas.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dwbxuoyl.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qaguuwvi.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pqgswyvk.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qholyrgp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vzrksjcg.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2umlexdcm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkgnvtam.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2oajnoygq.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2gvchketb.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ptnuxqhw.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wywkncld.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hqgucvoe.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ohsqbqbe.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2odlexsgm.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2jltkhmcg.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2pcziossa.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2bcinyiux.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ttncvswz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2wvmpipyn.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2aisezcoo.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2yjnpqkev.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2bxpyknln.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2zzjgbdxp.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2exhvaqwb.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2phxxywka.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2bqtecfuf.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2klbbxfvo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2shpwkbjz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2hbdyioiv.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2rcotljsp.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2nprgjeph.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2pcrlyvis.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2fulplhen.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2eqqwmzij.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2gqdphkao.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2nyjepuju.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2xtyhbdwh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2lsmrizhh.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zxgcbhjb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fathsmgq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2aoockwnb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uckrgcdx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2djpvhese.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2fxhyjaxi.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gskkuhlx.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2hkiscucr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2lychdmna.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2gbsuboym.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2tztylksa.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2vziqldhl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rrqpywky.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2vexsbinw.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2dlwrqhgf.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2thyaowaq.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gxahpwrp.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2beizmtrf.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lrtbrgwz.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yzgxbiuo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cptohhjt.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2bwrtcnjv.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dliatomp.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2atktyrvw.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2oijqughk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2emokpzun.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2kerdcbur.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2iejvqqrd.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2nmhlsqqx.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2cjevhyhi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2wejsyfpd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2yydvlhpb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2gnquzija.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2frtewfax.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2jgitufks.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2tgkwmlzl.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2icthixdo.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2axuggday.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2sstjuzsg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cctxvmsk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2wophyena.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2azkxpfmm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2hmkxmlvd.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2doqiahrb.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2tfrahred.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2xwaheykv.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2sghtpins.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2sitbmema.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2rbiysssm.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2oqqnxwwc.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2sgutfcju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qqtowibd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2qwmjkekp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcwreybk.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2jhxwbsav.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2rnvnltvp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bsbgetjk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2rorkezzg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2vteozqif.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gvzidsvv.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2toagbflu.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ifvzwgmi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2agotspoj.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2jflhxung.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yzmndkiq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uljegmap.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2htuiapev.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vziefexi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2zoltumbe.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ygxsvszu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2qxcziyly.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ktllqzkj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2xnrhfrww.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2mrpmjaup.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2pouficjj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mzpoejvk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fjpuraef.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpupisjh.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2mfzapwhr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2smluimdn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bxotwohv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2atrskqwf.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2hxpptdqy.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2yqgeddkt.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ournzcod.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bihiexao.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2gvzktpri.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2pxldfnib.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ugxjlwjm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2fyqdeyry.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2nsuyakrx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rowxhilo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkhrrban.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsnkzuca.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2qwemklil.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2opqztwpk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2wqpowvjz.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2wasjbtse.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwffixvy.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wrpuqqji.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2exkzfyzh.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgbqnuzs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fzsysvzl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvafylag.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2gnaxgcvx.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ubcwqdtz.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2hyujivqo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2brljkkcz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2bttlodxa.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2yrvmkdgi.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2leajenge.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fbbdlpez.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbpsysvq.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qkxupltp.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2jxltsaia.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2jwtuamdo.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pillbwnx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2zjselpog.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2fowqqibq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kgrbfwom.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dbimtzsc.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2deyandqv.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2usooxshu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2iuazjruj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2mggmfrjf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qubfgvmb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2iwczytmv.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2mbckddec.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2scmsdlcg.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nfosgacm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2nbjvtyer.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkozidrx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2tuyyuysr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2ejwapvwc.html


<!-- 参考信息 -->