代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3podavemy.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3dkzwqjpu.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3clsuhcvz.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3aabgscyl.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3mvtcudmv.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3kodvqsut.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sylevlad.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3fjnurojh.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3nrmeszuj.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3oxtxmzyr.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3rzvndbog.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt3vpabrjvr.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt3nuveprel.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3kzutjqop.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3vsetxrre.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3okpvpdxo.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3wilqroko.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3wwnlomiu.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3jccsvklx.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt3sqlvnzfg.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3qjhapvmj.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hjlgcgvs.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nyfmkera.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3tvfmyfot.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3oyyxuewt.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mkzscuso.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3mlosgbjy.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3xofcpjxt.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3ipdrruca.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt3ldlhabsz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3hqhapvgp.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3lqnscghj.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bspfoxcs.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3iqtvdtbb.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3jclkujez.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3ysrbrzal.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3ojxphvdr.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt3giaocvkw.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3gvgumeje.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nageioqo.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3xoeojdeq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3etruqyjq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3ktqebomf.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3onncpvfw.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3lmvommjb.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3dqvjycgy.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt3zkmbyqah.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3mqzgytfd.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3dxctezzm.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3cpytdyrd.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3fruuypxx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpctjdxo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt3pdobqsvp.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3efpztoru.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ctdtthpj.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt3mzwikwbg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3yhusbifb.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3svupiowj.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3ckfgytod.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3zxwbxhkb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3qzhhgoua.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uquhlmzh.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3sfrxoouh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3tpaczstp.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3oafsvahz.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3rloezaog.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nfxrxexd.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3fovvkiei.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3avjxsxcf.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3jhydqhyx.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt3epaftmtr.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3sokcyyxa.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3ueradmlb.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3hhqhykms.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3twdfuehq.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3fgdffqmv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3dvocqhgd.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3lbsnwtdo.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3qjojbzon.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3eztqkolb.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3dbzraroo.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3furgaokn.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3evioqrfp.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3iuryxuar.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3yuhskzuf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3weonocpy.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hdehcmnq.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3sxvcuimg.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3enyzyutx.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3jtcojddy.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt3fhsesgba.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3zpujxqkj.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3rneugkjh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3lejkluiw.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3befksivy.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3lcpvyowy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tnpteezi.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3jqijbgkz.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3ylgusfql.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3sugimndi.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kjsktivl.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jsqcoayv.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3chppjdey.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3uytvktzi.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3drhomsru.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3vpwykote.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmfghtyg.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3dkmiwaro.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3neluxstb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nofrzinm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3ayqbrdgc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3jvchsnnq.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ajhmzwoi.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3zheqkegr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3tyulcbfg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rgfqgjkm.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rduxwdaa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3hpoktsva.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3lwsyopjn.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3vzdavnwp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3rzxpzdex.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3lajjhesi.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ilkgnecr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3dgxifudx.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3plhlekjj.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3euhsqmni.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3zuoohqxp.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3brklqvfq.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3whtmhzsw.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3ptlozkpn.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkuqjfjf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3bcnpeqpp.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bibxkdvv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3kodlqvyd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3bijjpazb.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbpfqnvp.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3rksyzmii.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3ilqwtpvt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3sofmnxtl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3ebfvubgq.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3anonmadn.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3hfbtwzhg.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3xanglfzu.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3qzdlpipn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3gkkrqqxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mddncdfa.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3oloiakqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efcrkdcw.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3umvnhbmm.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3inleqmfv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqlfrjlb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3rcyfnoea.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3omovrkuj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3pkermver.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3gubhtpfq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3kljkxpbj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3fnhdlzhz.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3mljwkvay.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3bbszihuy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3lxxrswqr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mfvyqnuj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3agfcfbpl.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3uidohnnx.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3rqfdqjzi.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3ypkobycw.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3skxackog.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3vwxxptnk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3wrrbfdld.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3htxlziog.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3eekulhca.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3vtkzjkho.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mgvdaoce.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3fujthcjj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3lkuybbtk.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3kfmonhoz.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3iqmeuhay.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3xfivmifv.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3lrqnxart.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qzkzcbyp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3jaioywtn.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhiwmfya.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3atunpnkv.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3txxlnyxd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hzxvoetz.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cpjxeayj.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3dqqixpgd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3resncziv.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3ykwpetak.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3dsbytbdx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwzjqgib.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bsvmcxrl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3mzfmgdsb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pcwijylz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3psydbcmf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3irpyhksq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3imtleqqq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ydbvhoey.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3jyqkatmu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3huqjuhhe.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3ujzzyoqw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3cjimqdxr.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdpqgcmx.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ifbqdwpw.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fxksqlmw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3lnhdvyvo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pzqnmeja.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ddilbstl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwcysijt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3znselrbi.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3rwwofcer.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xffhxhtd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zcfcrtid.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3obbxhtyx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aavnkaws.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dfndtktn.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3baxkmusa.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ttmdmwhs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3jvhexnsq.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3rxlbvfeg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bfullglz.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ngcgquft.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3wurmieks.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ukszpsnb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qetksbfk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikwgcqky.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nsoebdmf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lwceishm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3cnquewpt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nfpmijya.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3sjrmtxyg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3tiioybaq.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhfgawwm.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lhegyspo.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3cpxfchen.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3yufobpqq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qbzjevxz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3clouazki.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3wdfwdkoy.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3vlihtlog.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3gqbeffhs.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3mcfkqvzb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bpqoamaq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3aszdwlzc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3admkmica.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3jvexrgow.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3euhfwqso.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3vwskxtss.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3kohfhsdl.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3zpfdltag.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3twqgebco.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jdqrzcvs.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lbuiaoxu.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jjmyyqwa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3vzarjvwy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3efoopynv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3uzaeddyw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3uzwwxtwp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3bmctlfji.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3qptkobfr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xbkxdmpq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bxthwpzs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3zaiiablh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wpqujzkd.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cyekefea.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3kanjqnho.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3kpadlfdc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rmuympmu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ggpkocxd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3guvmpflx.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wzjemwax.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hivgjics.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3gfcxviot.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dfbfbumh.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rdiafjho.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3afpxwagk.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3gxqjpjiu.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3jtilocvm.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rriculdk.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kjrgkyah.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ikvmvzhb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ajurdngx.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vlazutnb.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dysumjwm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3hfacfjry.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3letauzim.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3chyjzver.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jexnrecc.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3epxbcvnr.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ujbrkeqm.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3obxumvjz.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3ruvixlol.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3otlyfsnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bevvmfci.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3itslovqt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntodidip.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rrkftzbw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3gjhvxgzg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tbbautyg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3majotwlg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3danzlzgh.html


<!-- 参考信息 -->