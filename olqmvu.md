代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2jtxycegj.html

[A11] 条件表达式（三元）
来源：http://www.52xcode.cn/Article/details/gt2zzbtfqhp.html

Py:   "yes" if x > 0 else "no"
来源：http://www.52xcode.cn/Article/details/gt2dugflixb.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2zsgunuli.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2rntivnai.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2esrnargy.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qdjxzgxz.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.52xcode.cn/Article/details/gt2qtbdhdmi.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2vxbmmbvk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pehxhzil.html

[A12] 字符串插值 / 格式化
来源：http://www.ydjk.org.cn/Article/details/gt2pjmzopma.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2kvradhjb.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.ydjk.org.cn/Article/details/gt2arlzugdl.html

JS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2jdbdknbl.html

TS:   `Hello, ${name}!`
来源：http://www.ydjk.org.cn/Article/details/gt2zbjlrndo.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2iuqwmlie.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mihzqjea.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2hqwjjqfm.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2ydmtnuuf.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.ydjk.org.cn/Article/details/gt2wzavoipn.html

Py:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2ghkjnvtx.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ljygolcv.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2gacmwzya.html

TS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2vvxrpoes.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2kmdmsqra.html

Go:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2aaakzdml.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2submdoqb.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2wqlkataw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2koupxlqa.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.52xcode.cn/Article/details/gt2lydbyifu.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2fzbjhtym.html

JS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2tubelzxt.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2cpzgoxuo.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.52xcode.cn/Article/details/gt2vntwaslj.html

Go:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2rlfntelk.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2lwjnoohy.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2yxmoqbcd.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2hhmqdtuq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2fisaeddi.html

PHP:  $value = $data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2wiuibuol.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qiecukst.html

TS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2mchtbruu.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2zitopvwi.html

Go:   if data == "" { data = "默认值" }
来源：http://www.52xcode.cn/Article/details/gt2khsjfcmm.html

Ruby: value = data || "默认值"
来源：http://www.52xcode.cn/Article/details/gt2ptraptvf.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2pmyzcwcm.html

[A16] 真假值判断规则
来源：http://www.ydjk.org.cn/Article/details/gt2ofnbjbxy.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.52xcode.cn/Article/details/gt2nulqavmx.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.52xcode.cn/Article/details/gt2iiryayqn.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2dszpdhjl.html

TS:   if (!x) {}
来源：http://www.52xcode.cn/Article/details/gt2friodlvo.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.52xcode.cn/Article/details/gt2ivyrajyz.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2eqvrtntc.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.ydjk.org.cn/Article/details/gt2wwhfzybm.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjzrkfrz.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2fvwtrkcs.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ukqmyjme.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vcajgeya.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vbaslvqn.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2zywndcrn.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mlyqqbva.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2fawpecgj.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2mixsilnc.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2vhvhhjbt.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2rkufoxvw.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2mfvxdwom.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ioogdvvu.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2panbzouj.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2buahfcrq.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2rezvattt.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2vietqzsz.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt2zoownzwc.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2tlwgnqsy.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2hgihjnsu.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hyboxcwr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2xwgtmnfh.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2rhrgzkbi.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2kjidpsjf.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2xgilflid.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2psmgpsww.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2oygszyqp.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2fpcvpstj.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2gnnnhjrk.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2sloybtmp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2rmfsyafx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2ocwznecj.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hauaztal.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2uwygvzje.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2deubkcuh.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2wlxouslj.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2fbivrbih.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2giijkdru.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2edkgudtx.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2wbpudjih.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2rlusazae.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2inkhoerm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2jrhggtjf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tjcntlbo.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2dqusxvdc.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2ilrfnspg.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2uwlnfqlv.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bhlmimlk.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2namzoony.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2qkkcfxjf.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2pdfvsmmz.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jmyymctw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wherlnzu.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2krwobolk.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2eyvhkpcj.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uyqqlhkb.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2etwikpjn.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2jjeorkdj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2npddltfu.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2sdfqisnk.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2qiynaidm.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dxjcxqzp.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2holszrrh.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.ydjk.org.cn/Article/details/gt2jmvxqzhl.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2guqvrens.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2galdhnfa.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2toyjkidm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2gpvhjtes.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2idorkkdp.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2uoagpleh.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yeachgsf.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2knsmcvlo.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2pobtgoyv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dicdsxye.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2lugiucun.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2pznrrhxm.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mjhcdmwd.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2lmtqlumy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2fdgtypch.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vxuictgo.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2ufwwwjoz.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2oessmnig.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2iuzbpshq.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2jbscsnez.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2fmoajtnu.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2rtlsvfiv.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2tuxjmppw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2gmbcgoqb.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2wjorbfil.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ouqofdan.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2lldajsjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nlisagkh.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2hpxqqnhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pszbjewz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2tvmbecex.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2lejgoouz.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpmstetq.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xavafrqp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2csqdcrua.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2bqbqpqrt.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2odhbcoci.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ucffnwbg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dzazedvi.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2xioqpsxw.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2tonepqne.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2qealuewy.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2grmrzfys.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2thovkemf.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2vjqhzwnm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2ogotqqds.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2vjeybpwz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kgixmnwz.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2duzjuydv.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2cddhhewh.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcunwcnk.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gctxvaov.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhuduibx.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkvzqgds.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2cyosyfag.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2yxcodexu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2lalxibcc.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ygcsmkcm.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2avrltpyu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2mzdzjpki.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zztktkwr.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwvuitym.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mygzddld.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2cwoijigm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2lrnhwnqz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrakbqlb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gdboejve.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2pzebxwjh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qlrwholu.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2umecgezw.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2kxdyvlxs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2xrauugox.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ydntflew.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rpvqdobz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ergogwgg.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2utzgvluq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2ufoqjool.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dasmjocq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2knlclkfb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ctwvvltt.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2xvtspjwh.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ojhahbem.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2ccueamxx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lxgtipys.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2onosetlk.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2rezrjkae.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcihllfn.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2juuyqnnd.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2aqamxicp.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2umwocget.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2asiyjazx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2gdmrcine.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwqczxeh.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ctjzzpak.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2jwuqsrqq.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jbkwxnnj.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nlaczjze.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2vboqipvu.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zuucwaas.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2woytlyom.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2hvyvhmso.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2xovluogm.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2gvbiioee.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kemzrpav.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2mqavscwf.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixguprrp.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2oylxxoid.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tlwmyeci.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2jsaqczbq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2krfczxup.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2szbscird.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2zhdvdofk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2okkdifla.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvwecrhv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2sgjbmyta.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2psgsnklz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrkxauhl.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wasmrlya.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2anrstxqu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2koymihkk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2nglpudiv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2osratodm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2xonussvn.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mnumgrxj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2etryegnv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xoxorqeu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2mzcsqpmp.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2unpnzpej.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2nngilamb.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2kvsddcgf.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2fdjadcin.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2enpbqqha.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2prkbcgei.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tqtiezay.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2aivycpaq.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2avwrvshd.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2qxytjwcu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2rzjwfruw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2lcgqqwit.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zatabjhj.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2euxywljj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2hdriopoa.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2mtpppqjs.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2qxvupois.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2biahsluu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ykqptgma.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2fpksyltg.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2fexzzovu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zqzkivrd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ptisidxi.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qfcegmof.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2siynzatc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxhigcqm.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dmladjrg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2ryaoblnw.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cbbutmwt.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2sgiyreoj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2dvnehorx.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2czllyxuh.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bggmgqgn.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2xymmttdb.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aihcyujj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2bpwfrhkb.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hsbdqrur.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rzagwmcq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pctyodzd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2aetnhmbn.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdbvzrtr.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2znjlknze.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2scpkotlp.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vswvzakr.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yapyhica.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2qxageydc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lnhkxstu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idikhnhm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2cotvglae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hwvplcst.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2arxofxkn.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ylqnutbp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yijpxagv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2neqgyfgl.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2oafkidcw.html


<!-- 参考信息 -->