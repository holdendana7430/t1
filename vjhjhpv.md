代发 wailian999

Go:   fmt.Sprintf("Hello, %s!", name)
来源：http://wap.hesvh.cn/Article/details/gdzshnzfg.sHtML

Ruby: "Hello, #{name}!"
来源：http://mobile.fehbvm.com/Article/details/gkcdywzgs.sHtML

C#:   $"Hello, {name}!"
来源：http://read.share.zdbjq.cn/Article/details/gpjxvyynr.sHtML

[A13] 多行字符串（练习 \n 转义）
来源：http://baike.zdbjq.cn/Article/details/gghdwzskk.sHtML

Py:   "第一行\n第二行"
来源：http://mobile.hesvh.cn/Article/details/grdcaetzo.sHtML

PHP:  "第一行\n第二行"
来源：http://www.share.hesvh.cn/Article/details/gmwnifgdp.sHtML

JS:   "第一行\n第二行"
来源：http://www.blog.hesvh.cn/Article/details/gewrdknev.sHtML

TS:   "第一行\n第二行"
来源：http://wap.hesvh.cn/Article/details/gmeaztpxj.sHtML

Java: "第一行\n第二行"
来源：http://www.share.zdbjq.cn/Article/details/gwbhecnpq.sHtML

Go:   "第一行\n第二行"
来源：http://m.share.hesvh.cn/Article/details/giczpeaqp.sHtML

Ruby: "第一行\n第二行"
来源：http://baike.hesvh.cn/Article/details/gfhwtfmfq.sHtML

C#:   "第一行\n第二行"
来源：http://wap.fehbvm.com/Article/details/gamodysym.sHtML

[A14] 注释写法
来源：http://3g.fehbvm.com/Article/details/gcklhsmqv.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.fehbvm.com/Article/details/grujfnyrv.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://3g.hesvh.cn/Article/details/grhkbifoh.sHtML

JS:   // 单行；/* 多行 */
来源：http://m.share.zdbjq.cn/Article/details/gbwamnzsq.sHtML

TS:   // 单行；/* 多行 */
来源：http://blog.hesvh.cn/Article/details/grxorwbdg.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://www.blog.hesvh.cn/Article/details/gbylqtsyi.sHtML

Go:   // 单行；/* 多行 */
来源：http://baike.fehbvm.com/Article/details/gedawaixx.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/ghwgxjyvo.sHtML

C#:   // 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gtvcrxkce.sHtML

[A15] 空值判断与默认值
来源：http://www.blog.hesvh.cn/Article/details/gljoxebva.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.hesvh.cn/Article/details/gtjqrtnct.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://3g.zdbjq.cn/Article/details/ghrkmdbiq.sHtML

JS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/grlnmuyiy.sHtML

TS:   const value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gtysqzmkd.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fehbvm.com/Article/details/guljguadp.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://wap.zdbjq.cn/Article/details/gzbiqfjql.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fehbvm.com/Article/details/gzenxffjw.sHtML

C#:   var value = data ?? "默认值";
来源：http://mobile.zdbjq.cn/Article/details/gkqwtvczk.sHtML

[A16] 真假值判断规则
来源：http://baike.hesvh.cn/Article/details/gkqgkonty.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://www.share.hesvh.cn/Article/details/gnqpkifqy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.hesvh.cn/Article/details/gdmylqlmc.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.zdbjq.cn/Article/details/gwkwrefoa.sHtML

TS:   if (!x) {}
来源：http://3g.hesvh.cn/Article/details/gtmljevzp.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://blog.fehbvm.com/Article/details/gosglqcnn.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://baike.fehbvm.com/Article/details/gzugwrgjo.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.hesvh.cn/Article/details/gvwasjdrk.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.fehbvm.com/Article/details/gvfkipshf.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/ggjewuiee.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gxaoapuzh.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://mobile.fehbvm.com/Article/details/gvxzswocs.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gyeclagzk.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gyhehrqjt.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.hesvh.cn/Article/details/gplcfmplf.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://read.share.fehbvm.com/Article/details/gwpqngbuf.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/glcafklry.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gxmzafupz.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.fehbvm.com/Article/details/gzlpjuzuo.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gbshugqea.sHtML

PHP:  ord("A"); chr(65)
来源：http://wap.fehbvm.com/Article/details/goqpfvfyt.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gtcbrhtpk.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.hesvh.cn/Article/details/ghmonmaqa.sHtML

Java: (int) 'A'; (char) 65
来源：http://mobile.hesvh.cn/Article/details/gidlzwuup.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://m.share.fehbvm.com/Article/details/godrrqsbi.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.zdbjq.cn/Article/details/gtdgtuwgl.sHtML

C#:   (int)'A'; (char)65
来源：http://blog.fehbvm.com/Article/details/gpxobpnrg.sHtML

[A19] 交换两个变量
来源：http://blog.hesvh.cn/Article/details/gjxxctfmn.sHtML

Py:   a, b = b, a
来源：http://www.blog.hesvh.cn/Article/details/gvzuupdwk.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.m.share.fehbvm.com/Article/details/ghfwvxusg.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.fehbvm.com/Article/details/ghtqsqwcl.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.hesvh.cn/Article/details/gkimvbwcd.sHtML

Java: int t = a; a = b; b = t;
来源：http://wap.zdbjq.cn/Article/details/gcrbkchdi.sHtML

Go:   a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gvmwswivf.sHtML

Ruby: a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gwcrqdhyg.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.fehbvm.com/Article/details/gtwunkwkf.sHtML

[A20] 读取标准输入
来源：http://www.blog.hesvh.cn/Article/details/gjwjsugwa.sHtML

Py:   name = input("请输入：")
来源：http://3g.zdbjq.cn/Article/details/gvzhxvxar.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fehbvm.com/Article/details/goevyjzeg.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.zdbjq.cn/Article/details/gkjhyhrui.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.hesvh.cn/Article/details/gotyzberg.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.hesvh.cn/Article/details/gaiswfaii.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://read.share.zdbjq.cn/Article/details/gbufyxpvm.sHtML

Ruby: gets.chomp
来源：http://baike.zdbjq.cn/Article/details/gywrwnfiy.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fehbvm.com/Article/details/gayqbupsi.sHtML

[A21] 保留指定小数位输出
来源：http://wap.hesvh.cn/Article/details/gyfxqsnnk.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.share.hesvh.cn/Article/details/glvdhpxjt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.hesvh.cn/Article/details/gdnyfvybg.sHtML

JS:   (3.14159).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/grymqurny.sHtML

TS:   (3.14159).toFixed(2)
来源：http://mobile.hesvh.cn/Article/details/gdcuxtomv.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.zdbjq.cn/Article/details/gjffdvpee.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gghqxbeif.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gxfigsdrg.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.fehbvm.com/Article/details/gsipbbuys.sHtML

[A22] 获取字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/ggsfxutox.sHtML

Py:   len(s)
来源：http://www.share.fehbvm.com/Article/details/gnakkaozt.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://m.share.fehbvm.com/Article/details/gxxbcznav.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fehbvm.com/Article/details/grgxytcsp.sHtML

TS:   s.length
来源：http://mobile.fehbvm.com/Article/details/gmcxvtjof.sHtML

Java: s.length()
来源：http://www.blog.hesvh.cn/Article/details/gvfgrjuao.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://read.share.zdbjq.cn/Article/details/gnshvsomp.sHtML

Ruby: s.length
来源：http://wap.zdbjq.cn/Article/details/gummtcpwh.sHtML

C#:   s.Length
来源：http://baike.fehbvm.com/Article/details/gsirrcula.sHtML

[A23] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gvxqomcxi.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://baike.zdbjq.cn/Article/details/gqgtrkdrs.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://mobile.zdbjq.cn/Article/details/gjpvfghbl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/gizcxwybj.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.hesvh.cn/Article/details/gvkpofzxo.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/grfbqxzcx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.hesvh.cn/Article/details/ginlmuilg.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gvrhqsoro.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.hesvh.cn/Article/details/gmuvcqxwj.sHtML

[A24] 去除首尾空白
来源：http://m.share.hesvh.cn/Article/details/gjarupmjs.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.zdbjq.cn/Article/details/gvdphangt.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.blog.fehbvm.com/Article/details/gyhnrchkn.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gbwnbzfrk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.hesvh.cn/Article/details/gqyxkooro.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.hesvh.cn/Article/details/gwgcgbdca.sHtML

Go:   strings.TrimSpace(s)
来源：http://m.share.fehbvm.com/Article/details/gjihgegbr.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.fehbvm.com/Article/details/goxeqmnxn.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.blog.fehbvm.com/Article/details/gafefvudk.sHtML

[A25] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/guoxltgzv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://read.share.hesvh.cn/Article/details/gtvmdpfop.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.m.share.hesvh.cn/Article/details/gtvkfwqyl.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://3g.fehbvm.com/Article/details/gbkjmmlcw.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gpduqkkfq.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gnxukpswt.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.hesvh.cn/Article/details/gfzozwpxl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://read.share.zdbjq.cn/Article/details/gekbvhxcw.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.fehbvm.com/Article/details/gmyuthmxo.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/gnjtjykqa.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.zdbjq.cn/Article/details/ghojrsawu.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.fehbvm.com/Article/details/gutxdxaho.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://baike.fehbvm.com/Article/details/gxfzhuwot.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.hesvh.cn/Article/details/gzgxqdahj.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.hesvh.cn/Article/details/gfrwpszfo.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://wap.hesvh.cn/Article/details/gorogwnwh.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://read.share.hesvh.cn/Article/details/glndvqzvt.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.zdbjq.cn/Article/details/gmnzvmluh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/grfiuzyre.sHtML

B. 流程控制
来源：http://3g.zdbjq.cn/Article/details/golgknxvj.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gdzrbvuql.sHtML

[B01] 条件判断 if / else
来源：http://www.share.hesvh.cn/Article/details/gwnqztjnv.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.zdbjq.cn/Article/details/glsjgjgtx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://read.share.hesvh.cn/Article/details/gqirvsvyv.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://m.share.zdbjq.cn/Article/details/glzjlcbds.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/gupgoghcc.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://m.share.hesvh.cn/Article/details/gixgscyei.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.zdbjq.cn/Article/details/grygciwpq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://baike.fehbvm.com/Article/details/gdwexeghj.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gnblmsrbh.sHtML

[B02] 多分支 else if / elif
来源：http://wap.fehbvm.com/Article/details/godeoyvut.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/gxvdgbswn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://m.share.fehbvm.com/Article/details/gmfmzpvpe.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/gohrrclro.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gtdxzsjve.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gxipiwick.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gzwjkomzx.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://read.share.zdbjq.cn/Article/details/gaepcdadv.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.fehbvm.com/Article/details/gssprcqqo.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/gyalktyxn.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.fehbvm.com/Article/details/gihygaams.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gstlyqzkx.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gynmxcnsc.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gqjnopfsq.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gvdabidyn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://3g.fehbvm.com/Article/details/gtbzlpbhb.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://m.share.fehbvm.com/Article/details/gfncyokfj.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fehbvm.com/Article/details/genidobun.sHtML

[B04] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/ggfoxqvzd.sHtML

Py:   for i in range(10): print(i)
来源：http://mobile.zdbjq.cn/Article/details/gevpmwitl.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.zdbjq.cn/Article/details/ggkkjkcvq.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://mobile.fehbvm.com/Article/details/gkspyycan.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gmkfwzajr.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsfiuvdcp.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://3g.zdbjq.cn/Article/details/gyfubcqkd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.zdbjq.cn/Article/details/ghybkgqys.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://blog.fehbvm.com/Article/details/guhduesnn.sHtML

[B05] 遍历数组 / 列表
来源：http://read.share.zdbjq.cn/Article/details/gsyjwfchg.sHtML

Py:   for item in arr: print(item)
来源：http://mobile.hesvh.cn/Article/details/gjmfspkah.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.m.share.fehbvm.com/Article/details/gumrdufzz.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/guyybmlac.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gomsmfuzx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/gwidcxxcb.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://mobile.hesvh.cn/Article/details/gmimmmpla.sHtML

Ruby: arr.each { |item| puts item }
来源：http://baike.hesvh.cn/Article/details/gztmljdal.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.share.zdbjq.cn/Article/details/gybvzgzow.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.zdbjq.cn/Article/details/gtgnoifkr.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://www.m.share.zdbjq.cn/Article/details/gkssastuo.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.hesvh.cn/Article/details/grbgvoxiy.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://3g.zdbjq.cn/Article/details/gnxxximsl.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gjxemcpgf.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.zdbjq.cn/Article/details/gzccgqfcn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.hesvh.cn/Article/details/greobcvmh.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/giknjzwdc.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.hesvh.cn/Article/details/gxpxewflg.sHtML

[B07] while 循环
来源：http://www.share.hesvh.cn/Article/details/ghasegrdu.sHtML

Py:   while i < 10: i += 1
来源：http://www.m.share.hesvh.cn/Article/details/gjhqrefns.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/ghfxxoixm.sHtML

JS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/grfxyshae.sHtML

TS:   while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gkqkvtmwd.sHtML

Java: while (i < 10) { i++; }
来源：http://www.share.zdbjq.cn/Article/details/gzwpjgnfk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.hesvh.cn/Article/details/gtjudprzm.sHtML

Ruby: while i < 10; i += 1; end
来源：http://www.blog.fehbvm.com/Article/details/guoydlbdd.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtpybuitv.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.hesvh.cn/Article/details/gnwjyvugw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.zdbjq.cn/Article/details/gsurjjyte.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gihjvcgmm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gycbxuesj.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gdignwsud.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/grposvdgo.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.blog.hesvh.cn/Article/details/gmtzfdkkf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/gggdpkkfa.sHtML

C#:   do { i++; } while (i < 10);
来源：http://blog.hesvh.cn/Article/details/gxdgsukym.sHtML

[B09] break 与 continue
来源：http://www.share.fehbvm.com/Article/details/gfupuwbjp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.hesvh.cn/Article/details/gxnzdkgbe.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gmfrhalee.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gmlxzuaib.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gjbwvkuvy.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gwfbhmaay.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://mobile.fehbvm.com/Article/details/gsdnvfqqo.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.share.zdbjq.cn/Article/details/gblxblqah.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.hesvh.cn/Article/details/gyvezoowj.sHtML

[B10] 遍历同时拿索引
来源：http://www.m.share.hesvh.cn/Article/details/ggpqdjtjx.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gbiwhcfwr.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://wap.hesvh.cn/Article/details/gdptgqlzk.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://3g.hesvh.cn/Article/details/gssuiwkko.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://3g.fehbvm.com/Article/details/ghbanoxqj.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gtqbldjaq.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://m.share.fehbvm.com/Article/details/gdxxrdxva.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.zdbjq.cn/Article/details/gjgyiteay.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.fehbvm.com/Article/details/ghifwfoxz.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.zdbjq.cn/Article/details/ggcqbqsst.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.m.share.zdbjq.cn/Article/details/ggjokzxny.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.hesvh.cn/Article/details/gmiejanua.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://read.share.hesvh.cn/Article/details/gmqlvnocv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fehbvm.com/Article/details/gywvvismo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://baike.fehbvm.com/Article/details/gxktpmekd.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://read.share.hesvh.cn/Article/details/gexssbqdl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.zdbjq.cn/Article/details/gfzbrlbgi.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://read.share.zdbjq.cn/Article/details/gmgmcqith.sHtML

[B12] 跳出多层循环
来源：http://read.share.fehbvm.com/Article/details/gmitlyteq.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://mobile.zdbjq.cn/Article/details/grpphymxy.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.zdbjq.cn/Article/details/gdokzucjv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.hesvh.cn/Article/details/glpzwyfon.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gnjjaauco.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://read.share.hesvh.cn/Article/details/gxyjosjqg.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.m.share.fehbvm.com/Article/details/gkhokpnln.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.zdbjq.cn/Article/details/gfjeqkqvd.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.share.zdbjq.cn/Article/details/gxjnwprfj.sHtML

[B13] 判断是否为数字
来源：http://www.m.share.fehbvm.com/Article/details/gmmkitpbw.sHtML

Py:   isinstance(x, (int, float))
来源：http://blog.fehbvm.com/Article/details/goggnduoh.sHtML

PHP:  is_numeric($x)
来源：http://mobile.zdbjq.cn/Article/details/gjishomnp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gxqalffkw.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fehbvm.com/Article/details/ghsvgidte.sHtML

Java: x instanceof Number
来源：http://www.share.fehbvm.com/Article/details/gttgopzdh.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.m.share.fehbvm.com/Article/details/gfmkfcxaa.sHtML

Ruby: x.is_a?(Numeric)
来源：http://3g.zdbjq.cn/Article/details/gppqubejq.sHtML

C#:   x is int or double or decimal
来源：http://www.blog.zdbjq.cn/Article/details/gtniwlbtr.sHtML

[B14] 判断值是否在集合内
来源：http://wap.fehbvm.com/Article/details/gvtfwtfyv.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.zdbjq.cn/Article/details/gxnpmuavd.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.share.zdbjq.cn/Article/details/geczbwgev.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gvtvihcfe.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fehbvm.com/Article/details/gqbutjnjs.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/ggtvavosy.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.zdbjq.cn/Article/details/gxgxlzree.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://read.share.hesvh.cn/Article/details/gqlagnose.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gejvktmvm.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fehbvm.com/Article/details/gwzotceez.sHtML

Py:   a and b or not c
来源：http://3g.zdbjq.cn/Article/details/gkgboajjp.sHtML

PHP:  $a && $b || !$c
来源：http://3g.hesvh.cn/Article/details/gdmkqoqld.sHtML

JS:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gmnplutql.sHtML

TS:   a && b || !c
来源：http://www.share.zdbjq.cn/Article/details/gkiobhpon.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gzqjigbqr.sHtML

Go:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/glvnnnhbm.sHtML

Ruby: a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gezjyvufm.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gwxsmzejs.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gybmbvjbc.sHtML

Py:   if not data: return
来源：http://www.share.hesvh.cn/Article/details/gjvqfwfqv.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fehbvm.com/Article/details/gpthxvzlu.sHtML

JS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/ggvmhwdcs.sHtML

TS:   if (!data) return;
来源：http://wap.fehbvm.com/Article/details/gtlucngec.sHtML

Java: if (data == null) return;
来源：http://www.blog.hesvh.cn/Article/details/gkityvzsi.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gcmeidxkh.sHtML

Ruby: return if data.nil?
来源：http://read.share.zdbjq.cn/Article/details/gkgvnyfgo.sHtML

C#:   if (data == null) return;
来源：http://blog.zdbjq.cn/Article/details/gweqlmjde.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtcgqcmgo.sHtML

C. 函数与作用域
来源：http://wap.hesvh.cn/Article/details/gjecnpajs.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gejjedhdn.sHtML

[C01] 定义函数
来源：http://wap.fehbvm.com/Article/details/gsleelehn.sHtML

Py:   def add(a, b): return a + b
来源：http://www.share.hesvh.cn/Article/details/gxvcmsehj.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.fehbvm.com/Article/details/glhqtdlvq.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://blog.hesvh.cn/Article/details/geyfdxydb.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gidbivemd.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://wap.fehbvm.com/Article/details/gaqbxxeld.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gvhkonfcb.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/gjumvpmjw.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/ggssydvxx.sHtML

[C02] 默认参数
来源：http://wap.fehbvm.com/Article/details/gstouzpyb.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/gcwzpmmmj.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://read.share.zdbjq.cn/Article/details/gkirrxieq.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/grotyuqhi.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gjfhyewxn.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://baike.fehbvm.com/Article/details/gwtbvwfex.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.hesvh.cn/Article/details/gpyuszynz.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/gaypgpohd.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gmxjxqcul.sHtML

[C03] 可变参数
来源：http://baike.fehbvm.com/Article/details/gpgrkgmjg.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fehbvm.com/Article/details/gontlibdz.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.zdbjq.cn/Article/details/gqpveopqq.sHtML


<!-- 参考信息 -->