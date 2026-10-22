代发 wailian999

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2dnqbzbew.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oiypodfm.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tozrodig.html

Go:   const PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2yqcswctw.html

Ruby: PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2rpbnkfkn.html

C#:   const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2zooebzff.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2efgquzrn.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.ydjk.org.cn/Article/details/gt2mumhjnge.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.52xcode.cn/Article/details/gt2ilebfsis.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.ydjk.org.cn/Article/details/gt2cwvpizxl.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2rghwimiw.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.52xcode.cn/Article/details/gt2lnhzklxk.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.ydjk.org.cn/Article/details/gt2rqtroqvy.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2hrdzdkga.html

C#:   x.GetType().Name; x is int
来源：http://www.ydjk.org.cn/Article/details/gt2wosyfuuv.html

[A05] 整数除法与取模
来源：http://www.ydjk.org.cn/Article/details/gt2ettpacnu.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.ydjk.org.cn/Article/details/gt2jilweeer.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qzloqrcz.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2ampvkspo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2dyjpexcy.html

Java: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2hkyykpsq.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2wbvtfivh.html

Ruby: 7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2uidrunpb.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2qyonoapi.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xkaggtbj.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt2ihlxklwp.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2xyeaacsf.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2gtzomhqv.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2usxutdta.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2kvmfasxz.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2htsgywaj.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2drdwwkrc.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2jljqftgu.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2pzeqdbnp.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2ztpzdrhq.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qhmenmpw.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2eimtzubs.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2gimodbba.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2bvhgbsjh.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2wfozaeky.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2tgymjjzg.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2ezovqqpj.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2cunhydeg.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2pwlbkiqq.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdnmdzob.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2rcdlfzfw.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2ypqbdkjl.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2vblepvlq.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2gkcjtvre.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2dttdjovc.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2tgzhjmvj.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2jwbmbucn.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xsvktfro.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2miiailbf.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ndcdtkik.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrsoahqg.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ieknuaog.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2ghmtktom.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2hdffhadh.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oqpdzjfr.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2wxfchfgr.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2gtwhcxpv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2ixqjzsij.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2mzpgcdbn.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2lnfnsunn.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2onofzsvg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2wphsgnjo.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2tevvbvwy.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2ybvzdguc.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2sauoblgb.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fhbjfigk.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2lkgkplom.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2seosvinp.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fzenfxwp.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2mxwokfmz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2lzvjhttp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2phzewxfm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zcwrvoxt.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nwgruxnu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ghyvezwq.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2sjsxavjt.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2ctsgfxyl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2fbuzoepa.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2qgzytikv.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2lpgzulap.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jmudkvmh.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2dmytrloz.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2zommfnri.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gjmatuns.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qdcmhnut.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qnozpxls.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ehigcaik.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ijrrjbel.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ttnevqub.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2thwjhfim.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2palcbpig.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2bhpulves.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2fetcmnfx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2eaipbnyp.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mpcbdyph.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ctsfyzhd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2rmfwaate.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sabwcvxc.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2rkcvejne.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ubkvhhau.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2bvsqmloa.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2zopmegmm.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2eqyopdaz.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2euguymvl.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2namzlyei.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2ykuuuuzg.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2allkkaop.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2yplomrth.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2hzuagxog.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2nxdytwwy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2nratbvlr.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2sygpgcbv.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2qjtnbfcj.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zigwngge.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yucmckgb.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2ydrnlayb.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2jitarvqh.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yvfohxfp.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2dexiucfl.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2plebxlqh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ssogeaun.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zgmqzget.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fdoyslgu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xtmzersl.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ilkaztka.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lbzavxpo.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ubzsvkwv.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2qiooicfa.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ebilhvky.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2guulmbjn.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ezhggnkd.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fzithfns.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2nvqfekze.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2rswogiok.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2rtdcfsjp.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2uwzitemu.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2xonvwwgd.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ykqsrhfi.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2udlfexrz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2romlrmgb.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qxfrjbdx.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2bvegcszi.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2wkysthwg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jjwlmowo.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2pwplpmxy.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2zrlgbcgw.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2ldssdljp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2exnqhvlm.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2jqdxmqrb.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2zjwmnano.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2hijoalgc.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2qhhbmwyd.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2bphjtraq.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2qjilglaj.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ymkubvyf.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2thsibfwm.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zgjuwrfe.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vpkgzhjf.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uotlkczi.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vaialdik.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yexjzery.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2swyzbtdi.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2qrkklocd.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qkbsqwst.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2uxasbcjo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2dyabohqw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2zwbyzydz.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mrcigtoj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2zlitnyxm.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zxmbfozz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2ddzotlax.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2enrghhge.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gorzwkor.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2ipeenkbr.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2ewzrgypc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2nolxfpcq.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2obiffcvf.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rlbunqen.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2mfxjlhcb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vupocsoz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2zuoguqlx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2gwkgyrcp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2rtoxlpiz.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qstbhixm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2msqvjcvz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2rtrknqwk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ymepkpdz.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2deeaxthd.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2hujyiebq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2fqnkpmhs.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ajsjqamf.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2phtkzzpc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2ihhgbhze.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2wnvmomnw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2wkzluvxm.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lrqiaiit.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2sltmddxh.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2socqpkzf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jeovbexi.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2twpwxnqu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2mbzwxjed.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2dxlzzqou.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2omhzcogw.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2zokmhttr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2kgikgghv.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2zmwnpspw.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hocbmnyz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2uttuqwgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2flxvfxuf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2xribqbju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khkdfeou.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lcgdvzjh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ashtdffz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2flkqejyj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2aalsefwi.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ailrasjd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2cnpwfboi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2rnkniugm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2fcdzaxyk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hlivuemg.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2rjhtupls.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2cpjgynay.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxihnoyf.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2todhpjpd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2btsizzbq.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vzuudcry.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2yqupzbil.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2saucnkxc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2inmdwbpp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2umalcacv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2xjvkzvag.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcpowpnv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2obzbluyb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ywzgjqlr.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxxvgjym.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2epkawwjj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2sxyjsrhb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2bdyceakc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2baqfrntl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2yepnmrry.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2bhoqxmzp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zlqfqptz.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cqzrpmpa.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cytoczwz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2cvsntwyy.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mnxbiiky.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2tjmgvtnw.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ugmrtmki.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2rcwbgyuv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2vchbgeto.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2oftcoohd.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2fcokfwmk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2ixxhojyt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xsscrplq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2ksqorbdg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2bccgbqmf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2trrkstcf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2hupcaqyv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2fpnwvmew.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qonsdsul.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2jsvikqyx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2pguuxucw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2jypvonxf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2bkatvgmy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmyaaahr.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2gigxyyeu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2vccgkzsm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtlueplc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2domlpcgl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vytvhwjy.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypizodaj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2uvkixgla.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2rzgqypbq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2drwkzkqx.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2cdpruvef.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2josmaufx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ngeacvgn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2sngxjupe.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kptwnmgk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2duitvfsx.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2gkdkwawm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2xtdjosqg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jmrfycsa.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2elqtjpmy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2anaslmuk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2qyroibbp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcfeqaeo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2hpegnelo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fqxqcagc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2dhxioetg.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2qbfkhtjk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2siyyktst.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2uwxipghs.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2sgkmievd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfifcehl.html


<!-- 参考信息 -->