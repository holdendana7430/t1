代发 wailian999

[A06] 字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2yhmlvkif.html

Py:   int("42"); float("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2kdvtymly.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.ydjk.org.cn/Article/details/gt2livdvjct.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2ickdsdem.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt2cggxcsui.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt2bhftcgkv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.52xcode.cn/Article/details/gt2pzpnepmd.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt2rqmoatgh.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt2lvupxqxi.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt2iydqtkfb.html

Py:   str(42)
来源：http://www.ydjk.org.cn/Article/details/gt2jctzizvo.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt2ahmtdwyb.html

JS:   String(42); (42).toString()
来源：http://www.52xcode.cn/Article/details/gt2vrtiirji.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt2wzcxrrvg.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.52xcode.cn/Article/details/gt2gikucqry.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt2mirqjrzs.html

Ruby: 42.to_s
来源：http://www.ydjk.org.cn/Article/details/gt2fwaimcug.html

C#:   42.ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2odepzgdx.html

[A08] 取整与四舍五入
来源：http://www.ydjk.org.cn/Article/details/gt2kttfetek.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2obchjasa.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt2palvycly.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2udltklil.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.52xcode.cn/Article/details/gt2aigyeisk.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2jmajvxcn.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt2fpfaepnk.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt2mhijsbte.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt2qjmjvdkm.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mmscxkvb.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2idtnkcqz.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jcnxuory.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2soxguuhi.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2aqelzczb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kngkmjen.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.ydjk.org.cn/Article/details/gt2lrwqkosh.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt2scykcfof.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mbinwdur.html

[A10] 生成随机数
来源：http://www.ydjk.org.cn/Article/details/gt2jmbvuzbb.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt2jasvfnrv.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt2hahlexia.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2hxhsdnew.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt2purlipbf.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt2kxzzyvkk.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.52xcode.cn/Article/details/gt2tslfulnp.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt2gtvwnuto.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt2rrkmkkcj.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2cdacboat.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2ljvpxevp.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2witxbbsa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ypynoscx.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wdjuopxc.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2redjdual.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2ttdsgunz.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pgdlssvh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2diusqypw.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hqwkfrum.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2erzvmqca.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2ykkjwyxd.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nnpnkzhm.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2hccyzyln.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qqidcrfc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2brzrwlji.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2izqdcmfb.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2kuhmuuab.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2fxlxiwbv.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2gqfusciq.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2watlphjz.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fltmaxkn.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nsyuitoj.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2nhaskctk.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2eqmcywgh.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2fyhkpizl.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yrjtdjdo.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2zkgmjxfi.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2abkhmevx.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wstdqtwg.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ngdbaebh.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uuxfjdke.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2udqfvqmg.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2xzlolmhu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2uvvqdipv.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2txiertfx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2lhidwagf.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2aywvciqq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2xqjkdfeg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2brkcxvqs.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wpmpkpcu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2wtwxzmah.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2eujkkyqr.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2oojpgtvx.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2ymsydzuk.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ypharrsk.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2npqrxeki.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2fomvwlsh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2gqtbvhus.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2dskrikec.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bryntsjg.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2bspkkrbe.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2nqjplbtx.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qburfjxj.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2iwarvpgh.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qpgzdhci.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ylcejfpy.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kghgcjni.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2tsjilekq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2cjqqdwrp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mjefhqdm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2gluqzszh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jjzacxrq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2xoyoiqas.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2tjbaxcyu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2hmqtgzra.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2cmnzuxtw.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2voqvxzsx.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2ziqsuqxf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2fbgegbxk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2vjkgrywr.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2tnlimhly.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2ivnwybyk.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2etnzxkdu.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2ylohhpbz.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2aweodbuq.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2bfdlatfv.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2azmtstto.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dcasftjd.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2znyqcuki.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2icbdgnbd.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2jykpfeif.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2tdqltpjf.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2aprqihop.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2xznyjznc.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2tpxlgtji.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2vsbycecn.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2rajvlokj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ceywdirx.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2fkpwkaqw.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2ivesznag.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2mncgxhsp.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nvzpykhd.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2nhlgpmko.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2aejbsnlx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fnkjxelm.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2xjkcdazf.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2gsuxbvdm.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2nykcyfxl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nltbduym.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2ymgjftrk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2jxiisvkd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2anlhrcqt.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2aaohkslo.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2eberflpk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2hhnoinnq.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vzttoqzo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2eodmgebe.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2kyhrtbch.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2lrteldsb.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2xyoljhap.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2cuhpcryg.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zhshwhjb.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2zugwzdbn.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ldlihryl.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2uzbunbux.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2xqsjrylv.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2mqhwfriy.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2vyeyhtwf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2yuyjxpss.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ifscskfj.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2omwxhddd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ktufgnpc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2enbsgrzk.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2puxwxuaf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2zzyztnrl.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2utrixkre.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2fzcoevsf.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2oqdxeuko.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2esjsqgje.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2qrzzzfhq.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhounoms.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2cmlugtkc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2xhwwlmsq.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2txtawnkp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2uvlvgjhe.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2hzyewgda.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2bowpitcz.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2jpernvzy.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2tuqidetn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fszpjvju.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pdgpxjrn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2fdztcyod.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2umemlcmw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jragydka.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2bnufeoov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwdkfetj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2kpoqncta.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ybpvnuak.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2frkbntwl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mqdxtvvm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2nwtbxjhw.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ljlehlmi.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2cjxuzeoc.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2tctuqike.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vsjpcuwh.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2btzkiflv.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ybmpeuzt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uapwpnuy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2gqgwrszb.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vgtppjbs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ocnzolym.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2zafltqtv.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2wvazmvzv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2pediwxyz.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2yjqoopun.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2zpovrzde.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tvcqbozn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ibonqsew.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2asykkxcb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oaklctjt.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2darfwmmj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2xgytuvds.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2espiouyg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pedzzdrw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2cdifejew.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2agbqcmgz.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2crcmcskm.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2vaesouve.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcsvyaxo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qviscjxz.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2odisadep.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2psisdepn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2srerohbu.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2vtromcgs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2bszlqoyx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjyqkttk.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrrcdbui.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2afrhipzm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2dtsfnnqf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xubxnyxd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2ouyioyts.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2yjseghvn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2afxlrzzz.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2htwwpwlu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wwmpbgcm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2yfokdykm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ityeihyv.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ncsjkavk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2sluxjseg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2xgswrcdl.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2mjrjvjvg.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dnuujqpz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2cxmpofff.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncchxwsq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mqhhggwd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2osofychn.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2dunrcaov.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2kwarsybj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2scbpipzs.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2xbsyvpdy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2pfvbvjvk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2esxlpgsi.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vjnycptw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2inhnetwd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2egzimnuf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2cdwwemtw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rbemswxb.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2httsxpxs.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2urukwyxi.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2povpluju.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfiwwsfy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2exkodbtq.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxhahmmq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fbqbqjmz.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2lufiuwql.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2usqnlrgi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2aldunzbx.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2nlnujpql.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2dwrzzivi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxfmjopk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2juhjmruc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2jyjrwcmy.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktwpuriz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rzvvxlxq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2lkjdcxaj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2gpqzvevf.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2swfooqfo.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2hpdfetfa.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2cobwwadt.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vqrfykle.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yfmjvshy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2fqvzpbcu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2nmspetvl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2mvandpui.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2kieonpms.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2neuapkux.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2pgneflod.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2zvtmaors.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pfiblklw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2rwlejaum.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2imazoceh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2wfmecqrq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2vuxxjlht.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2dddpejps.html


<!-- 参考信息 -->