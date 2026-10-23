代发 wailian999

TS:   Math.floor(Math.random() * 100) + 1
来源：http://www.52xcode.cn/Article/details/gt3hffckfev.html

Java: new Random().nextInt(100) + 1
来源：http://www.ydjk.org.cn/Article/details/gt3dtfabvcn.html

Go:   rand.Intn(100) + 1               // math/rand
来源：http://www.ydjk.org.cn/Article/details/gt3zgpiqoln.html

Ruby: rand(1..100)
来源：http://www.52xcode.cn/Article/details/gt3byhuwooc.html

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt3afrwrpkp.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt3wnjemkqz.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt3xadpaysm.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3mhcruuqa.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3qgzhdtas.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3vwqbherh.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3zhrtidxs.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt3fjofqdzo.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt3minpelyr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt3qusfwcuy.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt3trlrjfbk.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.52xcode.cn/Article/details/gt3pgmynfpu.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt3crrtoqhc.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3uxyckonn.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt3lxsmpuui.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt3glwhvekl.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.52xcode.cn/Article/details/gt3cpktebkc.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt3qgelmutn.html

C#:   $"Hello, {name}!"
来源：http://www.52xcode.cn/Article/details/gt3puhhumby.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt3lyizkyaf.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3achbynls.html

PHP:  "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3ryobxcsd.html

JS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3zmyksgjw.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3bbcglozt.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3nhxyevoy.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt3msjmeyss.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3eaxkfmet.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt3rameqskk.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt3yuikmeqw.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt3hdzbssxz.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zfswtdoz.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3fmrigaza.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt3bknvwmho.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt3wqmdbadq.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3zqzwlkpe.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.ydjk.org.cn/Article/details/gt3oouabdqy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt3yzsxyroq.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt3eutculer.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3fehhhulg.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3pqcdaecn.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt3delregej.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kgocdmua.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt3dqfpiker.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt3rjaxqqbg.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt3sdsavplr.html

C#:   var value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt3kuhqnpci.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt3myjcjgmx.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3aenjognj.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt3catrgmjh.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3ehueeknj.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt3ywcrrjjf.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt3hhqknwut.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.52xcode.cn/Article/details/gt3czfubebl.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt3jwagcsia.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewchfquh.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt3zdnwlfbg.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3eqwfunia.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nncutqpl.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3nmapxvya.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3xazmeicq.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3qkcbwpws.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt3yrdnsvsz.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3mgzlzcxh.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt3vatjlbot.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt3eiqkspnv.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt3nxmueqot.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt3wrrzngoy.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3jthyrsan.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt3vbsmodiw.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt3qltqwnnz.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3wcfrjzcp.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt3ukmxxhoo.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt3huvlpzgc.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3bntgpmfi.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3pdcjxfen.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3iodagows.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3mmcxzoky.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3pthkblmf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3rtrolpdc.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3yfqkeylg.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3mkwsdruh.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3ygoeetji.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt3qwmtbqph.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3ofuzqobw.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3cqmcskoo.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3qusieqed.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3ycavlshs.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3tvdnnjks.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3ddvpwbzj.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3wjyvzije.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3wyhkoquq.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt3cfhvcxts.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3bnzbcsib.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3pfsvtylg.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hevcfqsu.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3pbecpocw.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3tvihermw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qphwonsu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xzpbsxms.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3jekwuixl.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dkvbgdvz.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3fajcdfhp.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3hcldklyz.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3thpppesu.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3oronpxds.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3poyspgeo.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sbrecdnm.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3afusdvwx.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mjwsfwqt.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3grweffsm.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3wpyaigsc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3qywtpyva.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ejqxpjwt.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3viavybrj.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ybydzokb.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pqpsdtkb.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3riiuancy.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3ksbeqqnh.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3qmhmhasi.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3wdruamwg.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3zowggvli.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3nufsmzhw.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3qinpjbcz.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3fbsmcxpm.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ypmxlflu.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3qpsuwvng.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3cfxzzuar.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ixseymfl.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3ragsacub.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xqomrvuv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3adqykzlj.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3kzquntdx.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3soclnyle.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ysollxay.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3oqomhhis.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ckdzcyxn.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3getbazgv.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3drzumyvc.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3omqhvskj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt3hfznoiwf.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3kflgsifh.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3akifkbym.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3creqpuom.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3gujznzjz.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zccgpqez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sscyatld.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3bikjuhdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxtmhfdj.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3glphazmt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3izjyoafo.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3xssvpwiz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3evrhnuoq.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3wznxdlbc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eyvrxqlr.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3yrzdbzqq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3mumytqyj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3urmwagjd.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3dnytpdzt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3evmlikba.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwotyoxk.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ytdutmbn.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3aazmptkx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bmzntonb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3ulwpsumn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3hetfstbp.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ebdchepp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3yfcaanya.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3crhmynoh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jdorcrrq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3sgqxvlfe.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvupwjrl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mnojuhqb.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3yupykcsd.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3keuiwqvo.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3yooufhvg.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nicgflmz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3lrynavys.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3npxyfoag.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3gndgkjvc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3pqzjzrgi.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3lyrxoyzz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3tstrbsgg.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3nikzjcqc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mesepern.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dzurqfko.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fcdrvwol.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjqgytrs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3gbjckfwt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3octakjse.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3hjtdjeqr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3tejqamjy.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tumotwtb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjwdivhn.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3utmydxwd.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3qqsgthsq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3mvfpbbgk.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahgtdwpb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpdclita.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rwddecfs.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3lkfwrkwo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3wddrfnxo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3yhpvqlam.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3hmpldzwk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3zgntrglu.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebiznoea.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3iouipsuu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jhtnhqrj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvldauaw.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gvgalwqb.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3desmencc.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zcozippf.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3lmbcjetz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3pqxaprvi.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3akxfoajf.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bnyhbcmr.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ivtdpphx.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3akldbdvl.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3newbzmmj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3kzwpahat.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pqgwxbsh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3sojlsuri.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3yushtptn.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ckmeoiyf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgjzctos.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rdtdrpio.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ylaqdszl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3nuzkeamx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3tkuweape.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nctotoif.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3ggoscszj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3bjfkaljg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3srfahbth.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3weailfez.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3niyyrwqt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ynaqiaqn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wngnjcoi.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3akirzzdb.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3jzdfrykq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3gqtebemz.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3qtvzcrib.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3fsxseaat.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3wfqrqljy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pwulluwa.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3oillvddy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3mwyharym.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3vjtivfgn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jwgbpalg.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3jzxoerhp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3fzbjclob.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3wyjnrcug.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qmcggpzm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3khugovlz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jneepmiu.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3xauyspoz.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3izlshrbp.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3mtdyjtje.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3zdkofejy.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3zrnpktre.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3pdxdswqd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdthopnv.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pocvuwzx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3aadnbdtl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3yflhkckq.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3xuopqbvr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3rgipzaej.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3fkwozxjt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3eboflcsu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3yzbtlpcb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3llwsfuav.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jhdeawuj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wbjzuhjd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3oyldxwil.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3seiiwbck.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zlylmgia.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3qooclcvk.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3cedafuay.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3exxqazdj.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3thqyznsr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mcpdbjgs.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zbwgyrsb.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3apuciobn.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lwzounrt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3znbqgynn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3miaivupx.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3iqddeqik.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyqpagzi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gastosqk.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ljvbcmyl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aatumtrw.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gwpbjide.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3hrdqvauj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3daofcejw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uaawmztr.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3nzsmeawr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qsojgvnz.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gswnangl.html


<!-- 参考信息 -->