代发 wailian999

[A06] 字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3vcnvmixw.html

Py:   int("42"); float("3.14")
来源：http://www.52xcode.cn/Article/details/gt3ogdipbmc.html

PHP:  (int) "42"; (float) "3.14"; intval("42")
来源：http://www.52xcode.cn/Article/details/gt3uspttdiw.html

JS:   parseInt("42", 10); parseFloat("3.14"); Number("42")
来源：http://www.ydjk.org.cn/Article/details/gt3jjunmyri.html

TS:   parseInt("42", 10); Number("42")
来源：http://www.52xcode.cn/Article/details/gt3kafbqyxh.html

Java: Integer.parseInt("42"); Double.parseDouble("3.14")
来源：http://www.ydjk.org.cn/Article/details/gt3bdxqfubv.html

Go:   strconv.Atoi("42"); strconv.ParseFloat("3.14", 64)
来源：http://www.ydjk.org.cn/Article/details/gt3iyznwule.html

Ruby: "42".to_i; "3.14".to_f
来源：http://www.52xcode.cn/Article/details/gt3fdpnuhfv.html

C#:   int.Parse("42"); double.Parse("3.14")
来源：http://www.52xcode.cn/Article/details/gt3yrrsemzt.html

[A07] 数字转字符串
来源：http://www.52xcode.cn/Article/details/gt3ebvxwvjm.html

Py:   str(42)
来源：http://www.52xcode.cn/Article/details/gt3cugbtbmm.html

PHP:  (string) 42; strval(42)
来源：http://www.52xcode.cn/Article/details/gt3ztxalzlc.html

JS:   String(42); (42).toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hdwghkml.html

TS:   String(42)
来源：http://www.52xcode.cn/Article/details/gt3kuijgxzy.html

Java: String.valueOf(42); Integer.toString(42)
来源：http://www.ydjk.org.cn/Article/details/gt3allkgach.html

Go:   strconv.Itoa(42)
来源：http://www.ydjk.org.cn/Article/details/gt3riawuizl.html

Ruby: 42.to_s
来源：http://www.52xcode.cn/Article/details/gt3cnuxpcxi.html

C#:   42.ToString()
来源：http://www.52xcode.cn/Article/details/gt3krqhtjqt.html

[A08] 取整与四舍五入
来源：http://www.52xcode.cn/Article/details/gt3ohdswmlb.html

Py:   round(3.567, 2); int(3.9); math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3fuigwxdh.html

PHP:  round(3.567, 2); floor(3.9); ceil(3.1)
来源：http://www.52xcode.cn/Article/details/gt3dxkfxvme.html

JS:   Math.round(3.567 * 100) / 100; Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3qypnnpoq.html

TS:   Math.floor(3.9); Math.round(3.5)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvcbgxs.html

Java: Math.round(3.567); Math.floor(3.9)
来源：http://www.ydjk.org.cn/Article/details/gt3uzftbrid.html

Go:   math.Round(3.567); math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3mjazrqdm.html

Ruby: 3.567.round(2); 3.9.floor
来源：http://www.52xcode.cn/Article/details/gt3drvlhakg.html

C#:   Math.Round(3.567, 2); Math.Floor(3.9)
来源：http://www.52xcode.cn/Article/details/gt3jkglieba.html

[A09] 绝对值与最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3nrlzbqxr.html

Py:   abs(-5); max(1, 2); min(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3saghycgh.html

PHP:  abs(-5); max(1, 2); min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ndxjvlnj.html

JS:   Math.abs(-5); Math.max(1, 2); Math.min(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eonuvhyo.html

TS:   Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3auvqxodb.html

Java: Math.abs(-5); Math.max(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3oyardzoq.html

Go:   math.Abs(-5); max(1, 2)          // max/min 为 Go 1.21 内置
来源：http://www.52xcode.cn/Article/details/gt3loikynog.html

Ruby: -5.abs; [1, 2].max; [1, 2].min
来源：http://www.ydjk.org.cn/Article/details/gt3jmcuigut.html

C#:   Math.Abs(-5); Math.Max(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3swtfnwsc.html

[A10] 生成随机数
来源：http://www.52xcode.cn/Article/details/gt3rtamdmxm.html

Py:   import random; random.randint(1, 100)
来源：http://www.52xcode.cn/Article/details/gt3tjypushz.html

PHP:  random_int(1, 100);
来源：http://www.ydjk.org.cn/Article/details/gt3kttbevmr.html

JS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3jmuvdczh.html

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3pblpoohf.html

Java: new Random().nextInt(100) + 1
来源：http://www.52xcode.cn/Article/details/gt3ghvkbowu.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3tymatcfe.html

Ruby: rand(1..100)
来源：http://www.ydjk.org.cn/Article/details/gt3fpzdjzba.html

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3pzubocaa.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3zoixoyco.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ccupipjm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3jsrprogk.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3udrxlslu.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vdhhciwj.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qwadctkj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3ncveojsb.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3cixwmcbw.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3xldjciyz.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3iboggicz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3zhjbnzwh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3ttnahriu.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3wdafbvhu.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3hozspjjr.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3idgcevbi.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sqjomhzg.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3jkdyrznk.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3xviungsl.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3cawbvunr.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zacfieaf.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3ospmhudi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3jmeqwloc.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3vjqawthf.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zgvtaayb.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ekbquole.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kpzepybf.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3xiuoeoev.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ybvhqcrx.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3ytbqwhan.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rompurlw.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3mwsxecrv.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3lpuekjwd.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3lufwxuaj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3cfltcqxu.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt3thtepfef.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3jsohdbyx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3xyacaqgs.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3rdatdoee.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ppbsnitb.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3unvonmsj.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ndxvjgmi.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3cpjixmtq.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3kdxtbyru.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3xadspqps.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3ypzvdomx.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3yoamndin.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt3bqjghlnv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ljyuydse.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt3vngqndnq.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3xqopvcop.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3yeeqbeid.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3qknmfcxy.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt3nzvpzpqt.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mtumswru.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3kcoqaess.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3fpenveep.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3smwpbeoa.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3fdwlepnn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bqqyaztu.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3bfngcpqs.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3pnvtbdrm.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3tpbcdsop.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3hotcailn.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt3clekdsjv.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3tjoyokhc.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rxmwlbce.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3zjevuhsj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3hwigrzym.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3oumtxagr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3ftwrkhza.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ksivyctv.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3uinoqxra.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3cdhttbxc.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3vyrlnvtt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3rqpkssel.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3rthmcirv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3ungcjftd.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3ysyqamoi.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mbmanaev.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3xciitodq.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3qoviuhte.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3vazdmpfd.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt3unwvyuxn.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3jmvoehgi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3mevcnikm.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3qhnbrkem.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3efplwbeg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3aeixabfp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3kfzkfzgy.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3rxnrjvse.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3ewtitwtq.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3dibmnbbe.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qmnzsrzd.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3esdmqvvk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3iiwifnqp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3tscxthsf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3zysgossm.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3nnjjdpow.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3amigsehy.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ippjwudc.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3urqfnwvi.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3udbjomxd.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3psufwrrm.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3taycrfko.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fozinjnv.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jesbvnbw.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iqrzvvfo.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3vcflecba.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nkoacuoi.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3bqeprlku.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3ljjjnjve.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ndfccscr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3crtkbrlc.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rwizektb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pruvyndn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jlvuanpd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3ysqcxntr.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3peficudk.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3cwexxazy.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3nsaronoa.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3mbqytqzk.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3deyqpvbf.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3abdoukvb.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xnsmahun.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3yljidzjg.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3fqaxfpfn.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ufkiydih.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3zritcyjt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3jpuahgyd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3cfgkazgj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3lnspusov.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3rcaodtkf.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3atvoaoir.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3dtglshte.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbcvjlxe.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3sgxltsvg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3gpiytgxf.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3eydswabp.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3pluvwadq.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3forrvknj.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3wivadkdk.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3qbndzaku.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cjxukhls.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3lircwqvw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbtqasja.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3wwdweise.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kbymcwjo.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3lcrjjcha.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3xosfxunt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3diszqrkd.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ujqrwlhu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vohsrhew.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vjsyysbp.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3aiqovact.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ricxbdtw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vjdxbseb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3sdnsuoih.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3nebnamke.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rvimotju.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ylwpgwtz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3srzaakip.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3crhoakih.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3lvzkdovd.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3qjmfcifi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ikwblazb.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3qaayptke.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3tihlzacl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3muenrfox.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwsagkqd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3lfamcjdq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bkkimexw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yyvwiaix.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3yctjdymt.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kxewikij.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mbukhysg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3musacamh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3xyqwllav.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3aaptiyci.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3ioxqrjrc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3knuygpgv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3rejekayp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3ogodrcze.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztqiotta.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zwnamdda.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3vhoyvktn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3wkmnuhea.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3oomghatj.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3knumxcak.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3pyckltby.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3rcuhxkhz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3sjxpxcym.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3hhdtihsv.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3gabpdlep.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3rqsfduqt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3erujfjns.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mcwumenx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbnfypqj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3pmrcmnrm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3okngyndc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3zptsizxe.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3wyfbvnng.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3fqnpripb.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3kmdjzkdc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ojlydhxo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tebpzjdb.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdqhudxu.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zwqpqipd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3oiqvbcxy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yipggqnx.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wleaoire.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3wglhjdtt.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3cqwrrsta.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pwatoepi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3unjurbom.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3siemqcsm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jpgmifqt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3unvdvnye.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3jljiptff.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bytmfmyx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3vmryasma.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3qxxagivs.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3burgkxni.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ouagwvmb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3otpheuux.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lernbewi.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3xtmcnmmu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3iqdwvswi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlnhmldr.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3azoapogd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wzuydfow.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3tyyqqouj.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3gtqdxfli.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3txkvpdsw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3vmckgemp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3lghzhvsl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3dhwrbdel.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqydsvte.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3naqguqfz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3uitlumfx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3doupeuur.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3byhguzqo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3fxflfxeq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3gldlijqy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3gynmgtbr.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3cjczivhp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3ppimdgbh.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qgixkuyl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3fisrcqem.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3vlbvhqek.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yqrebxtq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3isoptwiu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gvykmjxf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3eimvskua.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ciqldxoy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vihomhzk.html


<!-- 参考信息 -->