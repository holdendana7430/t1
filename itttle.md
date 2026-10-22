代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fzfuhqrf.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kuuylueh.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2tdmfodcu.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2ukpaweug.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2dxikwkly.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2cgrfjnta.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2xvljcdmw.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2zemvqruu.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jnmekymq.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2bhqnapak.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2hkqazqag.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2hrtjppws.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2pjtiitbu.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2thnjigsi.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gwqzxvsj.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kgeqkghb.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ivcixozs.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2obrwqlxz.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2weagibjv.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2lbhyuxhb.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2mrrmrnaf.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2tinkxnyn.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2ixdpthwv.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2sxjulnfv.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lycraczv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2alijkftj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cgmvhpiv.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2mtnliwun.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2epznnynx.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wgzuhfhl.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2mbbfewwj.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2mdmkhbsg.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2wjzvlseq.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2nmomcgjt.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2gdnwyiys.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2okgumxgy.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2lldruwia.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2zbaiqdcu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2jmaoaowj.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ixrdpeyv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2zegihlat.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2huhtkvsr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2wkehvpvx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2saaliiea.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2snbkunli.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2ygrhpnaz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2jpirgdew.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2ccfyozbu.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2tqrktceh.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qcctkjvo.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2izgrcufp.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2qczqwydo.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kxsuhsck.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2bnpyygzp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2hapexebq.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2wdrxkydx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2vectichs.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2nfzfzimu.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bltqusml.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2wloocgde.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2rlltjpse.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2jsmnrmbe.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2nbzszjrk.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2oqwrlbcu.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2lswgkwtq.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2yoxmjxvz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tftmdpbo.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2edqjcnof.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2nmquopid.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2auorqfkr.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2dbgowcji.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2apeutirn.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bybnsrmn.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2jljikspa.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2hwgpprsf.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2dltwrdpu.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2lfzgjmrf.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2jumzphlk.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2afwibqpn.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2aqtndzqj.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2alvjnqpl.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt2hsybjmqa.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2fsadhunk.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2kjmfoful.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2fnfwmykz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2adzoowsl.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qtkuowka.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ayeofakp.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2oqhkvtgb.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2febowozs.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2nsvfkkbx.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2chwelrdh.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mvjmfkap.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2gbiiocvn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2sfivanao.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2kfvvriko.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fdhbuasb.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2mmsopnbd.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sebdwceh.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2nijrfkfr.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2onlacqyx.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wzxztcis.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qglfutec.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2bxdmvdyy.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2laijygfc.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fphlgfss.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2hktqeosa.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2hfszfuir.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dmumiqqd.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2laruhlpj.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2uuurykkp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2oovaholp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2jrkkgrzb.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2vxaxlucr.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2qimauqqa.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2buyuunmi.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2xtqsbcew.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2yuzejxwm.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2ejrcziil.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ubbgsugw.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2vbezeggz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2wqfmmbvo.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jfkgevbw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2fyyxyoos.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2gzufhxjw.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpdrgdnc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2epdtvxhu.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2mfzwhpdo.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2aymouwzz.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ffxoqwnq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2gvwmgwxh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2diqehnzo.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2paxmglsq.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ebkqketp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2ofmnsodx.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2wzzyottm.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ztjeiaue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zycvadyx.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2vsjhgwxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ggrfouho.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2qdtweggr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2skfkllxn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2bqpzsomb.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2auvctpbb.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2jjhsonfc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qxpvkcjw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2zsiuonbp.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2auqfhino.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2hflyzzvv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2qtljljad.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2yndzgfes.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2gxzlzhkk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hrnqvfet.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2idmtqqvf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hunjcocu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qcrjmurj.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2uxxsygvi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vponpjvg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2hfpaaibx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2rryplejj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2owjhnulf.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2frnxmkxp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rjrrqxcb.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjagtdfq.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2xjsskknk.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2bloyiklo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2wbuotggb.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ahkdzbeo.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2sfksznwi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqwpuzob.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2mheuaxcw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlrjngav.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlvnpnwy.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2ijumkbdt.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lflfoics.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytswfvtm.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zewpzgnk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2fnexugzn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2raepxgyo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xjbfquyw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2opgoqola.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mgpaovxz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2fchjkwgw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2hwnravxk.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xnwmuudp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qkuevwey.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2ajbxkyze.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2indwrukj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2teftteha.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2quvhwrgf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rejarsew.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2gdodnpjy.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ekagwtbg.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2nkaavyyo.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2qnfkoots.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2rryuptyk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gakkpcrs.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ndckorbr.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2iizvtava.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qzueedan.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2uxbdgxdl.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2bocsnqsq.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2srdcdlpj.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2okmjllkj.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2ftjprhcb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wcgsgorh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2llmzqrds.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yubwgnsm.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kmuzdxnf.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qknsifpb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2wzasppmm.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rxrhslqk.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2hnqqzqeu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2rvjplepz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hojrtfdj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytyoinkz.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mmybxeqc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vvspvykm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jhzjigmr.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2rugktfda.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2urmanaze.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gvvfukbx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2sadcapwc.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2itqzhosk.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2btngfffz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2prsrrtjx.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2kjrhvwbf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2gwgxvuzb.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ntzkqqjk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2tzupobnz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hbnbxrcr.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rufpjbqf.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jrdcgbgu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qiuzhalc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zlzyxruy.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uyuscfku.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2lgrwiojh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2cuzdgasq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dzcmdtqv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2nyibqoaf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2dfvxozho.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2vqqmwkma.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ffojjmoy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zwshmtmp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zjaqftsv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2lioaxwyi.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2koyljkzx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2kffbliia.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ravqtiyd.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2funmevxw.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qedxyjag.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rlwyxyyw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2egwqnnku.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bahzqppr.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2sbrljzes.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2daswific.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2lrqnayow.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2ivwlhmbv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2ngmzmgkz.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2niwyxock.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cvhzuott.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2srmoautg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2dksbfnmh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2usozbpmg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2uujkgauf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gwdmejoa.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2vikdbger.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2lgxxreyc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2rhhjarjp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pqpntxct.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2xejybsxq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hnzjxrfz.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2yhcvcudf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dujlqnge.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2svuajlnv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2xoxrpcvi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2merqapdv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2cljxjvfb.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zurzusli.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2plvzbzhj.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2fitkjtwy.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2nhcwemli.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2iqjkmcxl.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ztlavsue.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kjfnpros.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2giwiudje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2soqvtebk.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2auhkljfl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2udfcjcch.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukhhijmg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdhkpqvi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sltpfqey.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2mjcfcgrg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2tlfpzpzs.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ccjzxpta.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2koonjnuq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bnggjpqt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2bjwemugm.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2bnkyzoss.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wjlqlvqq.html


<!-- 参考信息 -->