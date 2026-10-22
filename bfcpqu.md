代发 wailian999

TS:   let name: string = "Alex"; const age: number = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2fkorzple.html

Java: String name = "Alex"; int age = 20;
来源：http://www.ydjk.org.cn/Article/details/gt2stvlhggl.html

Go:   name := "Alex"; age := 20
来源：http://www.52xcode.cn/Article/details/gt2frjzgdqj.html

Ruby: name = "Alex"; age = 20
来源：http://www.ydjk.org.cn/Article/details/gt2qgizgmyl.html

C#:   string name = "Alex"; int age = 20;
来源：http://www.52xcode.cn/Article/details/gt2mpawpgyi.html

[A03] 常量定义
来源：http://www.52xcode.cn/Article/details/gt2wzbdeaia.html

Py:   PI = 3.14159                       # 约定全大写，语言不强制
来源：http://www.ydjk.org.cn/Article/details/gt2zgmflkjx.html

PHP:  const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2gpsdcfdr.html

JS:   const PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2oxrinxgh.html

TS:   const PI: number = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2anxftewd.html

Java: static final double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ukwoxykz.html

Go:   const PI = 3.14159
来源：http://www.52xcode.cn/Article/details/gt2mzyzvzax.html

Ruby: PI = 3.14159
来源：http://www.ydjk.org.cn/Article/details/gt2fmktkojd.html

C#:   const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2tmsccvta.html

[A04] 判断变量类型
来源：http://www.52xcode.cn/Article/details/gt2hjgbmpnz.html

Py:   type(x).__name__; isinstance(x, int)
来源：http://www.52xcode.cn/Article/details/gt2lmttprep.html

PHP:  gettype($x); is_int($x); is_string($x)
来源：http://www.ydjk.org.cn/Article/details/gt2nhczgieg.html

JS:   typeof x; Array.isArray(x); x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2tpbufvow.html

TS:   typeof x; x instanceof Date
来源：http://www.52xcode.cn/Article/details/gt2qpatiobi.html

Java: x.getClass().getSimpleName(); x instanceof String
来源：http://www.ydjk.org.cn/Article/details/gt2vmagwfad.html

Go:   reflect.TypeOf(x).Name()
来源：http://www.52xcode.cn/Article/details/gt2uqzbrrka.html

Ruby: x.class; x.is_a?(Integer)
来源：http://www.ydjk.org.cn/Article/details/gt2kphanclm.html

C#:   x.GetType().Name; x is int
来源：http://www.52xcode.cn/Article/details/gt2suuwqskj.html

[A05] 整数除法与取模
来源：http://www.52xcode.cn/Article/details/gt2znfplbve.html

Py:   7 // 2   # 3        7 % 2   # 1
来源：http://www.52xcode.cn/Article/details/gt2vzhcmrad.html

PHP:  intdiv(7, 2); 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2wlsukjoh.html

JS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2vnjgcszo.html

TS:   Math.trunc(7 / 2); 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2tkumvwqh.html

Java: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2mbivvuzd.html

Go:   7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2nwzvkmoq.html

Ruby: 7 / 2; 7 % 2
来源：http://www.ydjk.org.cn/Article/details/gt2sqqlwlpu.html

C#:   7 / 2; 7 % 2
来源：http://www.52xcode.cn/Article/details/gt2jbgskbhm.html

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2niqetcit.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2pppkrkil.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2cgmxjbih.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt2jelrxecn.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2zscmfmga.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.52xcode.cn/Article/details/gt2qgmqcvuq.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt2jelopcep.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2qztdemjh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2endbtfes.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2rhaswncv.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2cfbwwncd.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2olrsdxfv.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ehzpyfcw.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2saigcpwt.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2vfapxtqc.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2thjnmdyz.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt2ldecjjzi.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2awzaupqt.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2zufouamc.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2penzrvaa.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2vnchbeoj.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2ircqbyuq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2vbdzafqf.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2klpymsua.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2uvbjokmw.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2qapziend.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kavrapuv.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2aqvcnvjg.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rqyoyydt.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lbyzvbll.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iwpqwqoj.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2itmekaqz.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wxxilvcc.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2svqaajir.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2disptvco.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2pvbvjupn.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2copmpfvd.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2rikbzwqy.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2nljlqlgg.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2kkkkmupp.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2faiuymls.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt2amdjmkjg.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2muibgaxv.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt2bzucpsfr.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2fwbwxvqy.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2daftkllp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2wjfzaukv.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ynoiqhsr.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2tuatpdxg.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xcabwuoc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ixkbbbap.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2jozsxugf.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zrxbjtdm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qsvkywpp.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2udrzisuu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2sdxrunuf.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2qdklbagg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2miolcqwn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2thflwezj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ifkqpsjp.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vgwoppqs.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2mhvisbwl.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2ystntxrx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2shforinr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2illixtlj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xqbewpma.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2fjqheqcq.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2igdrzrib.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lrrbuhvz.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xtjsijkh.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hxdsscet.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2luonyckq.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2ogitzfjp.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2bifcxkrw.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2kczulvdg.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2olepxznj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2dopftulu.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2wghotuax.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2fzzqcyup.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2qbwvdvqi.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2mayuitfw.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2pqbpxfre.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2xamysnvd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2alpqndsb.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ookwwpbm.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2havotbul.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2yofihast.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2kuxewlyx.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2dtaunatb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jfpooesx.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2miwrukbq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2qjfahdhv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2cexhbyeo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2frgbcfmy.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2sggzyizv.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmjqcgdf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2iytpetlg.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2xxmecjig.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgozxkkx.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2hqjuriia.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wsxihmls.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2avpegolw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2epzgicac.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2gtmrndjb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2aimcdcno.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2louckbqr.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2spijophr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qsrvpbml.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2bwkvyzxo.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2scuesdkv.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2ipcvvoht.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2ubktzmrz.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2pczfmioh.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2cdsmuenp.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2hwumjrnd.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2iaoeekgi.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2hsjltkze.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2mdxdlkdf.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2gacmmcza.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2pszlscbr.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2tahmwzij.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2jnmcigbc.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2najidtjv.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2ttngionl.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2bkwezqdq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2gwssgsjt.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2birvhsyw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ldjvuuil.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2mwdwgbkj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2mbuinlko.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bjhderji.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2idtmeglj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2lkledzko.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ryrpacwy.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2mjrzcqhq.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2mblsrbtj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2hrzqfurp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gymhpetd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pqlkheme.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2gyupsozm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vgrvtvtt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nndrwrjx.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jfvcvqfh.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ufznubfn.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2lbeafjip.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2xqevngsd.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2mhcfvthr.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2gsxzqnla.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sippaabs.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2mzjhbpda.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uhwhssrw.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2mvasjkiw.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2bmnaspum.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ojudqwye.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ycdezkmb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2gsngjwgz.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zivrxzme.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ybhxrvps.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2mlxolakr.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wjdjpdvu.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bdpbofiu.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2rufkylam.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2saxqdsfb.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2uxoncnsw.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2krflapym.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2piodxkav.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2emhbbuvq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2ntupxoim.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ernpivod.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2gyxieiht.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2vohyksla.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bzfwynzp.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2qulftlhl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xpjajgbz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dekuagzv.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uzprdhao.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2yvxsbdqe.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2aimieihz.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2yeggxkit.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ygkokwao.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2yduesfpi.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2vrjbbllq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2nnsaqchx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2mbhjufvp.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2fszutknj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2leelmyob.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2psukafxs.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2xdwyogoj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2oirfhoms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2umdpbekd.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2vsjxdydm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2luvjnawv.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2mxrjhafj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2znrnxrjw.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2hkhkzbiv.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2ixxapyin.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tdxgjcwy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2icdjcokt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2csosalro.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2pldeegxf.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vrxlcfsd.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kpbgakxa.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2clzjrvpq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ppksspkd.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bgphjiai.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2elfxpuoy.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ycxfvzfj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2jorqqoad.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2ymzcrvyc.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lwmpynaf.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2yhqaxckz.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2cvqhjmsw.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2awblpsnm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqhwpayk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2atmrdkbx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2thkarchg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2fxhlkxgr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2iwzjrtuo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2thqqemte.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bfhxxgot.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2qdddzvum.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gselzdyg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2bwrvjulr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfbvklxg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aohuqxli.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2fdfoychd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2zoogdhpw.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zvekieau.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sxrttnrn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2agsolaac.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2nftokyjy.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2epxwouye.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwywvqtb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vlrcllmn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2liawtqss.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2mcglacdb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2kpbifeyp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2iaizlaxa.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2exnqpafl.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dzgdibhz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kmbcvamp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2otqahkzy.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfipsbaw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2bdkzxdzo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ijfzwtpa.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2vnjznpiz.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2nzwrllhe.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kcjafwfl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2xjwsitgd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tipkbleu.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2rootksgp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkctxfvk.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hghstuak.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2uwbytluj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2dtewrhiv.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2ewepfpas.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2paszxveo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fikrawyp.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2siohjhcu.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hjajrwzm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kvufdzbm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ubcfatow.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2ajnqzedu.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kgayeaxn.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2jtvlrrsn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2uupuqhqk.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2yafwjemm.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejnrgpec.html


<!-- 参考信息 -->