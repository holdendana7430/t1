代发 wailian999

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/ghnpluwog.sHtML

PHP:  "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gxclejgga.sHtML

JS:   "第一行\n第二行"
来源：http://mobile.zdbjq.cn/Article/details/gkwfvrrsk.sHtML

TS:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/gsoatdqvk.sHtML

Java: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gueflvtmt.sHtML

Go:   "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gidvhvfhu.sHtML

Ruby: "第一行\n第二行"
来源：http://www.m.share.hesvh.cn/Article/details/gevjbvglg.sHtML

C#:   "第一行\n第二行"
来源：http://read.share.hesvh.cn/Article/details/golandunx.sHtML

[A14] 注释写法
来源：http://read.share.fehbvm.com/Article/details/gtdxrlbsc.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://www.m.share.hesvh.cn/Article/details/gvqgfmmzp.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.zdbjq.cn/Article/details/gmersamiq.sHtML

JS:   // 单行；/* 多行 */
来源：http://3g.fehbvm.com/Article/details/gxgtuerwz.sHtML

TS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gnqxrdgbp.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.share.hesvh.cn/Article/details/gzrxzvgli.sHtML

Go:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gevsdzjmf.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.m.share.zdbjq.cn/Article/details/geqfvvvsw.sHtML

C#:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gzyiwcfxq.sHtML

[A15] 空值判断与默认值
来源：http://baike.fehbvm.com/Article/details/gpufyxinr.sHtML

Py:   value = data or "默认值"
来源：http://read.share.zdbjq.cn/Article/details/gsdqsetsc.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gojqcpcjm.sHtML

JS:   const value = data ?? "默认值";
来源：http://blog.fehbvm.com/Article/details/gvkxcxinm.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/grenvltkl.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/geiakyyjl.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://baike.fehbvm.com/Article/details/gofspwxra.sHtML

Ruby: value = data || "默认值"
来源：http://www.blog.fehbvm.com/Article/details/gvhyjufjr.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.m.share.zdbjq.cn/Article/details/gavdrbpnf.sHtML

[A16] 真假值判断规则
来源：http://wap.fehbvm.com/Article/details/ghyrgishy.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://m.share.fehbvm.com/Article/details/gvlehfjub.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.fehbvm.com/Article/details/gllfjuhfe.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.fehbvm.com/Article/details/gnthlvkki.sHtML

TS:   if (!x) {}
来源：http://3g.zdbjq.cn/Article/details/gspltlwbt.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.hesvh.cn/Article/details/ghplluwse.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://3g.zdbjq.cn/Article/details/gzxmmbsiv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.hesvh.cn/Article/details/gjqpcazqu.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://baike.hesvh.cn/Article/details/gqqzxkhdd.sHtML

[A17] 位运算
来源：http://mobile.fehbvm.com/Article/details/ganqipqsf.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.share.hesvh.cn/Article/details/gkoyqpcsc.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://m.share.fehbvm.com/Article/details/gatjmliqn.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gmaewigja.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gjvbjucwr.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.zdbjq.cn/Article/details/givhsqggm.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gndctylmp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.zdbjq.cn/Article/details/grluhaqfw.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gqrygawom.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/ghrwqztrf.sHtML

Py:   ord("A"); chr(65)
来源：http://mobile.hesvh.cn/Article/details/gjnbhtnbs.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.hesvh.cn/Article/details/gbgipewxu.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.hesvh.cn/Article/details/guuofarov.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.hesvh.cn/Article/details/gjdxihzlm.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.blog.hesvh.cn/Article/details/gqkmulbcd.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.hesvh.cn/Article/details/gqjlxnurh.sHtML

Ruby: "A".ord; 65.chr
来源：http://3g.hesvh.cn/Article/details/gmlmymjpx.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.hesvh.cn/Article/details/gkirlzlrr.sHtML

[A19] 交换两个变量
来源：http://m.share.fehbvm.com/Article/details/gnlpyahtd.sHtML

Py:   a, b = b, a
来源：http://mobile.fehbvm.com/Article/details/ghuvyphfh.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.zdbjq.cn/Article/details/gsqycgqtg.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gqfjgffxa.sHtML

TS:   [a, b] = [b, a];
来源：http://wap.zdbjq.cn/Article/details/gjbkrvqne.sHtML

Java: int t = a; a = b; b = t;
来源：http://read.share.fehbvm.com/Article/details/gmrbhuals.sHtML

Go:   a, b = b, a
来源：http://read.share.fehbvm.com/Article/details/geotmoicy.sHtML

Ruby: a, b = b, a
来源：http://m.share.hesvh.cn/Article/details/gfcsitopc.sHtML

C#:   (a, b) = (b, a);
来源：http://mobile.fehbvm.com/Article/details/grsppztvj.sHtML

[A20] 读取标准输入
来源：http://m.share.hesvh.cn/Article/details/gxunnqriz.sHtML

Py:   name = input("请输入：")
来源：http://wap.fehbvm.com/Article/details/gxrlkvvuy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.zdbjq.cn/Article/details/gsrbuswqi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.zdbjq.cn/Article/details/gixhysguc.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.zdbjq.cn/Article/details/gkflwponf.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://wap.fehbvm.com/Article/details/gckcsltmv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://baike.fehbvm.com/Article/details/gcwbtzaew.sHtML

Ruby: gets.chomp
来源：http://mobile.fehbvm.com/Article/details/glbjsyzpj.sHtML

C#:   Console.ReadLine();
来源：http://baike.zdbjq.cn/Article/details/gbvmcngyu.sHtML

[A21] 保留指定小数位输出
来源：http://baike.fehbvm.com/Article/details/gbfnmamlj.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.fehbvm.com/Article/details/grwlffasx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gxvdtaevt.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/gbzjheawl.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gvtvfwzby.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://read.share.hesvh.cn/Article/details/gsflggizz.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gtgrazydm.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://m.share.zdbjq.cn/Article/details/ggshquwen.sHtML

C#:   3.14159.ToString("F2")
来源：http://mobile.fehbvm.com/Article/details/guizltiqf.sHtML

[A22] 获取字符串长度
来源：http://blog.fehbvm.com/Article/details/gymotfktb.sHtML

Py:   len(s)
来源：http://wap.zdbjq.cn/Article/details/gvbjjxvab.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/glgaimncn.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fehbvm.com/Article/details/gkzkjcmsv.sHtML

TS:   s.length
来源：http://www.blog.fehbvm.com/Article/details/gwfrmpzxd.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/gpxdyugtc.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.zdbjq.cn/Article/details/gqihygadr.sHtML

Ruby: s.length
来源：http://www.m.share.hesvh.cn/Article/details/gdiznwkii.sHtML

C#:   s.Length
来源：http://wap.zdbjq.cn/Article/details/gaawdlkmb.sHtML

[A23] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/giyeglytk.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fehbvm.com/Article/details/gzeitivyf.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://baike.hesvh.cn/Article/details/gtxuppacv.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.zdbjq.cn/Article/details/gazrfvlmw.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.zdbjq.cn/Article/details/gjfprklgc.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/ghmdldojw.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.blog.zdbjq.cn/Article/details/gspmipgsq.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gmjwqcntj.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://mobile.fehbvm.com/Article/details/ggpbluaqd.sHtML

[A24] 去除首尾空白
来源：http://m.share.fehbvm.com/Article/details/gmdzmafhy.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.blog.zdbjq.cn/Article/details/grqupxdjx.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.zdbjq.cn/Article/details/gnmbptfgg.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gkhmdwthu.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.share.zdbjq.cn/Article/details/gsicwabvw.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://read.share.hesvh.cn/Article/details/gezmyikzs.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfeiuyct.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.hesvh.cn/Article/details/ghmqgfobq.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.zdbjq.cn/Article/details/gspyuplzj.sHtML

[A25] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/ggebzezxc.sHtML

Py:   s1 == s2; s1 != s2
来源：http://3g.zdbjq.cn/Article/details/gqycrhlek.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.zdbjq.cn/Article/details/gojrxhdjl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/glszjltxz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.hesvh.cn/Article/details/gchkqfmpv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://wap.hesvh.cn/Article/details/gofmtfovt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.zdbjq.cn/Article/details/gfduxmlin.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.share.zdbjq.cn/Article/details/gbrlcyife.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gcjbcciui.sHtML

[A26] 类型转换总览
来源：http://baike.hesvh.cn/Article/details/gvjsicily.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://3g.hesvh.cn/Article/details/grpzmcure.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.m.share.fehbvm.com/Article/details/geclmhqmc.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/gzpdrfrty.sHtML

TS:   Number() String() Boolean() x as number
来源：http://mobile.hesvh.cn/Article/details/gfnjdczmw.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.zdbjq.cn/Article/details/gaqxschbi.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://m.share.zdbjq.cn/Article/details/grfiwksrg.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://3g.zdbjq.cn/Article/details/gzzwebujo.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gokhmuaig.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbawvsvan.sHtML

B. 流程控制
来源：http://baike.hesvh.cn/Article/details/gkefgskxl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyisvdwmy.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.hesvh.cn/Article/details/gjytydbgq.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gbuospjvb.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.hesvh.cn/Article/details/ghntamylp.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/grflggnyw.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.zdbjq.cn/Article/details/gwmuwtnmd.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gmqcwrdzf.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://read.share.zdbjq.cn/Article/details/goosatkzz.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.m.share.zdbjq.cn/Article/details/gwcxwnpvw.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gwkbhibmv.sHtML

[B02] 多分支 else if / elif
来源：http://www.blog.fehbvm.com/Article/details/gqpeejvwa.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.zdbjq.cn/Article/details/grqqbxnkf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.zdbjq.cn/Article/details/gtctxrpqb.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.hesvh.cn/Article/details/ghuuwoxet.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gvyqysfzd.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.hesvh.cn/Article/details/gyccdtwro.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://blog.hesvh.cn/Article/details/gmkrpdnun.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://3g.zdbjq.cn/Article/details/ghnfwlnjn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.fehbvm.com/Article/details/gbkbadgxk.sHtML

[B03] switch / match / case
来源：http://blog.zdbjq.cn/Article/details/gyqkfpmjw.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://mobile.hesvh.cn/Article/details/gqcbrootu.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://3g.hesvh.cn/Article/details/gythkxazn.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/grumlyslm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fehbvm.com/Article/details/ghqjbcpes.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://baike.hesvh.cn/Article/details/gdglojhee.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.zdbjq.cn/Article/details/gojqoqrqn.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://read.share.hesvh.cn/Article/details/gwxnpveay.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gkafdrswm.sHtML

[B04] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gwkaoemxo.sHtML

Py:   for i in range(10): print(i)
来源：http://m.share.fehbvm.com/Article/details/gdmmodzln.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.share.fehbvm.com/Article/details/gjmgsqpuw.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fehbvm.com/Article/details/geqzhbazv.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://wap.fehbvm.com/Article/details/gffhmjpbt.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://wap.fehbvm.com/Article/details/gfhyknxkt.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/grcocpjbn.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.hesvh.cn/Article/details/gwehmixvu.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gqbukogea.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.fehbvm.com/Article/details/gtaovcvwf.sHtML

Py:   for item in arr: print(item)
来源：http://www.m.share.hesvh.cn/Article/details/gknomrczx.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxqavtohm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.zdbjq.cn/Article/details/gmtliryqo.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.blog.fehbvm.com/Article/details/gddyfochy.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.zdbjq.cn/Article/details/gahsehknq.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.fehbvm.com/Article/details/gzrtrzrms.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/gqcqmquht.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.hesvh.cn/Article/details/gkfdwtapy.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/gycsnimgq.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.share.fehbvm.com/Article/details/gyoruqfok.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.hesvh.cn/Article/details/gosjuwjgm.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.hesvh.cn/Article/details/gfzgpxjss.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gyflshyye.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://3g.zdbjq.cn/Article/details/gietgsfkv.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://baike.hesvh.cn/Article/details/gnkgzzbze.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://m.share.zdbjq.cn/Article/details/gsljkpbrg.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://m.share.fehbvm.com/Article/details/gbxmyhvok.sHtML

[B07] while 循环
来源：http://mobile.hesvh.cn/Article/details/gilnkmxsf.sHtML

Py:   while i < 10: i += 1
来源：http://read.share.zdbjq.cn/Article/details/gqxdqxvqa.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://3g.hesvh.cn/Article/details/gzeonmtrk.sHtML

JS:   while (i < 10) { i++; }
来源：http://mobile.hesvh.cn/Article/details/goznpihge.sHtML

TS:   while (i < 10) { i++; }
来源：http://www.blog.fehbvm.com/Article/details/guqlnwasb.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gngwndnao.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.m.share.hesvh.cn/Article/details/gkhglslux.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.share.fehbvm.com/Article/details/glyidhdsa.sHtML

C#:   while (i < 10) { i++; }
来源：http://wap.fehbvm.com/Article/details/gscbaqlhk.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.fehbvm.com/Article/details/gjklgwilh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://mobile.fehbvm.com/Article/details/gfxisydep.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://blog.zdbjq.cn/Article/details/gvzricigc.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gzxncoopg.sHtML

TS:   do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gxdpsytbt.sHtML

Java: do { i++; } while (i < 10);
来源：http://read.share.fehbvm.com/Article/details/gepdcdhrn.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gosnvbkmb.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://baike.zdbjq.cn/Article/details/gxxfvqhuo.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/ghojepiye.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gfhyhyjkl.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.zdbjq.cn/Article/details/gogjoaryg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gqohxkoea.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gmwrlgzty.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gjedeicvn.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gomlwgcyb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://read.share.fehbvm.com/Article/details/garknuclq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gjcqqjgbo.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.fehbvm.com/Article/details/gjgakvqqd.sHtML

[B10] 遍历同时拿索引
来源：http://www.blog.fehbvm.com/Article/details/ghfveyrkv.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gdlybxmsp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://mobile.fehbvm.com/Article/details/gffxsooen.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.fehbvm.com/Article/details/gjkvkmhgx.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://m.share.fehbvm.com/Article/details/gvyhxlpdw.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://read.share.fehbvm.com/Article/details/gzdhkcuod.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghuoyxfvf.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.fehbvm.com/Article/details/gjvlkubob.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://3g.hesvh.cn/Article/details/gkjalrkjx.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.m.share.hesvh.cn/Article/details/gvxvmsmxn.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.fehbvm.com/Article/details/gosnhcnjm.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.zdbjq.cn/Article/details/guxtgqpju.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.fehbvm.com/Article/details/gwtmuztfs.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.fehbvm.com/Article/details/gqhencphe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.hesvh.cn/Article/details/ggihlwhax.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gdhwaroyb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gphycqmlq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/guoxaiptl.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gqcqpgxjr.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://baike.hesvh.cn/Article/details/gcoihfuja.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://baike.hesvh.cn/Article/details/gqahgzpll.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.fehbvm.com/Article/details/gnklzzpqo.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gbczaxiam.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/gzvxttvde.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.zdbjq.cn/Article/details/gwqynvrfm.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gggbpbnua.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://baike.fehbvm.com/Article/details/gwvlkvsty.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gyebomsnw.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.zdbjq.cn/Article/details/gmkswlbrx.sHtML

PHP:  is_numeric($x)
来源：http://read.share.hesvh.cn/Article/details/gjyapkeuj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gstbsykvf.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gfzpxkmca.sHtML

Java: x instanceof Number
来源：http://blog.hesvh.cn/Article/details/ghmxpbnuu.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.share.zdbjq.cn/Article/details/gzneeynpi.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.blog.zdbjq.cn/Article/details/gvcmdbnhk.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/ghwcfjzhm.sHtML

[B14] 判断值是否在集合内
来源：http://blog.hesvh.cn/Article/details/gdhyfmoxt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gqushpawy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://m.share.hesvh.cn/Article/details/gbaeteihu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://read.share.hesvh.cn/Article/details/gwsturykt.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gaglbmubc.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://baike.hesvh.cn/Article/details/gbdnklzbj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://blog.fehbvm.com/Article/details/ggahwjpvh.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gmlupfngr.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gywpjgwhb.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.zdbjq.cn/Article/details/gmhbkbsav.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gpekagsmi.sHtML

PHP:  $a && $b || !$c
来源：http://blog.fehbvm.com/Article/details/ghtsfkval.sHtML

JS:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gjrrydfhc.sHtML

TS:   a && b || !c
来源：http://www.share.fehbvm.com/Article/details/gwferwjgg.sHtML

Java: a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gdzhwpzff.sHtML

Go:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/gzrdlxjpm.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/giixqdvgv.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gbouhlwte.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/goxczggna.sHtML

Py:   if not data: return
来源：http://mobile.fehbvm.com/Article/details/gdryimyas.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.fehbvm.com/Article/details/gwizjwnvj.sHtML

JS:   if (!data) return;
来源：http://m.share.zdbjq.cn/Article/details/ghzaikucg.sHtML

TS:   if (!data) return;
来源：http://read.share.fehbvm.com/Article/details/gfkneodea.sHtML

Java: if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gplowpwxo.sHtML

Go:   if data == nil { return }
来源：http://m.share.zdbjq.cn/Article/details/gclcfoqdp.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/goqtfevbw.sHtML

C#:   if (data == null) return;
来源：http://3g.zdbjq.cn/Article/details/gvftrmalv.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmkdomzgq.sHtML

C. 函数与作用域
来源：http://mobile.zdbjq.cn/Article/details/gbldqmgcx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggivnfakw.sHtML

[C01] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gdwawihdb.sHtML

Py:   def add(a, b): return a + b
来源：http://read.share.hesvh.cn/Article/details/guqbxdabm.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gzclcxldw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.zdbjq.cn/Article/details/geslwbgow.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gjhveslnu.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.hesvh.cn/Article/details/gifkztvcu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/guwximdcj.sHtML

Ruby: def add(a, b); a + b; end
来源：http://read.share.hesvh.cn/Article/details/gomfpxbuq.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gndxeooqc.sHtML

[C02] 默认参数
来源：http://baike.hesvh.cn/Article/details/gsdadxlmy.sHtML

Py:   def greet(name="World"): return name
来源：http://www.m.share.fehbvm.com/Article/details/ghuidoazj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnooxvyjb.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/gwatiuxnh.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gcmqbrzqh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fehbvm.com/Article/details/glnpbbmrn.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://3g.fehbvm.com/Article/details/gluvictqq.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.fehbvm.com/Article/details/gtvyvkrhl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.hesvh.cn/Article/details/gszhxjevp.sHtML

[C03] 可变参数
来源：http://mobile.hesvh.cn/Article/details/ghspiclzc.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gjmtwspns.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://m.share.hesvh.cn/Article/details/gqtuzrell.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.zdbjq.cn/Article/details/ghzmphqom.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gpqsjfkwq.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.fehbvm.com/Article/details/gitmbmtvr.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://3g.zdbjq.cn/Article/details/gvdvpmppt.sHtML


<!-- 参考信息 -->