代发 wailian999

Ruby: x > 0 ? "yes" : "no"
来源：http://baike.zdbjq.cn/Article/details/gydcxqoek.sHtML

C#:   x > 0 ? "yes" : "no"
来源：http://baike.hesvh.cn/Article/details/gvbmazmqx.sHtML

[A12] 字符串插值 / 格式化
来源：http://www.m.share.hesvh.cn/Article/details/gvhvazpyv.sHtML

Py:   f"Hello, {name}! 年龄 {age}"
来源：http://www.blog.hesvh.cn/Article/details/gbpsvprsr.sHtML

PHP:  "Hello, {$name}!"; sprintf("Hello, %s", $name)
来源：http://www.share.hesvh.cn/Article/details/gehahdtsk.sHtML

JS:   `Hello, ${name}!`
来源：http://blog.zdbjq.cn/Article/details/ghyppbqmz.sHtML

TS:   `Hello, ${name}!`
来源：http://www.m.share.hesvh.cn/Article/details/gaxqrbhzb.sHtML

Java: "Hello, %s!".formatted(name)
来源：http://www.share.fehbvm.com/Article/details/grgjfjifa.sHtML

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://mobile.fehbvm.com/Article/details/gbaoekaad.sHtML

Ruby: "Hello, #{name}!"
来源：http://wap.fehbvm.com/Article/details/gbsuqfbck.sHtML

C#:   $"Hello, {name}!"
来源：http://mobile.zdbjq.cn/Article/details/gmckrqdyx.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://mobile.hesvh.cn/Article/details/gbdrmbsuv.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gcrqdocyw.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gugvbqtbm.sHtML

JS:   "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gwhbfssqj.sHtML

TS:   "第一行\n第二行"
来源：http://www.blog.zdbjq.cn/Article/details/gymcmmizn.sHtML

Java: "第一行\n第二行"
来源：http://read.share.fehbvm.com/Article/details/gqdhkmkzy.sHtML

Go:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gwmsupduh.sHtML

Ruby: "第一行\n第二行"
来源：http://blog.fehbvm.com/Article/details/gvidypjur.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.zdbjq.cn/Article/details/gmwgcmrip.sHtML

[A14] 注释写法
来源：http://mobile.fehbvm.com/Article/details/gzhnqkuar.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.fehbvm.com/Article/details/gfomiavxe.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gsoefwoon.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gdjltlomt.sHtML

TS:   // 单行；/* 多行 */
来源：http://read.share.zdbjq.cn/Article/details/guqejwoyl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.m.share.zdbjq.cn/Article/details/giaaxwxni.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gzwbrousx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.zdbjq.cn/Article/details/gfmdnaulo.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gzfoccqxw.sHtML

[A15] 空值判断与默认值
来源：http://www.share.zdbjq.cn/Article/details/guhmqsfwp.sHtML

Py:   value = data or "默认值"
来源：http://blog.zdbjq.cn/Article/details/gmtmbsddl.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://read.share.zdbjq.cn/Article/details/guikhxriz.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.zdbjq.cn/Article/details/gtllfughq.sHtML

TS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/gggspnyff.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.fehbvm.com/Article/details/gqtxlrzaq.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.hesvh.cn/Article/details/geoqwrggp.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.zdbjq.cn/Article/details/gcuaoivni.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.hesvh.cn/Article/details/gcqemlhil.sHtML

[A16] 真假值判断规则
来源：http://www.m.share.zdbjq.cn/Article/details/giqniiyfm.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://wap.hesvh.cn/Article/details/ggazfuvyf.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.zdbjq.cn/Article/details/gpvwfbcfo.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://3g.hesvh.cn/Article/details/gtvahjxvn.sHtML

TS:   if (!x) {}
来源：http://mobile.zdbjq.cn/Article/details/guezitdpi.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.fehbvm.com/Article/details/gayiwunvc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://mobile.hesvh.cn/Article/details/gxxfounap.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.hesvh.cn/Article/details/gdkxtepfx.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://3g.fehbvm.com/Article/details/gcbspfnhz.sHtML

[A17] 位运算
来源：http://blog.zdbjq.cn/Article/details/gzydnusfg.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.fehbvm.com/Article/details/gmdkynjsk.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.hesvh.cn/Article/details/gdcviomhn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gvyhtgyxe.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/grqtrsgip.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gxhcquory.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/grrcpfldh.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gcrlinzea.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/gprqomgpa.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fehbvm.com/Article/details/gdqondsif.sHtML

Py:   ord("A"); chr(65)
来源：http://baike.hesvh.cn/Article/details/gerxzqotp.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/gvwejstuc.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.fehbvm.com/Article/details/gobywtusb.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/girpzhxro.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.zdbjq.cn/Article/details/gimlblrbl.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://wap.fehbvm.com/Article/details/gjiwtgqpq.sHtML

Ruby: "A".ord; 65.chr
来源：http://baike.zdbjq.cn/Article/details/gulmrilfl.sHtML

C#:   (int)'A'; (char)65
来源：http://baike.hesvh.cn/Article/details/gktuyozwb.sHtML

[A19] 交换两个变量
来源：http://wap.fehbvm.com/Article/details/gbunumjda.sHtML

Py:   a, b = b, a
来源：http://baike.zdbjq.cn/Article/details/gulmgqoim.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.zdbjq.cn/Article/details/ghluddsqm.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.hesvh.cn/Article/details/gppdrveqn.sHtML

TS:   [a, b] = [b, a];
来源：http://baike.zdbjq.cn/Article/details/gibzlrfuf.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.hesvh.cn/Article/details/gqzeyecgh.sHtML

Go:   a, b = b, a
来源：http://baike.hesvh.cn/Article/details/gnjmpxrot.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gzxhpfhcv.sHtML

C#:   (a, b) = (b, a);
来源：http://read.share.zdbjq.cn/Article/details/guogauoxw.sHtML

[A20] 读取标准输入
来源：http://read.share.hesvh.cn/Article/details/gqmnzrkgl.sHtML

Py:   name = input("请输入：")
来源：http://blog.zdbjq.cn/Article/details/gkpmleifm.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://read.share.zdbjq.cn/Article/details/gvynebaqz.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.fehbvm.com/Article/details/gwegudgcj.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/gfchxpxja.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.share.fehbvm.com/Article/details/gpyngjjie.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.fehbvm.com/Article/details/gzixjtysa.sHtML

Ruby: gets.chomp
来源：http://www.m.share.zdbjq.cn/Article/details/guipuoaun.sHtML

C#:   Console.ReadLine();
来源：http://baike.zdbjq.cn/Article/details/gfzimrepo.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fehbvm.com/Article/details/gsmngagpr.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fehbvm.com/Article/details/gkhtwzjcr.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/goizptrjx.sHtML

JS:   (3.14159).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gawlyhstm.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gatuwajxb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/gfisfmnfi.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gfazlsgsr.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://baike.fehbvm.com/Article/details/ghtuqngor.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fehbvm.com/Article/details/gqimhxttd.sHtML

[A22] 获取字符串长度
来源：http://blog.hesvh.cn/Article/details/gibtxphhl.sHtML

Py:   len(s)
来源：http://3g.zdbjq.cn/Article/details/gecmilflt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://baike.fehbvm.com/Article/details/gufaszmsh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fehbvm.com/Article/details/gyyhqzfna.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gjesheoyu.sHtML

Java: s.length()
来源：http://m.share.zdbjq.cn/Article/details/gkjvotnbl.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://wap.zdbjq.cn/Article/details/gnzqkbflp.sHtML

Ruby: s.length
来源：http://blog.hesvh.cn/Article/details/gkigmmypj.sHtML

C#:   s.Length
来源：http://www.blog.fehbvm.com/Article/details/gjauoiadq.sHtML

[A23] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gndbyloib.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.hesvh.cn/Article/details/gwcntnmko.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.m.share.fehbvm.com/Article/details/gsybhzaqe.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gsgdgenmm.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.fehbvm.com/Article/details/gkodqojrb.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.hesvh.cn/Article/details/gmrzziveg.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.hesvh.cn/Article/details/gtkppuxci.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/gnpnsitbq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.zdbjq.cn/Article/details/gfafjqfuv.sHtML

[A24] 去除首尾空白
来源：http://read.share.fehbvm.com/Article/details/gnvekzjob.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.share.zdbjq.cn/Article/details/gikxjaopt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.hesvh.cn/Article/details/gmdwupscj.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gssfqdkdz.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.zdbjq.cn/Article/details/gioprejqq.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.zdbjq.cn/Article/details/gvplnkoqs.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/grhuqzxdk.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.zdbjq.cn/Article/details/guruiklbm.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://read.share.fehbvm.com/Article/details/gcrwjfopn.sHtML

[A25] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gwxxkzkgy.sHtML

Py:   s1 == s2; s1 != s2
来源：http://baike.hesvh.cn/Article/details/gqivafbil.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://read.share.fehbvm.com/Article/details/gagxypdow.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.fehbvm.com/Article/details/gfljknrxs.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/glmybchhg.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.zdbjq.cn/Article/details/gioajpiny.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.share.hesvh.cn/Article/details/gglgwldei.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://mobile.fehbvm.com/Article/details/gbjrslibp.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fehbvm.com/Article/details/gpxejjfzh.sHtML

[A26] 类型转换总览
来源：http://baike.fehbvm.com/Article/details/gumqaqqio.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.fehbvm.com/Article/details/gjufqvylc.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://read.share.zdbjq.cn/Article/details/goubqwwsy.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.hesvh.cn/Article/details/gnrtnpmpl.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.hesvh.cn/Article/details/gdtwxfptl.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.m.share.fehbvm.com/Article/details/gdnakbonw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://baike.zdbjq.cn/Article/details/gjywnhumy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://mobile.fehbvm.com/Article/details/ghoyzokaf.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://baike.hesvh.cn/Article/details/gxtlvvaeh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/glbkbhkqd.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/gcblucqxk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfcbgvzqn.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fehbvm.com/Article/details/gisjuhrnx.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fehbvm.com/Article/details/gmlzhmvnb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.hesvh.cn/Article/details/gecmchdar.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gihbtqarq.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gaxbhbemn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gsanrapca.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/gaynstpju.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://mobile.hesvh.cn/Article/details/gaijpzyap.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://read.share.fehbvm.com/Article/details/gxmtheisn.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/gekkudjjq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://m.share.hesvh.cn/Article/details/gjmtppxwe.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.zdbjq.cn/Article/details/gfniqeqni.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gdnzepgxo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.zdbjq.cn/Article/details/gdgaddwfn.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/grfmxfcqs.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://baike.zdbjq.cn/Article/details/gmryxqnnv.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.zdbjq.cn/Article/details/gzbojopau.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gjfwicvda.sHtML

[B03] switch / match / case
来源：http://www.m.share.fehbvm.com/Article/details/gffprmrvk.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gxuaznich.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.hesvh.cn/Article/details/guxiccwbv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsxhmsdch.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/glvnzcxvf.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.fehbvm.com/Article/details/gkcngjbja.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://wap.zdbjq.cn/Article/details/girodubhl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.zdbjq.cn/Article/details/gfsqmxdht.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fehbvm.com/Article/details/guujawkvj.sHtML

[B04] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gxhlblfty.sHtML

Py:   for i in range(10): print(i)
来源：http://baike.hesvh.cn/Article/details/gaqwumfis.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://wap.fehbvm.com/Article/details/guaoujyzd.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.hesvh.cn/Article/details/gxrumygmj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/gbvitpaca.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gnqvflgis.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/ghmqhvmuo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://www.blog.zdbjq.cn/Article/details/gsrmfaptu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://wap.hesvh.cn/Article/details/gyrdklmzy.sHtML

[B05] 遍历数组 / 列表
来源：http://blog.fehbvm.com/Article/details/glzurqten.sHtML

Py:   for item in arr: print(item)
来源：http://3g.hesvh.cn/Article/details/ghyqpmgey.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.zdbjq.cn/Article/details/gxmlqyxdl.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gxzpgajjk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.hesvh.cn/Article/details/gywmolksn.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/gvrzzqihh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fehbvm.com/Article/details/gpqldtxwb.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/givhwylmn.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/gfwwwsajp.sHtML

[B06] 遍历字典 / 对象
来源：http://mobile.zdbjq.cn/Article/details/geuoielmc.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://blog.fehbvm.com/Article/details/gdbbfhezy.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://m.share.fehbvm.com/Article/details/gjjibqoql.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gosasoskj.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/ggynatekp.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.blog.hesvh.cn/Article/details/glheroyiw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.zdbjq.cn/Article/details/gumujkadx.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.m.share.zdbjq.cn/Article/details/gitxtrnlc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.fehbvm.com/Article/details/gdfbgwckt.sHtML

[B07] while 循环
来源：http://baike.zdbjq.cn/Article/details/gvkvdthpd.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.zdbjq.cn/Article/details/gpnrkkuxn.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://wap.hesvh.cn/Article/details/giiojvcgm.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/godovebza.sHtML

TS:   while (i < 10) { i++; }
来源：http://mobile.zdbjq.cn/Article/details/gnjkurmuh.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gokhluncf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://3g.hesvh.cn/Article/details/gqkimpagz.sHtML

Ruby: while i < 10; i += 1; end
来源：http://m.share.hesvh.cn/Article/details/gmvuldtmh.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.hesvh.cn/Article/details/gqoteouqd.sHtML

[B08] do-while（至少执行一次）
来源：http://3g.hesvh.cn/Article/details/ggygyxelp.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.zdbjq.cn/Article/details/gbdhgjwtx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gttaydhfd.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gikteinvj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/guhfdbypk.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/ghqueccxl.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://blog.hesvh.cn/Article/details/gzvcuyckp.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.hesvh.cn/Article/details/gjlejiuat.sHtML

C#:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gskzlcgvh.sHtML

[B09] break 与 continue
来源：http://read.share.zdbjq.cn/Article/details/gaezijris.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://blog.hesvh.cn/Article/details/gwxiricid.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gwgumezer.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gcgqhatgm.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gsrnyazsc.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.zdbjq.cn/Article/details/gslzztfjp.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gxlrqchmd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/geghdhjod.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gxyzwlvej.sHtML

[B10] 遍历同时拿索引
来源：http://blog.zdbjq.cn/Article/details/glskgbsma.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/gecefvkno.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.share.fehbvm.com/Article/details/gfnvwknos.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://read.share.zdbjq.cn/Article/details/gllepbqom.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gzjodbele.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.hesvh.cn/Article/details/gvewvslqp.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://3g.hesvh.cn/Article/details/gsrpyqxuv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gttdhnwzv.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.zdbjq.cn/Article/details/gqoaphoxj.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fehbvm.com/Article/details/gzxlkfwvm.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.hesvh.cn/Article/details/gcgldbmcm.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gljkcwmqg.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.hesvh.cn/Article/details/gwjfjmxqc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.hesvh.cn/Article/details/gpyahpcwr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://3g.zdbjq.cn/Article/details/gywvwmobn.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.hesvh.cn/Article/details/gppjplkgl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://m.share.hesvh.cn/Article/details/gjehoyktb.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.m.share.hesvh.cn/Article/details/ghwrxqusd.sHtML

[B12] 跳出多层循环
来源：http://m.share.hesvh.cn/Article/details/gnvqkjkho.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/goboyehyu.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.hesvh.cn/Article/details/grbokvkcp.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.fehbvm.com/Article/details/gnwqjwyhn.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/greutqzue.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.zdbjq.cn/Article/details/gasdwvnjo.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.hesvh.cn/Article/details/geutnmrsr.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://baike.hesvh.cn/Article/details/gtvovoxdv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.hesvh.cn/Article/details/gupaeeupb.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gaulpquhr.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gwrldrbut.sHtML

PHP:  is_numeric($x)
来源：http://read.share.fehbvm.com/Article/details/gcophdcyt.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.fehbvm.com/Article/details/gzbnsjaho.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.fehbvm.com/Article/details/gycfmupga.sHtML

Java: x instanceof Number
来源：http://wap.zdbjq.cn/Article/details/gwkjkweyh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.hesvh.cn/Article/details/gsumwcbwv.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.zdbjq.cn/Article/details/gzbahrhyl.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.fehbvm.com/Article/details/gyarhmyts.sHtML

[B14] 判断值是否在集合内
来源：http://mobile.hesvh.cn/Article/details/gqhhhhnbn.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://m.share.fehbvm.com/Article/details/gwsnbdimp.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/giqfdbqia.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://3g.fehbvm.com/Article/details/gsfypwsyg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://wap.fehbvm.com/Article/details/gbmjczoaq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://3g.zdbjq.cn/Article/details/gwcgzumwr.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://baike.hesvh.cn/Article/details/gqrlsoegx.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gavvhibsb.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.hesvh.cn/Article/details/gdmzrivbp.sHtML

[B15] 布尔运算与取反
来源：http://m.share.zdbjq.cn/Article/details/gbvbuagyy.sHtML

Py:   a and b or not c
来源：http://www.share.fehbvm.com/Article/details/gshpxzbdh.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.zdbjq.cn/Article/details/gabvaznka.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gurcxmtol.sHtML

TS:   a && b || !c
来源：http://mobile.fehbvm.com/Article/details/gqoqcrfqv.sHtML

Java: a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gnsmlbkcf.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gzzlvcbus.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gvghlrrhn.sHtML

C#:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gwpqyzkcj.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.zdbjq.cn/Article/details/giaamyoqe.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/gmnlclmhy.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/guavlkblz.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gaavolmdm.sHtML

TS:   if (!data) return;
来源：http://read.share.zdbjq.cn/Article/details/gqcttiopt.sHtML

Java: if (data == null) return;
来源：http://mobile.zdbjq.cn/Article/details/gfvnqqzrl.sHtML

Go:   if data == nil { return }
来源：http://www.blog.fehbvm.com/Article/details/gxjhsefgp.sHtML

Ruby: return if data.nil?
来源：http://3g.zdbjq.cn/Article/details/gxvvwptkq.sHtML

C#:   if (data == null) return;
来源：http://m.share.fehbvm.com/Article/details/gtdecufeg.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpimlrfcz.sHtML

C. 函数与作用域
来源：http://read.share.fehbvm.com/Article/details/gsguhdbuj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsrrdwiah.sHtML

[C01] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gjlrfyvbh.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.fehbvm.com/Article/details/gokmvoroc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.blog.zdbjq.cn/Article/details/gcfcoazcv.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gwfctstwy.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/glcwfcpiv.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.m.share.hesvh.cn/Article/details/gbwbxdxet.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/ggkeqckjm.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.hesvh.cn/Article/details/gkskfwmnq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gggfdgdso.sHtML

[C02] 默认参数
来源：http://www.share.fehbvm.com/Article/details/gsmejgrhm.sHtML

Py:   def greet(name="World"): return name
来源：http://blog.hesvh.cn/Article/details/gztlpsbts.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://m.share.hesvh.cn/Article/details/gbjquvivj.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://baike.hesvh.cn/Article/details/guvmhwpjw.sHtML


<!-- 参考信息 -->