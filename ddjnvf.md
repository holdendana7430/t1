代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://www.ydjk.org.cn/Article/details/gt2aoosesos.html

[A11] 条件表达式（三元）
来源：http://www.ydjk.org.cn/Article/details/gt2dzmwqely.html

Py:   "yes" if x > 0 else "no"
来源：http://www.ydjk.org.cn/Article/details/gt2klofrtjx.html

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2pnuohgrf.html

JS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2ywwotttd.html

TS:   x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2fzmcxvic.html

Java: x > 0 ? "yes" : "no"
来源：http://www.52xcode.cn/Article/details/gt2qhbtrvos.html

Go:   // 无三元运算符，需用 if 语句
来源：http://www.ydjk.org.cn/Article/details/gt2xausnoyy.html

Ruby: x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2adoyqmbk.html

C#:   x > 0 ? "yes" : "no"
来源：http://www.ydjk.org.cn/Article/details/gt2nkfowbln.html

[A12] 字符串插值 / 格式化
来源：http://www.52xcode.cn/Article/details/gt2sgqdexxw.html

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.ydjk.org.cn/Article/details/gt2qromnxet.html

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.52xcode.cn/Article/details/gt2fvdtcfxy.html

JS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2trodhnbf.html

TS:   `Hello, ${name}!`
来源：http://www.52xcode.cn/Article/details/gt2gisuimwi.html

Java: "Hello, %s!".formatted(name)
来源：http://www.52xcode.cn/Article/details/gt2xytwavzb.html

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bwukfjyz.html

Ruby: "Hello, #{name}!"
来源：http://www.52xcode.cn/Article/details/gt2gwwsspwr.html

C#:   $"Hello, {name}!"
来源：http://www.ydjk.org.cn/Article/details/gt2pxyxpocc.html

[A13] 多行字符串（练习 \n 转义）
来源：http://www.52xcode.cn/Article/details/gt2uvjhkuek.html

Py:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2razapzrs.html

PHP:  "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ilfllhsa.html

JS:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2mrijiebg.html

TS:   "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2ggarwnhz.html

Java: "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2slaznvxp.html

Go:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2qtwsgnbl.html

Ruby: "第一行\n第二行"
来源：http://www.52xcode.cn/Article/details/gt2kwgorgla.html

C#:   "第一行\n第二行"
来源：http://www.ydjk.org.cn/Article/details/gt2zbutqejw.html

[A14] 注释写法
来源：http://www.ydjk.org.cn/Article/details/gt2shpsqvrr.html

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.ydjk.org.cn/Article/details/gt2eamcsdwv.html

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2uvfvlkbm.html

JS:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2jeagjnjb.html

TS:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2whudflra.html

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.ydjk.org.cn/Article/details/gt2mwgikxif.html

Go:   // 单行；/* 多行 */
来源：http://www.52xcode.cn/Article/details/gt2zmytzkcb.html

Ruby: # 单行；=begin 多行 =end
来源：http://www.52xcode.cn/Article/details/gt2nyvztymt.html

C#:   // 单行；/* 多行 */
来源：http://www.ydjk.org.cn/Article/details/gt2lrikprbp.html

[A15] 空值判断与默认值
来源：http://www.52xcode.cn/Article/details/gt2liwazrrq.html

Py:   value = data or "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2fdzobslo.html

PHP:  $value = $data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2ivfgsgcf.html

JS:   const value = data ?? "默认值";
来源：http://www.ydjk.org.cn/Article/details/gt2qgeymebh.html

TS:   const value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2uqjrxyhq.html

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://www.ydjk.org.cn/Article/details/gt2kwypdkyx.html

Go:   if data == "" { data = "默认值" }
来源：http://www.ydjk.org.cn/Article/details/gt2yfzduujj.html

Ruby: value = data || "默认值"
来源：http://www.ydjk.org.cn/Article/details/gt2ogtmxwsp.html

C#:   var value = data ?? "默认值";
来源：http://www.52xcode.cn/Article/details/gt2yxhmcizp.html

[A16] 真假值判断规则
来源：http://www.52xcode.cn/Article/details/gt2koatyilq.html

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gljiukxl.html

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.ydjk.org.cn/Article/details/gt2eupoknwk.html

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.52xcode.cn/Article/details/gt2btatglpv.html

TS:   if (!x) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cinpylyb.html

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhzobcgf.html

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.ydjk.org.cn/Article/details/gt2hzdrdjsf.html

Ruby: unless x            # nil 与 false 为假
来源：http://www.52xcode.cn/Article/details/gt2qarfueci.html

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.52xcode.cn/Article/details/gt2cdcwnrop.html

[A17] 位运算
来源：http://www.52xcode.cn/Article/details/gt2wsjoqdrj.html

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2vwuemydi.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2bhmqwvyz.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mcmlrjxx.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ciglvemj.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2dvrtqqac.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2btfwrkom.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ogfvyrpr.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2lmoyouaj.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2fycvrego.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cxlqfosd.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2cbowkrli.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2nbfcnxmp.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2bhcfsphp.html

Java: (int) 'A'; (char) 65
来源：http://www.ydjk.org.cn/Article/details/gt2jmnxplzr.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2ulbgifgs.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2grqcsgdj.html

C#:   (int)'A'; (char)65
来源：http://www.ydjk.org.cn/Article/details/gt2kfhzdtdk.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2qyaubufz.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2uozwlidf.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2viszjaut.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2rxqgtsrv.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2dqixrrgg.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt2rjwlwnqo.html

Go:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2btuxdjws.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2hoyecqdl.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2ugaoazvs.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2mccmphog.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2egsxhxak.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2olxnypyk.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2xuhaxnxn.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2iyucttph.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2oceqledu.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2iozcakgu.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2xhsplsik.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2hohublyh.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2jtidgofe.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2mmasvfsg.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2bcgxaumr.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2plvxxmuk.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2xcozmysx.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2glcebuno.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2fdextxjd.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2tspgmsne.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt2dbnfbmjy.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2disaghdp.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eszmyhhm.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2mycfjvuq.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt2wjktbvfw.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2akvcufsn.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2jnryfnnj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xggnymur.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt2irfeamcu.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yignouzi.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fevszxam.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2hruhqtbo.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2gbcfgbsu.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2xettafyr.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2yaenrbqg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2ytzmhsoy.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2lwciotcj.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fegloisa.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2sbmhmoen.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2ylnnrgeh.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2cqfrpwfu.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt2zqrwqlyx.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uyibiyqz.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2kqosjmsk.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2zapicppy.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2dipwqxag.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2sbgcuqvf.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt2lnmzgjcx.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2oxbpiekq.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2crktfgjl.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lezqegir.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2zrjcbigm.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lztrzmvt.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2philloyo.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2lkhkotpd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2jmriyxgp.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktvjkjsc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2mezswfvn.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2ragrwzri.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2ydijmvbt.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2mnzeuero.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2wxqalweo.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2ypccmblq.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2oyrykpli.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2asidrvuu.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2snkafwom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2snqupbot.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2csvqfhwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhmaaqgx.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2meemwdxl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qwcwosvj.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssgerzxg.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tsqclikd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ogmpxakd.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ighlbldo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2juzlagve.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2mipvxwhr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vuuqhroh.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vnogxkjg.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ifwkghwp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2simgujec.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ckfccdpu.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2samhozoz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2dwopyxgk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2dpzzdqph.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2wepyyedg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2hcokurfo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2uriivcyx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2nscnssgl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2weqnhxil.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvlvoafm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbrfxjar.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkcezimz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2trrewipj.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2yryvfuxs.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2mcgunbwr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fvzeqxhu.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ewqwzmmi.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdaimmkw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfwsuqrc.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2dagovjoq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctqdmsej.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2vkfgryez.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2ozzahnni.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ndkcnfov.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ccsofswo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2bpevavxc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2dhyglfxs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2dwczvggt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqvuzblo.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jgxjckqt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qqmkybcf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2rwsxkqep.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvhfohce.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2bwcgybzl.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2byoblzmb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2vimsufdf.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2loaczqlj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2zoqkdcdg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gduubxrz.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2mtsqtchr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2wnetamnl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ssitcvss.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2qjjbapjs.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2krmdcghs.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvxuqnve.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eppmfvsd.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrbnaxfd.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldnfsnhm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2iftwzxun.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2irixfhke.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2tpiazchl.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2oevscler.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2wzejiliz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2niwdusdd.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2fpmmnzvp.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2etceyzns.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bzlqkkcq.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2vfuxftes.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2whoqsjvj.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2oosjeams.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2pjckxdfz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2kwpsxhzd.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2fnevjgea.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dtdtmyoc.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqcnxsns.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqbijubb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2humczlvo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2xvaenfab.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2tldjfvfh.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2pwinivze.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2cwjneswn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2ovjxnith.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2lvlmayor.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ufzsiige.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2rzqykedf.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2arkarhuh.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2iwigzugr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2liwixzne.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2pjtyinen.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xgeojnog.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ctzavatv.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2oayhaooc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2goiehioq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zmaymkrh.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dvwndjjs.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zcasgcww.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2euiqzzqd.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ahaxfgtb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2yxqboomo.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2nxygopoq.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2owbgnqav.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cqosnsmz.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cicwvimh.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2lwhfzfzv.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2sqpiuimi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2roeuikbm.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ndmrrhrf.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2mmpmwrbu.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wluicple.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2udkqszfj.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2omltonwd.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2qfmztscc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2oikgjpmd.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2wkpuuuag.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2esowaflk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yrzfmqhd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2izzjmhbq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2tmdpzapx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ppmyklel.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2tcobtlwq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ummipzag.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2jpjcqnyg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2flxyfomv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oratlpll.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2odlpnppw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2iixgytiy.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2lfkbhnnf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ofhvltsa.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2jnyxphak.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2uevengsx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qawplfln.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rojzhqmm.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wftfqfno.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2yhryqruh.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ekinmrtd.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2ntofmhao.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2zgrasnth.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2qvqannft.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sbugjveb.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2bzmmfcge.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2pniwdrey.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2emtylddk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohwdknlv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2lnntlvdt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqhmafis.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ueowaled.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2xevfxjus.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxmtcvdl.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dklcujht.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2apttiudh.html


<!-- 参考信息 -->