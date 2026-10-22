代发 wailian999

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2tybjtzxm.html

[A07] 数字转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kxxvpnym.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt2srabwpzn.html

PHP:  (string) 42; strval(42)
来源：http://www.ydjk.org.cn/Article/details/gt2qmameoxt.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qywtexjd.html

TS:   String(42)
来源：http://www.ydjk.org.cn/Article/details/gt2kztkgwob.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2tysjmuah.html

Go:   strconv.Itoa(42)
来源：http://www.52xcode.cn/Article/details/gt2frepapzg.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2whbgrewr.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wfanwdxv.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt2vaikdqez.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2dtogvujk.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2ctpvnjpy.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2hjapgxoz.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt2gxvowpfx.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2kyxkbltv.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jqjilvvu.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2lioepwrm.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2nigfjlid.html

[A09] 绝对值与最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qcflhjly.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eaafhmhi.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ttuiwbqu.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2ytiqwaku.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2katcojzr.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2zklkgzdw.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt2yvyqoagr.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.52xcode.cn/Article/details/gt2swlzlfnu.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nldbezlq.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2liwfezca.html

Py:   import random; random.randint(1, 100)
来源：http://www.ydjk.org.cn/Article/details/gt2nwbzurws.html

PHP:  random_int(1, 100);
来源：http://www.52xcode.cn/Article/details/gt2sarbtpzl.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2zsdpnylg.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2bgcchbbc.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2fbukzrtb.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt2zoemjhzv.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2yandexvh.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2soddohmn.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2ncrvaqjm.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ebjpawbz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2xjhtcvtx.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ligfnjeh.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2zedwmunt.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2aabhnxzr.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2gttiyrlp.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2yhpteqrm.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pntomxig.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2twntgshc.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnjoztms.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2ufaaicnu.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2rqxbzfnt.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2lrxoufju.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2ninbfzwa.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2gkqdxyba.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2pcrrkmjg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2lteedtds.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2mhmmhnpz.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2phgklpdm.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2amshzxal.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ncuhqnkt.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fnawkmce.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2hxtctwzu.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2tdhxvrbg.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2cvqeckpd.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2anhvvkyf.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2nulhvtbq.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2kzzsecgm.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2nxenhbfn.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2qsendayp.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2doaithpb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2rrxrsbzt.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cauqudhx.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2iqtalcvu.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2seamkcuy.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2hmadwnli.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2gmanjlhl.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2qaonupvk.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2dsksuxlx.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2oirscvfl.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2xromrogk.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2azqemdep.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2kozzfffh.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ujuzmfio.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2otdhqvyy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2khbpbisz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2uipyuseo.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2mrvlsurh.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uryqnurq.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ecleqgnc.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2vqnkvocl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2whfmsqdv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2rydvmccm.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2qtqyjmtq.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kdtmmsvh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2orhgwktp.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2syzswsnd.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2sbfjenop.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ktzueufm.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2imynzwzo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2clumivuk.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qutysekp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2rheabsfa.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2yzpqfqzy.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ystxgjnr.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nqcxswcs.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2yykwekdz.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2qnnywyqs.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2qfylrfia.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2uyzmhjxw.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2bgkoybcr.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2mgcdsjoi.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ghjpwtwd.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qvoxddeo.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fdvcrlms.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cjbuwmgs.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2cnokssck.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2pjqlirbk.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2xyobipdq.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2fzbghqko.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2agbknchl.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2yaymtthk.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2tzquzyga.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2cmoxuzup.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2ywsqwyka.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2wbsjicxv.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2jhsfudqh.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2jtxekrih.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2rufmouxa.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2vbbbjfye.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2pwhecgma.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ophuqguz.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ytnwcpsn.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pbangqfb.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2amhtannt.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bssqczts.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2yrozveic.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2jqeslhyd.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gnydarsw.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2yjxtcswp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2nqgzhwaf.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2adomuqac.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2zrqumwrs.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2brvnhyhr.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2ilfiplid.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2keezvnif.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2wiwcxies.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2olhrtnzf.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2pndatfch.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2abvofpvb.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ykzhkwqi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2tcyygtqv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cmfnzfix.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xvkdaboy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2afhfpvtn.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2itqyssks.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2oqbyucnn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2qmwvjbts.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2apfxglha.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tuyjiotl.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2dvqgzqgf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ofesrsat.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2yavyltfg.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2mbiikhcl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vwoxjuno.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ttylbdyy.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2nmgpudvw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2apmlnxlu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jkyojzym.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hitjiihn.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2uxgindgw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2caukijtl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2pxnjfsfs.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2bdxqmeus.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2kpqulzeb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2wqwifftc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2miwrwdnc.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xutwnhvi.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2fnfvhymc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2dxhblkkf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2jpfvwixb.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gkhkmjcr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2sxytbnwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yrlfqpem.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2zzyehyxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsvreqyf.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tbnyieke.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2buioldnu.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2czuvlbwh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bpxfjluw.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2himtxpsz.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pdxjmoxu.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2aagqsgnv.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2whgxatun.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2erlsiffe.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2applqfsp.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2disgqigu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2whtyzzdg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2oglfkfzb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2lrsttxdj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2aysuqnjg.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2pvtcmwii.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jophwipd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2txibxptc.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2wtgupwtv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2wbmojlsv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ppkddhes.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzybfequ.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mphljlyd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2qpmfjaqe.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2zfkdfcwm.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cbgwjdwn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2yodabamh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2teuzsopg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2tcgrckyf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2vkhvqcma.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2oiaywpfl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qxaqzvfz.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldbnfphu.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2inalumpd.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2syjhqodh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2grsorqsv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2gpbfdnly.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2beqolmqz.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykpxqnzv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfyicuzt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2llmmtsbp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqlhawob.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2uwgyxhys.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2mddwvqdd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2mmniejyf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2jayxjupc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ohgapcba.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cmiqcpcj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzgqybzi.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2niekvfdf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2iwrswkxe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gjzppgyh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2qjyserhd.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rfqbuxjg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2qdgjaazc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nlsaymly.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2viutowjm.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2etvfafzt.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pfrjosyo.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbyeotfs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kqczqhvi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2kgtrgdhs.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2upxezcvr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2vupiizwc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2yzlzuusu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qbtnhpxp.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ddegufoy.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fgnuozcr.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qfqmmpyr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2uwzchmwu.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rwxxgewl.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cgrbgluj.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2quxzfghb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2dayxraot.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2znigbhiu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2acctldfi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2imuoouis.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxmgnmsd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zfewuroq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2bgqkxmiv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2opgqyngm.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2iicokyvh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2fpjxotof.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2rlokadgl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2bcyzqvmw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2rjyepepm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2inovepic.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2kmeedfwe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ndjiordb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2xdjplupp.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2zxuswidt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2gbmkgupq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ngzzkpak.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qrwvafft.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qqilohoe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pvtbyzxe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2upiooqof.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2tqdznvdt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2pijbokco.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vgglqvwl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2ugmxhfnj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rykbgncv.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2novitfvz.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pqetzuvc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2gxjjcrmf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2famzmfcz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2umhkruxa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2hquyejuq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2mvxvwrea.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2xcihasyb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2dgsstayl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbvobxwl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2nvztauuj.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2pwoblolt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2avvcibjr.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hexvrrxv.html


<!-- 参考信息 -->