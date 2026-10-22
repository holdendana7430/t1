代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2onapuotk.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2haznyzdt.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rxbbkyvb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2xqfoiiek.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uxyfhwsm.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rdrcbony.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2cmkjyiyf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2tyltnkkj.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2pooluajk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2kcvkauvt.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2quwsjmfz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2yyutxxyu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2twrrbpdp.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2dwxyfgoo.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2hwpnahzs.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2dofrdcin.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2plultlgz.html

Ruby: "Hello, #{name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2uzvlsxam.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2jydakpxw.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2qfzixqkl.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2siusluwt.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2dftumisf.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2xnjbkedk.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qiacpyfr.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2qkmdgljx.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2hczfewck.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2epgdbcia.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2yykpgtap.html

[A14] 注释写法
来源：http://www.52xcode.cn/Article/details/gt2kpnirwii.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2icsghadd.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2keeecaxh.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2gdhcgcvu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wzbycqyb.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2afhwbeua.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2wnddocly.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2twgfluvk.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2khmgccbn.html

[A15] 空值判断与默认值
来源：http://www.ydjk.org.cn/Article/details/gt2sdgtakuh.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2slpzhngd.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2igmtdmpn.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2okbhnaca.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jviocije.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2yrjxbrhi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2drytgfaa.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ggjfwjyq.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ahykrjak.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2sayawvpa.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ozqkhczv.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2xjcfftdt.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2fnnpcvzr.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2xmsoodmx.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnenrnyo.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2tcnvguor.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2gtcdspii.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqljouux.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2gtktioje.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jjwlgevp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xetblxlz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2voqgrtai.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ezhzymjb.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2heeqbaop.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2sdwdcimw.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2xaaptlmc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2jvolafxx.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2midhrwah.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2faversbz.html

PHP:  ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2nclyghsx.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2tfocgybq.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2zowbkiai.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2qeetjooy.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2vesludao.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2zkiwllom.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2zbjvupsk.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2cquakstx.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2admklnoh.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2gwzwzidj.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2orowkazd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2mfdarqfn.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2mqbtqlaj.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2jagtljkq.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2dgczesmc.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2rocezzbc.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2hxjwvyll.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2dvghssrw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2gxcqsith.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2whhdrvqr.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2aqqwwrid.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt2evehdbys.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2imkueqck.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2zgkkpdbx.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2famqbeke.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2yuvbsyhh.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2zguratxx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wcbcgjyv.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2yrsljvzh.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2grarkxfy.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2txtyckhx.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gjngwbyd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ablsxtmh.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2nebgfhbp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cbufzlow.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2arzbamtl.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2anommfdb.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ymijsmpu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2qwpzbmeu.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2qblyhrei.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2flxuzyox.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oozhqptb.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2lekjeayv.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nzecjhsj.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2jcddltea.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2ihabkvwt.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2aanqlnws.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ejobadlq.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fptxfexz.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2cjxoaumk.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dtfjbgsx.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2trwmtfvd.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2jsxnpxcj.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2fwfypfit.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2qbupvjfp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tvtancwb.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xxxamyjg.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2ndhertyc.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2ffurxgrz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2fktddnxk.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2itdsjngl.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2gqgvpead.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2stdhcklt.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2yowxdroa.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tdmteisf.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dfczlftl.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2horwpkub.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2nghomggc.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2tygoctzf.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2sbvufuaa.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2czfkolin.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2fyzpetbi.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2burtcxqb.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2zvlqccrj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2rzwweebv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fzvyedti.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2vptbbnxn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2myjwcxry.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2byouqbyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iokepblt.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2clnzoqdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwuiqxql.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2lrepmlwr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2moijgjzv.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2smmkhsfw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kuswvvjg.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2yqpzkujb.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2reaetctz.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2ngkrsupq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2bkkzjkxr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2kcikuxve.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2elqmpmdb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2zhbyroia.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nribxhft.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jzqirjpj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ikqveuto.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jytuckwr.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2mgpdeimt.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2coozwmrs.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2tsjaqogo.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2yakrqvaj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2jkbrrbfl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxdxkbtn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mhxgigbg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgxysuwm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2chilmqsg.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2bxwfpbub.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2rkuekxeo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2hxziyvff.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2jvfdufig.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zxotnqsj.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2pplcyrkf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2iiizrpys.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2svsqnjzs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2hlzqgzss.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kmvopjks.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2kkoemjdd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xuvsquax.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2rhfbtyad.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2xnkfhkqg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2varbojpe.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtqtrawa.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kuaebhfa.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2gcqdxayh.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2btcosahw.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2bzurqaro.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uaharslp.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2wfobxifk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2vhpknbuk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cvjtyzqj.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zrxgnsag.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2xljahvqp.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2vffdjibw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2tijhhewa.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2yzbfpkzl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2kciyidbs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2kazqbsog.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2swlhzkvn.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrkggcov.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2moklbmpv.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvyjphyi.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2msmlxops.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2galxqmke.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2ueuxoixs.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuoihpuz.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2trwluner.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vsasvxnk.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wjjtuwcn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wsywfmui.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fsdaejdm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2loceduwt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2cqgvnfcm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2uqldgnbw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dqipinir.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2zmgutbqt.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2cvqtrlyb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2unurdxpb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjtbusur.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvdftbyk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2sopwvddm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2odkfrcwh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2jpvuephb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwewqtlg.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2yzuaoqid.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2bnloxlqy.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpvfoqpg.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2oapnzfvf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qwuwatcc.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2nsdvlvxm.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ddyoqobp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zrjrbagn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjbyxvyu.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2hqwufdch.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2kffavdrz.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vomdpngw.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dlfhnziz.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2fplqepiw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nwvduguc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2jnwzgsbv.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2novjlqgz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2uwthoifp.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zqklntvv.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2hsgxmjvq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2vjzuynxi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2qefrzujy.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jjabiuqh.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2fdwtoskh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2smfhcfzk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2vljviorp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2avybvwbe.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2xgkrqpdi.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2dnxfjpon.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qlpakbka.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gvojruxw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cardkcjk.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qlipzclw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2vgvzebkq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fwfnakeg.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2dyeubimy.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ohurshou.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2cxbgetff.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ghbiqswq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tuontosr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uenenzat.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oaovksnm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2ybqunkpj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2rbginkco.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2otnzkxfg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2aaijvvhz.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2bujzvhfk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2pecqoafl.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sbsmmtbj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rebzmdke.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wivixhcw.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zbnxuigw.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cfivhddl.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wvyltkmy.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2ybwrsusp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2gjptawgh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2udorhplu.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2wvgjgeio.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ydcuqjui.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xcdoenoa.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2mvlyvbcj.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2mzimntjx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2puaduytp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2usqnpedw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jpeeqtsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzffxawb.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gporztwe.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2kndwqang.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lzngrsof.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2sqtxkfux.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qaptabaf.html


<!-- 参考信息 -->