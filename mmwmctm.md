代发 wailian999

C#:   new Random().Next(1, 101)
来源：http://m.share.hesvh.cn/Article/details/gntbxuwds.sHtML

[A11] 条件表达式（三元）
来源：http://www.blog.zdbjq.cn/Article/details/gssxarzor.sHtML

Py:   "yes" if x > 0 else "no"
来源：http://wap.hesvh.cn/Article/details/glysthfex.sHtML

PHP:  $x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/grqwvqwxt.sHtML

JS:   x > 0 ? "yes" : "no"
来源：http://mobile.hesvh.cn/Article/details/guoilhnnf.sHtML

TS:   x > 0 ? "yes" : "no"
来源：http://www.m.share.fehbvm.com/Article/details/gbdpwbjak.sHtML

Java: x > 0 ? "yes" : "no"
来源：http://3g.hesvh.cn/Article/details/gkhxrfduz.sHtML

Go:   // 无三元运算符，需用 if 语句
来源：http://www.m.share.zdbjq.cn/Article/details/ghtwqfyug.sHtML

Ruby: x > 0 ? "yes" : "no"
来源：http://mobile.fehbvm.com/Article/details/gtgficqwm.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://www.blog.fehbvm.com/Article/details/gmvnovcsj.sHtML

[A12] 字符串插值 / 格式化
来源：http://3g.fehbvm.com/Article/details/gizeoomto.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://blog.hesvh.cn/Article/details/gvrjqthlu.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.m.share.hesvh.cn/Article/details/gelacgmbk.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.hesvh.cn/Article/details/gbyruaoeh.sHtML

TS:   `Hello, ${name}!`
来源：http://www.blog.fehbvm.com/Article/details/gvekxscjp.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://m.share.hesvh.cn/Article/details/gohadpuuj.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://read.share.fehbvm.com/Article/details/gyqvngtql.sHtML

Ruby: "Hello, #{name}!"
来源：http://www.m.share.zdbjq.cn/Article/details/gcqchohts.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.fehbvm.com/Article/details/gclzeodks.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.fehbvm.com/Article/details/gguakxpbv.sHtML

Py:   "第一行\n第二行"
来源：http://blog.hesvh.cn/Article/details/gehvbnkbk.sHtML

PHP:  "第一行\n第二行"
来源：http://3g.zdbjq.cn/Article/details/gmftycxhi.sHtML

JS:   "第一行\n第二行"
来源：http://m.share.zdbjq.cn/Article/details/gnwwtuzqo.sHtML

TS:   "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gmxrlsoug.sHtML

Java: "第一行\n第二行"
来源：http://wap.zdbjq.cn/Article/details/gambrrawl.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gtffaryqb.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.zdbjq.cn/Article/details/gqksoyzus.sHtML

C#:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gnwcpsowe.sHtML

[A14] 注释写法
来源：http://www.blog.fehbvm.com/Article/details/gchynynbg.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.blog.fehbvm.com/Article/details/gporaydom.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gloymisge.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.zdbjq.cn/Article/details/gbsndohbf.sHtML

TS:   // 单行；/* 多行 */
来源：http://www.share.fehbvm.com/Article/details/gnehsfjnh.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://3g.hesvh.cn/Article/details/gpeoaasxn.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.hesvh.cn/Article/details/gkdhfwura.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/gwyunjzex.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/glpvadaep.sHtML

[A15] 空值判断与默认值
来源：http://3g.zdbjq.cn/Article/details/guokqmzid.sHtML

Py:   value = data or "默认值"
来源：http://blog.fehbvm.com/Article/details/gucxyecqr.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gzoyvgnws.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/ghzopdmdh.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.hesvh.cn/Article/details/gevifsrdh.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://wap.hesvh.cn/Article/details/gdjepwczb.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/gsrjadsgv.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gkyhbvldf.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.hesvh.cn/Article/details/grjsgeizl.sHtML

[A16] 真假值判断规则
来源：http://mobile.fehbvm.com/Article/details/gsvexrdlu.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.fehbvm.com/Article/details/gqexodcfl.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://m.share.zdbjq.cn/Article/details/guzzzxeuy.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/gudygixol.sHtML

TS:   if (!x) {}
来源：http://baike.zdbjq.cn/Article/details/gkjwjvqjb.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.blog.fehbvm.com/Article/details/giluuhxjz.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://wap.zdbjq.cn/Article/details/giuivdbal.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://3g.hesvh.cn/Article/details/gubkwzjdr.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.fehbvm.com/Article/details/gejmkbxss.sHtML

[A17] 位运算
来源：http://www.m.share.fehbvm.com/Article/details/gkxmkdper.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/getibdjnf.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://read.share.zdbjq.cn/Article/details/grwqotpfj.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/ghxasmcyr.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gfriggups.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gcilvecbh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gzpyeaonj.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.blog.fehbvm.com/Article/details/grdbsaien.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gaadjlbxa.sHtML

[A18] 字符与 ASCII 码互转
来源：http://read.share.hesvh.cn/Article/details/gmeeozaoa.sHtML

Py:   ord("A"); chr(65)
来源：http://blog.zdbjq.cn/Article/details/gloubdcos.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gnnimzmih.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gxyvuhyjn.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.hesvh.cn/Article/details/gilpiynnf.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.zdbjq.cn/Article/details/gddqizqwz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.hesvh.cn/Article/details/gefyiwlyf.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.hesvh.cn/Article/details/gwutjobvd.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.zdbjq.cn/Article/details/gahvoefpt.sHtML

[A19] 交换两个变量
来源：http://blog.zdbjq.cn/Article/details/gmemweuak.sHtML

Py:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/glqsjodcz.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fehbvm.com/Article/details/gbrmglida.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gpmcjzzst.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/glvpcafbh.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.hesvh.cn/Article/details/gwxfvqaag.sHtML

Go:   a, b = b, a
来源：http://www.share.fehbvm.com/Article/details/glpjfpqsn.sHtML

Ruby: a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gixnpbshz.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.hesvh.cn/Article/details/gqtubgktx.sHtML

[A20] 读取标准输入
来源：http://read.share.fehbvm.com/Article/details/gtilwdauv.sHtML

Py:   name = input("请输入：")
来源：http://baike.fehbvm.com/Article/details/gusbwkwfb.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.fehbvm.com/Article/details/gkcjhslyx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.zdbjq.cn/Article/details/givjbebzr.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.hesvh.cn/Article/details/gkfgbwqrk.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.hesvh.cn/Article/details/gpidbdhjg.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.share.zdbjq.cn/Article/details/glzypzscr.sHtML

Ruby: gets.chomp
来源：http://www.m.share.hesvh.cn/Article/details/gvamewyxo.sHtML

C#:   Console.ReadLine();
来源：http://3g.fehbvm.com/Article/details/golvscgpv.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.zdbjq.cn/Article/details/gpqlwjypm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.blog.fehbvm.com/Article/details/gcdfavtdv.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.fehbvm.com/Article/details/gxxfbktkg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gceaamdjz.sHtML

TS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gepcquzro.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gofnmckkj.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/gnaunzncm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gtovrrujf.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.zdbjq.cn/Article/details/gjztbvway.sHtML

[A22] 获取字符串长度
来源：http://3g.hesvh.cn/Article/details/ghbzuhvvu.sHtML

Py:   len(s)
来源：http://read.share.fehbvm.com/Article/details/gncezpzmt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.hesvh.cn/Article/details/gzapdubmg.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fehbvm.com/Article/details/gnkvuejmo.sHtML

TS:   s.length
来源：http://mobile.fehbvm.com/Article/details/ggbidkqvt.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/greopgrdg.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.zdbjq.cn/Article/details/gmxhprwbl.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/guzvylzpo.sHtML

C#:   s.Length
来源：http://read.share.zdbjq.cn/Article/details/gwoznpshe.sHtML

[A23] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gclfkyzui.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.fehbvm.com/Article/details/gzyuainis.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.hesvh.cn/Article/details/gtxqqsuyf.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.blog.fehbvm.com/Article/details/giomfupnq.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gezqrsvlq.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gdjjmwatg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://wap.hesvh.cn/Article/details/glzqenpvu.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gtpsruycj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://read.share.fehbvm.com/Article/details/ghlqiyzhv.sHtML

[A24] 去除首尾空白
来源：http://m.share.hesvh.cn/Article/details/gazyngzeq.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.fehbvm.com/Article/details/gbqttfqjl.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.fehbvm.com/Article/details/gbpwgfwsi.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fehbvm.com/Article/details/gfztdmkgt.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fehbvm.com/Article/details/gekorhmcc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.fehbvm.com/Article/details/gzokbikqf.sHtML

Go:   strings.TrimSpace(s)
来源：http://blog.fehbvm.com/Article/details/gukqomhgs.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://read.share.hesvh.cn/Article/details/gtlthmwwi.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.zdbjq.cn/Article/details/ginvzxhng.sHtML

[A25] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gnpbyfmmp.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.zdbjq.cn/Article/details/gaitwtklr.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyanhsmze.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/gczzajfqd.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gkncxoomu.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.fehbvm.com/Article/details/gpgupwchf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gimzriphi.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.zdbjq.cn/Article/details/gqnforphv.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://wap.fehbvm.com/Article/details/gztflnwbe.sHtML

[A26] 类型转换总览
来源：http://m.share.fehbvm.com/Article/details/gwtawzvbt.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gpasgjmka.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.hesvh.cn/Article/details/gsqjmwsgf.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fehbvm.com/Article/details/gdcxnztlm.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.blog.fehbvm.com/Article/details/gljibints.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.share.zdbjq.cn/Article/details/glcwopgde.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.hesvh.cn/Article/details/ggyrryvee.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fehbvm.com/Article/details/gsukozwso.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://3g.hesvh.cn/Article/details/girsstcoh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gyryglrfk.sHtML

B. 流程控制
来源：http://3g.fehbvm.com/Article/details/ghjqadptz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxioozvsz.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/gexmfbxfn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.share.hesvh.cn/Article/details/gxawbwdux.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.fehbvm.com/Article/details/gyfadfkri.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gvgyofhxg.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/ggmorxtfn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gevbnolfv.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fehbvm.com/Article/details/gkuvtyabj.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.hesvh.cn/Article/details/gnvrzimcb.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gjrqdywjg.sHtML

[B02] 多分支 else if / elif
来源：http://baike.hesvh.cn/Article/details/gcwygtsbt.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.fehbvm.com/Article/details/glgjcwdkx.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.share.hesvh.cn/Article/details/gsaqheyxy.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gicntqcqb.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gvtsywbya.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gobxtzzco.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.hesvh.cn/Article/details/gumcfmrze.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.m.share.fehbvm.com/Article/details/gcnjogstq.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/gigyeqhaj.sHtML

[B03] switch / match / case
来源：http://read.share.fehbvm.com/Article/details/gpzyddipo.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gjwkuytoe.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.fehbvm.com/Article/details/glzqmemwr.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.hesvh.cn/Article/details/gqiutvvfa.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gufusvyvc.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gxdbewjkf.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gzmpbqdvw.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://baike.hesvh.cn/Article/details/ggcwdgfug.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://wap.zdbjq.cn/Article/details/gtmwzrtxb.sHtML

[B04] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gsninbxcb.sHtML

Py:   for i in range(10): print(i)
来源：http://wap.fehbvm.com/Article/details/gcvorxfmd.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/grewhuwrz.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gpxtbwzzl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/ghpvjhriq.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gkbgeuxba.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.zdbjq.cn/Article/details/gfihgilyo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.zdbjq.cn/Article/details/gqbgfyebd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://read.share.fehbvm.com/Article/details/guwohwdem.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gbbshbrxe.sHtML

Py:   for item in arr: print(item)
来源：http://m.share.zdbjq.cn/Article/details/gptguonwo.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/gfscjgnib.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.zdbjq.cn/Article/details/gewflccyx.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.hesvh.cn/Article/details/gloqgoffo.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.share.fehbvm.com/Article/details/gqzengcfa.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.fehbvm.com/Article/details/gcpistfxd.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.zdbjq.cn/Article/details/gpxxnkaum.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.hesvh.cn/Article/details/gzulxjlii.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gpxxdgxed.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.hesvh.cn/Article/details/gujmwrvlr.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.fehbvm.com/Article/details/gyqvncxtq.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gntkjljqs.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gsncfnuqa.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.fehbvm.com/Article/details/gfhlkppdq.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gcdsprzuv.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/ggurgvqtf.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.hesvh.cn/Article/details/gahlksymj.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/ggozkzexf.sHtML

Py:   while i < 10: i += 1
来源：http://m.share.fehbvm.com/Article/details/gaezjdhcc.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.share.hesvh.cn/Article/details/gkkczupyp.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/gwzitwoor.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.hesvh.cn/Article/details/gpsywozly.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gozbqcfht.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gcgoudscm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gttvqubhx.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.fehbvm.com/Article/details/gcnyymmly.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.fehbvm.com/Article/details/gcqwzosfj.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://blog.fehbvm.com/Article/details/gwohnidfw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://baike.hesvh.cn/Article/details/gljmezjcq.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/grpihwahm.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fehbvm.com/Article/details/grslgsqee.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.fehbvm.com/Article/details/gsnftjcuk.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.zdbjq.cn/Article/details/grjifwhpz.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.blog.zdbjq.cn/Article/details/gphghpsrj.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gcbrorpgx.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/giebjfplb.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.hesvh.cn/Article/details/glqtbsofs.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.fehbvm.com/Article/details/gryzrwafu.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/grrrgnvas.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/glnizwlmo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gmqgcojxe.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://baike.zdbjq.cn/Article/details/giounkrmx.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gdrhoquee.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.hesvh.cn/Article/details/glgqwpyax.sHtML

[B10] 遍历同时拿索引
来源：http://www.share.hesvh.cn/Article/details/gnrzqfewp.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fehbvm.com/Article/details/gvskkxccr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.m.share.hesvh.cn/Article/details/gojuczbug.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.zdbjq.cn/Article/details/gdddjfeyx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://read.share.hesvh.cn/Article/details/gexpytwdk.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.hesvh.cn/Article/details/gxvjdrkmm.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.fehbvm.com/Article/details/gwzmczfgf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/gewjuxaqp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/gvefqxepl.sHtML

[B11] 生成数字序列 / 区间
来源：http://m.share.zdbjq.cn/Article/details/gmgwatuhb.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.hesvh.cn/Article/details/gphviyugm.sHtML

PHP:  range(0, 10, 2);
来源：http://blog.fehbvm.com/Article/details/gasfhdmeb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gqepbglbs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gvgqleabj.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://wap.zdbjq.cn/Article/details/gydtvfhnk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.zdbjq.cn/Article/details/guwgmxuhf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.m.share.hesvh.cn/Article/details/gqlodfpdq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/gbizczsyn.sHtML

[B12] 跳出多层循环
来源：http://blog.fehbvm.com/Article/details/gqymbfhxf.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.zdbjq.cn/Article/details/gymheukvm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gnyaaqslz.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/gaqtqfsan.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.zdbjq.cn/Article/details/gszfwezer.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://baike.zdbjq.cn/Article/details/gllurxawm.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gxomuanws.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://mobile.zdbjq.cn/Article/details/gkcaofjmz.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.zdbjq.cn/Article/details/gdgpcjmjm.sHtML

[B13] 判断是否为数字
来源：http://read.share.hesvh.cn/Article/details/ghmpgaciw.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.hesvh.cn/Article/details/geevahnyi.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gldknpdmn.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/grmuczogr.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/gyhhhrgtb.sHtML

Java: x instanceof Number
来源：http://baike.zdbjq.cn/Article/details/gfhrlpqcj.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://baike.fehbvm.com/Article/details/gmmjgnttq.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gxysuylkk.sHtML

C#:   x is int or double or decimal
来源：http://wap.hesvh.cn/Article/details/gbvhuincx.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.fehbvm.com/Article/details/gjqsedojl.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gcbcqyues.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/gemswmnik.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gcqpphncx.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/glovboave.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbomwlfab.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.share.zdbjq.cn/Article/details/gcrhmjsqa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fehbvm.com/Article/details/gqechvrie.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gvcmebswd.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gfedrrtws.sHtML

Py:   a and b or not c
来源：http://blog.hesvh.cn/Article/details/gqgamihgu.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.zdbjq.cn/Article/details/gobbnhmez.sHtML

JS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gyptckyue.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gqkfqkgae.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gblzwazjn.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/ggyvawzob.sHtML

Ruby: a && b || !c
来源：http://3g.hesvh.cn/Article/details/ggevjygpt.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gwxwchiex.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://read.share.fehbvm.com/Article/details/gvgqbdvcu.sHtML

Py:   if not data: return
来源：http://3g.hesvh.cn/Article/details/gpoikwdfw.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gvyqqztjr.sHtML

JS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gmenvymsa.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gpzfedwuq.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gziaiwszs.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/geozoddsj.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.hesvh.cn/Article/details/gnkkapfir.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/grognoxio.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gweptrqad.sHtML

C. 函数与作用域
来源：http://baike.zdbjq.cn/Article/details/gikzbewgg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gloksvcen.sHtML

[C01] 定义函数
来源：http://m.share.hesvh.cn/Article/details/goqwncssj.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fehbvm.com/Article/details/gigammvln.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://blog.fehbvm.com/Article/details/gwzynqvqt.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gqrzuntmo.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.zdbjq.cn/Article/details/gxdexvluh.sHtML


<!-- 参考信息 -->