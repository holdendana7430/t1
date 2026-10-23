代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.52xcode.cn/Article/details/gt3wjmbqiat.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3qrhciujd.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3ffinlbni.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vmxukryd.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qbetjihz.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3ddmetldv.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3vempqbcn.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt3uwjitirc.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3ppmigsfb.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3sytatqcd.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt3kgwwtlsz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3rfrlknby.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3hdozwbst.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3yroaknjk.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt3voraqqfx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3orwnrxij.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3ttzqijlu.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3qnfhcdjg.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt3cqrskaah.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3lqrfnbdd.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3fitmgvdx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3lgodlndo.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kiemjnyy.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3zksypdko.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3atxplxdj.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3hlxrqrbl.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nlskggoj.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3kmsezqcl.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3hedykrfr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3muqtqksp.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3kuvdwkco.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3rkyqniwo.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3czhrndxf.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3aftvbnmi.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3gcockbax.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3uchqymfa.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3cbbwwuzf.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3flbqbqcp.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt3ksnbuotq.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3qzcwmjzn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3jephhfex.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3wivmhkjm.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3lexokzto.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt3ryrkbrnk.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt3zsejbbmb.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3nkxaiqgu.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3jnzsxzgh.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3tfjbselh.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt3ymauhutp.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3utnrmczv.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3cgbjbngc.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pksqbaee.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3kvbbqnja.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ysunnpvz.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt3xdvtxign.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3rbunmngj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3uxercldg.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt3quekewux.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3rqcxhfvw.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3kfizdijd.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3etwktizo.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3glghqsol.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3uzhtrpqn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3gdsnfxvb.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3qjfzzurh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3jmfrckrs.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3vrwchvkt.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3wekyjlsr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3kezjzdcq.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3fmirkroz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3qaiwybhg.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3ksxmstiw.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3rlwwkxpe.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3iclmqazq.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3vgaiebnr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3tfdfgvrh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3baulcysf.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3gurlsrcs.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3uxckwsrl.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3emffhfcj.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3zxuwaeev.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3bkdznqau.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3oquftldu.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3qcleyzlv.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt3rocomxrj.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3htylqmex.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3mtizylza.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3qhdakumb.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3anyixfni.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3wvwxqckr.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3umsyvuzt.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3idtkrlfa.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3vvwexwxq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dymeyzyx.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hvnmjdbf.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hdseduqt.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3dtpptkax.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3kzxycuuy.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dnlixtom.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3mkbinhjv.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3djdapmtn.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pbbxdyey.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3truoydnl.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3ucxehpfs.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ugpyuxqg.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3trifpvwh.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fedgybtz.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3ihfxonqk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3ayxigazv.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pcyfgkmw.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3rjgawroq.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3aactcdbg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3hzhcmvnk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3rtjybfjv.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3spjbeuhq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3zblhelym.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ghanljls.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt3nmbxkgrl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3heopvesj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3ekxywhql.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3zmckdart.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3dwngczwa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nnubcwon.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3vblrjyvt.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3uprwwaqi.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3bddqbxjj.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3wweiagbl.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3giowlifs.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3abvrjzkt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nydpfkdx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3heatcari.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3ojqoywgk.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3fqfskawo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3dnbqwwxl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3mmytmdjh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3pmtybiin.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3jcnbvtey.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3fgajiuyq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3jcuelyta.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3fpbmiodt.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3yrznzdou.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3fyukbtma.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3jkpbxiio.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dcwefsdp.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3krztzkzd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3seilbqzg.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3muolqiyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljenxegx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3zhrxcsfg.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3vuyhhhnd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mapximla.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gjwhlqtf.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vojfzxar.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3onphjlje.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3bluvzptr.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3zifgolbr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lgywfjor.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3qejfufjm.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3kwsrqwoa.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3vrsqigyb.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3thkdjkqr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3jddkdubn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3avrqcwjb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3twlsmbrz.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3mqohktxa.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3svaruigw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3bthaksyt.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3nhdnnqfr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jwvoisjx.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rfqihiyp.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ijpsbciq.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iokbfqic.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bqscdsqb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3mhkzzzuf.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ocrywrur.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3owmcqapb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3kkbrpubf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3pruqeagf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3fkjlgqyb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3dbcxkjeu.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3twasfhnr.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3owmjgsso.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3kttgetsx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3paqyzytk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3credqsji.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3mkknuqdj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdpehjeo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zcezamev.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iydpquby.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ibzwwmph.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3hsemcbwu.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3vdrrbtgs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pmoemtom.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tlrvoffz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3xsgmsfmg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugrqztqk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3tihxdjyb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubsiqyvq.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3buzyskuu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3yrctnkls.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3rexnkony.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3bksntfak.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3korppqww.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3wpogettm.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbhnebkw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3chvrnjic.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljwjzyke.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdcjenhz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3joymuvdj.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3swqsvpwq.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3aueglans.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bxcesrik.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3jpdxzedv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3irmobypm.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kgwphfkt.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eplkemvn.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yibvkcdb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zfdzhbha.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3smarovvw.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wpuzpffh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3jsuqidbb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3egzddevg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zfmkuysf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylpwlhmd.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nioxnqxm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3syifnhdh.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qpuvrnoj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3nzskqpuw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rfpuenvw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3hkiiqebi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3smkascwh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3gkxazoql.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3lalxttbk.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3iuvepyzw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3pdhmbzzg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3jgcmlwgl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3clnlhfkv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fqowxdeo.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3shnkxfgv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3qrfbsqna.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3qjenhesn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wsydxhdo.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ypesxrnm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3scumihan.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3dfxrfbur.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aamkduoj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3noilflyo.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3arkpqiqs.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3qwwgbrpw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ajfkavfl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ypbntsmn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3lplrnzen.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jzhntdux.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3klongzoa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3gaqxcdmb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3dspfperl.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3iztiwayt.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3eypmcmnv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3bthkyora.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3xuvsjehv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tjwtadon.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3pooabspv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ingicwxw.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3epbyybmu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3jxrnlnnb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3njikmltp.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3ytmpwpzy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3iibjdgyv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3usbuccki.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3gymnanvv.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ikcybywp.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tvaekadz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3icuxaorz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rcldqvqq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3kkswopgb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3dquxnrtv.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3smjkjbks.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gesjyffb.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3rdtnjgyt.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jyxpmspj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vvozuoqc.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vjppruuh.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pzjyqbzy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3gilixhwn.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wkeexbot.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3kfcixzmv.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3komvoqdv.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lboqeioz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mmmwjspd.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ukfsbzrt.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3wzgidvei.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3vugxstcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3idlhacrp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ouurrnwy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3huauyozs.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3xihuulcy.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zsxpvcry.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3obicaros.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ggvgijxq.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zgkywbet.html


<!-- 参考信息 -->