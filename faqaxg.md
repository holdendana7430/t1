代发 wailian999

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2ifcedssv.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2qyhkhzmh.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jisqzibq.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2htycpduq.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2qokpvzpa.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt2tpmgrdoa.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2arogdtsm.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2giwufquy.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzfarldv.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2qloncuzq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2uazmegsj.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2ubvjcznv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2mnbxdzeo.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.ydjk.org.cn/Article/details/gt2feysgich.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2zwuiltcg.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kinbsbrv.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2sqhqpjip.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2iwntwaxw.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2htkcyyif.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ntsswxhj.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2fgjtjfnz.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2rokkzfcn.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2cdjextuv.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2xcakgmgk.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2prjgvrwb.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2pyddhcpn.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2wahlzlzi.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2atnpnexf.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2siycpury.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hexgtkjd.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2uvsjhbyl.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2llatylka.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2kqfbvaob.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2acytzitt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2zxscdmrr.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nqtrkrrt.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vcvnvulo.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2yphhjjss.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ydsphpur.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2sckcijjo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zfxgnogs.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2bxurusmj.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2imoalqgm.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2fdhkqhnd.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2jmmvtjlg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2vjkeqkrt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2szinxxyb.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2anbidyjl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2kwejodvj.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2zayedriu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2xnguwxzu.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2lbmrvysw.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xwgxavlw.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2tyfqiigf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vpaugtjp.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kwvqxina.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zrggjlpf.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2lcdjedzw.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yggxqguu.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yllcpupi.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2dzuqafkb.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2krimmfhf.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zvzoujjv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2hdwboxfz.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2iusbmspk.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2qdqcziko.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ffoliixl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2yhwykrxy.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2lqcxvxgn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xipfeqbv.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ehzwndwl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2egyllxlh.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lgvgbjps.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uzsihrnr.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2ajubnnnb.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2qaqlceln.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2obsymgdr.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2psqecomn.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2fdrjkrrc.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tlajvocl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2txgzkdlo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2txrulmox.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilbgbcfm.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2nmfbpczo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2pccewmsl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2kxaeeukz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhtacjrq.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2cbwwidny.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lgortsbt.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2pvqhnetc.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zvwcrntg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2wdwckstc.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2nyrnhkwr.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uzvllhfw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hxzfagih.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kiffinrn.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2dyuevvfe.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2pnlrhiru.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2wzavtxap.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2yrtolddb.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2hpnfrvpj.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2qkfuwhuy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2fwtqghfp.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2znlhryrf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2klxojfhd.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2vwwmsxld.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2zouzgssw.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2jprlkode.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2pegudcvj.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2aipwzsnf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2pugwzeuj.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2flzusewv.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2udsdbhxd.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2hqncdrju.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2ksesahvq.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2lhdcsghm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2dcxramvn.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2mfkpnagz.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2uuiusesa.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2bruxwqae.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2ltwvcduk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2ohjrcmfw.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2fjlajcmm.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2uvjnuzhh.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2ffehbqui.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ssmncnwp.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rtxcllyt.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hpisgkgf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2twrdkqbq.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2dpwfqvfm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nhgtpqvp.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2ygayckdk.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vktekhxs.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vkejplwv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2cfxaktoo.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2snktsfwx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2mlmkwkkf.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wpifqppz.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2amicajyr.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2zaiwqugh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2kjjjivxs.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pohaaylc.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ihqgnfeb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2tjgsfbbi.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2dplixjxc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hykbosjo.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2gxamqrjy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oluxnaed.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bypazzjo.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2qgieudfl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2tcpngbkh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2cfgfkapk.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2thqgqzir.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kpgajhfn.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kzjzsqdp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2nfzgfxol.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ykuzolmw.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2acssspxn.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2byqreemn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2atmbkzop.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2ewukizoq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2bqsurebo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jijlxqgg.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2hzeablgg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyrszfsu.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkhskbtx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2qtrdmvtm.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ozbaimym.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2rmkjlsoy.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2zkuzrqsv.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2mtgrysgq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2cyhpaxni.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2wprbpmig.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2xhtoopym.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2iraipltn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2vfzhzmuw.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ccrlboze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cxzhzwjd.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2ikudurtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytkjgyde.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2silmedip.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ziwaoxtd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2exxipidf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2cxixaynw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xipdpfcl.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lvmkkkcb.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2pbptipsj.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dhwmegtx.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ehgdpieu.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2oaeptkqo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2uqbwgkyq.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2cgvtswbu.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jydtybqe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mgkpzecp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2xirchydj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2vbpjdqrv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2rlehgkxh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2leoxbqcq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2fvfaecvx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2ivpxgien.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkqapkus.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqsrgnnh.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2dusfebvz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xxuazwnf.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dqkqzyzn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2oorlfjdd.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2byazcbfd.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xniptbie.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ybgivuod.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjychfqj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pzocdvse.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwpcdofw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ymvqwrnr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2oixydxdp.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ylzxvzde.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2xoygfgkg.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rckefnjb.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2tvnqlypr.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ketjjage.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2iafvrixa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2hboxkhip.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2dtmfdoch.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2skpmdfnc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2kvynccad.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvlmfzwm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2ubjkrrxb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2uykgnlbx.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2mxophnbk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwyamrjm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pyackoww.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2asvlhnaw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2exvzfcep.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2daqarsag.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2svrdxfkx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2gzpkjzod.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2smdnyzix.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2czmvrqcy.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ejbskqbg.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hqrdfygk.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2kgqvdjxj.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2tkcsblxy.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2pdybilch.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pnevctav.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2pytywlqk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2tvrjehij.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ntbopcsv.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ykffvddu.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2baxjjlyy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2luvfshmq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2obqksrsq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2vfvbfysa.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kxejgzfh.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ocbzqyqn.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2jzlwyfyy.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxxsybdh.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2touqfksk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyunemgg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2avlcgpdn.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fcvkmfbf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2daiviavj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2femixwxs.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2mlfinckl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ifzclipa.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2udzokcjs.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2myldczdc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2eckmuyaw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2cixxeojt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2oqurwjbf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zslaiomj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2grcosnlf.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2tqmasfxk.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2efzitous.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2acwwhufn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fqnzxejf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2awxjxbps.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zscifjnf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2svdcamvf.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2agujublu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2ppkkhgcv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bjkxzuoh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2vdflcfbv.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rmhqpmmy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kihjnfde.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qwdzdoyy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iizgeito.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2nbpuequh.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2pgbbpzif.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hgnxyulj.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2xttedaza.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2njuthxbs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2tglbbaeo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fdbfosqf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pszkiwmw.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2ivwziftf.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xpvbabro.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2akepyhsr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2crsvtooi.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2grnwjmxy.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ylrzyzcl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ylmgtvcb.html


<!-- 参考信息 -->