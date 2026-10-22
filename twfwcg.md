代发 wailian999

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2wnwklnnb.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2uqlouuze.html

Java: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nkpfkxbf.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2qtukmoxu.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2nwcuaijr.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2egliitua.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2xslijnrx.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2cvifpyyh.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2mfnmcqfz.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2bnjytldx.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2qazlqrkj.html

Java: "Hello, %s!".formatted(name)
来源：http://www.ydjk.org.cn/Article/details/gt2dxynpexc.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vbwisqqi.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2xfgyvpzc.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2luzafmha.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2mpjjyayh.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2uiblafti.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2veezgppv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2rgazbxaa.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2zscrxjnu.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wuikxmzn.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qrgfptlz.html

Ruby: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2axmstgjo.html

C#:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2xcuhrmij.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2sgtxftrm.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2bhojnhnv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2hhjlbxxa.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2ykzzqzeu.html

TS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2isiilzgv.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2jgwcxdxc.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2uxcwinnn.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2rvpmkjlr.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lmrniwwr.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2hubhlxgk.html

Py:   value = data or "默认值"
来源：http://www.52xcode.cn/Article/details/gt2fraqyewn.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2tcbzusom.html

JS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2vwljevsf.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2gijdgupf.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.52xcode.cn/Article/details/gt2jvfiugqm.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2erhziygq.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2duhkvctg.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2dlrepixh.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2xowcxqwa.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2njdbmxwm.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2vpedpnts.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2pphozrwu.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awaktahp.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2yjlgzotj.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2yqrrmuua.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2vifyzxqe.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2dzdkpxar.html

[A17] 位运算
来源：http://www.ydjk.org.cn/Article/details/gt2oxjrhegv.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2kvedngti.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.52xcode.cn/Article/details/gt2iuhqlymw.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rcjjzzmf.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2yfcescix.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dpncmyzp.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2uxfnaaeo.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ysenjtdn.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dshfzlbq.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2icvgwecm.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2akjqejwg.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2gtodimho.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2froffumr.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2suercbxm.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2yqjpiflh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt2fpnawjmw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ukirbafs.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2oeiejoge.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2rwjqtlwt.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2qwqafiul.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2qfrrkdcp.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2nxtxmplz.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2fweoizao.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2cbgqeexz.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2onrespec.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2cggmqysy.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2kqfnujxn.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt2nfwpriib.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ysayefmi.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt2dxlgbbxd.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2qplrhzja.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2apbhfvnx.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2cfgvxnar.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2rqwilmky.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2reupuybk.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2goouexcl.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2isqhffyx.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2gikarzeh.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2uidiplbp.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bbbzsdzb.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpkedigf.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2gupbhfcw.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vvwtetoo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2cydlqdgw.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2puhxnksz.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gqonyodi.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2phxlmjub.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2zqnymufu.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2ntcrndre.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2wlyrylqy.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2bjdxcwnl.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2rdncgtxb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pvpibjdy.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2fxrwsmsl.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vsimttze.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ijrmhkle.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2uqspdggx.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ytpjljhh.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kzseqcrn.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2zqnzkeff.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2ihllvvmy.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2prtrevbt.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2anddyfxt.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2digtnams.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2kfyxporj.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2aegugiyj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2cwxotxbs.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2mnzfldsq.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2sxzhsgfp.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxuupmdc.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt2orlwrunl.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2hbomjykf.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iznpebfi.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2cfwyjitv.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2lqqmmnsh.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ksxjzynr.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ymxnwtws.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2bijafpmn.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2udutrccp.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2cwxhgtqv.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2unshieqc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2mtedmlsx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2gvrqeolj.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2zjxkoowm.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2gfokwglj.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2owfgijxv.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2fnojtjml.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2fbgizzob.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dxhkusfe.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2vxygwyvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmvzjyvj.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2cvqkmwbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fetzwdel.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2gvnchwjy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2dcctpqbg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2sgnvsfro.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2iaekjezt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ozhrpibc.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2setqhcym.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2vpybvcyf.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mdaqnlix.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fohgzqei.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2ddosygwo.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2epgsgosc.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lewmrswr.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ejjsglfu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2zpzwfpoz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2nxswyexs.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ivhougzx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2towptnum.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2imhtgdwb.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2fnheutcn.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2iqfwxevm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uzudxvcb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ckzyerrr.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ljqwkyek.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ekntizyw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ogtxblii.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2kvtlgjzz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2fysbhmsa.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xsglavrw.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2kpmkgrsx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2voyetdnm.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2hljcajzc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2ydmxaexa.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwpdyzvv.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2awrwovlp.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2bkkbsxdx.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2pkjfacjp.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2npiwmmsy.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2vmsugudv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2doquanrx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xywvxtas.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xxzapcrq.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2aczszqsb.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2urrbimar.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2pghgofvy.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2zrgeicec.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2irpqkkyr.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2npmoupue.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2xzkwgmdu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2kbadgurd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2fwykypto.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2envhtgjf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xnzijveu.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vdyhkjpt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2eehqgmex.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2yiqwpzlu.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2wjyzprrf.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2xieghjyr.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcbgrwfi.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ejlzulac.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2pwkkwuug.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2vtwdlvgo.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wzruswvb.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xekrkxbr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2auevlsat.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2vohgnqky.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xcnljtlb.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ggrafmyj.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rjyyakbu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kykavfac.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2pafmsceb.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2wbhtzmve.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2rrulyegu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2wobbcqfa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2rbzutbbb.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pflhyfds.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2lysyxftp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2errayvii.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2jszyqmfl.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jthkniaj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2spenbtzk.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmtbkhzv.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2fbouwnbi.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2xnlmqemt.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2whkienpb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2lgxbjeld.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2mhcunsuv.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ljmswsca.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2wrhazvfv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2bspurnck.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2axwhuhba.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ltqjqkaj.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2hqnnbihn.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2kvepfwjs.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wxrqtqyb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tprxukov.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ifdarjpv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2djhfbzpy.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2yvaqpksn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mxkhyjgb.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2mmanaflf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2keoqrztj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2gdszkqas.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2armyjaen.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2zkyltxhy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2squkluys.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2lvrztals.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2cvgciwsj.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2mthjwapk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2rrxpoynn.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2yaverqmw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2phlmmoia.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2lbporghe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kdhaqnzi.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2zovcnbzy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ctqnhlov.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nikxvihl.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2mwiqsgam.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2qeylubqt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2rqwxhaoh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2bdtxvzwt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ijwalbws.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2clfkpmgi.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hvdjhqiq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2korvbjqc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2czlzdzrm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2gghituap.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2xxahqgjc.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2irsejoum.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2mdhxbvlt.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zrzghfgc.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2uwwuruyr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2afsnpltj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aukigmfw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bgztldnc.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2lpxscdgx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2nmbflvmt.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2blndglhh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2iurutrkz.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2trpmvall.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uzdgcdcl.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2iynzjxdv.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2vltglteh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2gflgytgt.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2kwljlmsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ljqtxysw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2mbxjicbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ghjxixdt.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2slzbirkl.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2whelbyid.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2gsqndgzl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjkkxams.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pehjtaty.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmiokfue.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2scwlmvkl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2gtvzhnqj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzivliwe.html


<!-- 参考信息 -->