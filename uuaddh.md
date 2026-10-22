代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2fosndlrq.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wywvxsbb.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2chsqpzgj.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2giudjjdt.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2ljvcuiyh.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2tsjebatv.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yfcbzvxz.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt2eocixmoy.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2niyquqlg.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2elpnhzdv.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2nvurdhmx.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2iakrqliw.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt2kqpkziau.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2wjxbjapg.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt2vdwryaob.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2ckvehmkd.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2iinghgic.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2siriotbf.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2jrdxjjlj.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2atrjwgwu.html

Java: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ebphomva.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bfecgdgc.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2yynpzulj.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2bbkqjbae.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2pwkqxnzy.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2qmgxkaat.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cclyttok.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2rggivgdx.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2pmxmvoqe.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2excnafkv.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cryhavjl.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt2nvhukxkz.html

C#:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2wguaddbx.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2vugyxmpo.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2tywtgxyt.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2jgxbewpu.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wtbdouph.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2lunftogc.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2sitkrfms.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2wolrgxum.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2lswscqcw.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2szovwvlb.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2ifjeznri.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2wfthlqqz.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2qbbsnoxg.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2bxoqhfot.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2qbouwabj.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ogpvnvqn.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt2gvtczsim.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2edfdbsvv.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2smliqgad.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2qvtvktyf.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkbgesvp.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ndheuoff.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dhwaugiu.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lgjwpmty.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bhgmdqkq.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vaxrgkmp.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2jvvwpghb.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qbxpqcpp.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2ebzhespk.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2dtyfnmfd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2astrqwfp.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2lccqgqqa.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2poecmcsl.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2pylustcf.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2xiqtdcpt.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ebobgerd.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2cywdqwek.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt2pblxxmmk.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ywaogvjg.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2pfhwnlqd.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2uolfcqna.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2cijnfvhb.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2dyqyfebm.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2vazfzmyv.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2fpvegoxw.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2uifythkw.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2orxljyej.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt2tvklvluz.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2iyxynieo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2irjnatla.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2jjbnaffy.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2mnhraocy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2suzfbhxp.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2gdrndzfb.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2pxccllca.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2vvpcimzr.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2bxqpklwe.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ruoqgfqi.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pyipspei.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ccvqswxx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2ojwkzgwh.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2ndoihxem.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2avhshcff.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2prumemvn.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2arvxouae.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2zrvmrnyt.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2eucwtpgk.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2qgllulge.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2imoglmyw.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jdbrokdk.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xlbjfrjd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ntkfutac.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2kfosjgoz.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hdroshoy.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2kitxkpee.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2mudantnv.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2rjppgzaf.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2xbcdbnie.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2uaticicg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hogdqetq.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xqgbvrdf.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2bizejdfx.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2rcvwclpp.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt2hxukhsjl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2noukrprn.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2qrazlgis.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2wkgnzltd.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt2nripehvh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2alkueuhp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2zksubgmb.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kythsnhc.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jwtymumi.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2dpyxakvp.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2hqtvpzvz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2iategoac.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2ghejmkaw.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aofslpbq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2urkbifaa.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2gavzimno.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttwtnxpz.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2zshlflaa.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2ulpikiju.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ygmzvfhx.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2xbvfonfz.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2znjpvzzc.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ddoxdrbp.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pgtbfqig.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2gzqbyndr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2bgmfedpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxfeltly.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2tldwwyof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldxqzknm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2yvissrkd.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2xugkwokx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2xlfpcftu.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rpkasrqp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2wypoxcpm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2xdpndyxc.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2flhtxcfk.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2skxjuidp.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2odwvbjqk.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2vnciedns.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2yqfeakmj.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2emreopza.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2obbywwpj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dbgazjdv.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mynutsgl.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2kofjoifu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2oqupmhkv.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2nxgjdsfl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2wkqfnkvj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ffasbvsi.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vfeyvjnp.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2izbmaqwo.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2elqannsi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2unaihnkw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2diokbswd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2ajrkxrhy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2qibonwhq.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bmoglhge.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2pacxapyu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2urwbfckk.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2lppwtcrp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qkengcgg.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2xvwayrjz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2kohvgkxr.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2kakogepd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwmyxiio.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zhezyysh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2gnhjqqme.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2aysbvnpr.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pnkslofx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2regerxuo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2djmeazuk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rljmmamn.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2tmjswcfr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2eqigyigr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ttgqormv.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qnksdcuk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2zcopjdrm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qfbkjigz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2abvpwyod.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2iibrzvmt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2fxdgbkwg.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2mmppnkdu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2navtzhqz.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2gebpxtbv.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2abuidrfv.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2dzmyqzlh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2hhfbkhhm.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ymfncgdv.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2fxpdxnss.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2vcldkmbk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2ohksiwei.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2jtoxwcii.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2vcxqzssn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2kusihylp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2qnedlfgc.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vtcqjlfw.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2mnlampjp.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2iestnffv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ommuolkf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2qzwnfaqr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pittqnfa.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2afsmocyl.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wrqqfrau.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tarjnbvj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cxhnrteu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqrttjtj.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2anmurpuq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2yltwdlpk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2srcbrdpf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2beresjmj.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2glqftxto.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2ycihbyax.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eiubzaru.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2hipukgay.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2zuidkqsz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2bolglkds.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2jqgmgdlx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2lkombwus.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmlqitfn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2cltrjlex.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2jkggnvpj.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ioingunc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2afrphdvb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jpsrpruk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qcmliqvy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2teamorfl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cqflcehk.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ogcxmhjo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yxxjlqpj.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2vefrrwyq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2rpdxsppk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nwoajcoc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eygkgxyj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ucncwmgi.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2uayuydby.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2yiewpari.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2bfhvwrkm.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2viqbqcza.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2dbwcddww.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2kydqpxjq.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wiuroidw.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntnnozso.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2erobbibo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2vceztazx.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2bgozctay.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2dhwghfdt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2cvpmzqqn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2mixmhxef.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dhtxotwu.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2noivfiye.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2azkqssbw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hroljfyd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nxeeydsb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jwgevxfw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lcbalndq.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2ilhqkuae.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2uihvyrzm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2xgbcbmqt.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2irpzhlzv.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wgbyoiui.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2nofrrgpu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bikbyhex.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2utpjxypi.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2echignoj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2jdtyulkz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2tukaxiah.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2btdnwjgm.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bixjgkjl.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dxeckzss.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2elxxncam.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2gpqpujxw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2xylmcktc.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2yelkwznu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofzrptih.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qgkfruct.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eulmuuoz.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jonxezwa.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2lsuifxpv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynvlcion.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2awyfevbx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhezebun.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrokhiiy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2tmlknrpd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rhpthkxo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2etexmmah.html


<!-- 参考信息 -->