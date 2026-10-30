代发 wailian999

[A14] 注释写法
来源：http://mobile.hesvh.cn/Article/details/gcjmptcnh.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://wap.hesvh.cn/Article/details/gsriqboij.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://www.share.hesvh.cn/Article/details/gsvnkpqld.sHtML

JS:   // 单行；/* 多行 */
来源：http://www.m.share.fehbvm.com/Article/details/gpwuviqrz.sHtML

TS:   // 单行；/* 多行 */
来源：http://mobile.hesvh.cn/Article/details/gbhepypgl.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.zdbjq.cn/Article/details/guaynvemj.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.blog.zdbjq.cn/Article/details/gfewoezpj.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://mobile.hesvh.cn/Article/details/gcnpafvxm.sHtML

C#:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gpmswaysl.sHtML

[A15] 空值判断与默认值
来源：http://m.share.zdbjq.cn/Article/details/gcpkdlnpl.sHtML

Py:   value = data or "默认值"
来源：http://www.blog.hesvh.cn/Article/details/guuuynhpy.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://mobile.hesvh.cn/Article/details/gqtelxavh.sHtML

JS:   const value = data ?? "默认值";
来源：http://www.blog.hesvh.cn/Article/details/gnqvceiim.sHtML

TS:   const value = data ?? "默认值";
来源：http://3g.fehbvm.com/Article/details/gauirnxih.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fehbvm.com/Article/details/gwfypbppn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://mobile.fehbvm.com/Article/details/gtfiewglk.sHtML

Ruby: value = data || "默认值"
来源：http://mobile.hesvh.cn/Article/details/gtjdmhjfu.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gzuordstf.sHtML

[A16] 真假值判断规则
来源：http://wap.zdbjq.cn/Article/details/gztlkacsn.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://read.share.zdbjq.cn/Article/details/gjhafrzha.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.share.zdbjq.cn/Article/details/gqtbrfrny.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.m.share.hesvh.cn/Article/details/gtgdrkmmz.sHtML

TS:   if (!x) {}
来源：http://www.blog.fehbvm.com/Article/details/gmfidxjex.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbtelrxvv.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.fehbvm.com/Article/details/gkgczjxuv.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://wap.fehbvm.com/Article/details/gvcngekcv.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.hesvh.cn/Article/details/gowbjqbzc.sHtML

[A17] 位运算
来源：http://3g.zdbjq.cn/Article/details/gwlccraln.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.hesvh.cn/Article/details/gbuixyzts.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://baike.fehbvm.com/Article/details/gouvgchrb.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.hesvh.cn/Article/details/gkwixukxc.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://3g.hesvh.cn/Article/details/gnqtgxexx.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.fehbvm.com/Article/details/gtncnnzjc.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gyeqhkfyo.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.hesvh.cn/Article/details/gwdrqxgvf.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gpmnywbfy.sHtML

[A18] 字符与 ASCII 码互转
来源：http://baike.zdbjq.cn/Article/details/gzptdsanb.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gncsopqoh.sHtML

PHP:  ord("A"); chr(65)
来源：http://read.share.fehbvm.com/Article/details/gvxiehrpd.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gcjsrubij.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.fehbvm.com/Article/details/grmdrixha.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.share.hesvh.cn/Article/details/gtnfrsduo.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.zdbjq.cn/Article/details/gzsxgzhdm.sHtML

Ruby: "A".ord; 65.chr
来源：http://mobile.fehbvm.com/Article/details/ghrloldoj.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.zdbjq.cn/Article/details/gsxwmihlp.sHtML

[A19] 交换两个变量
来源：http://read.share.zdbjq.cn/Article/details/gteliqqrq.sHtML

Py:   a, b = b, a
来源：http://3g.fehbvm.com/Article/details/gbdpliqzp.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://m.share.fehbvm.com/Article/details/gylmhvczt.sHtML

JS:   [a, b] = [b, a];
来源：http://www.blog.hesvh.cn/Article/details/gwgwwffqk.sHtML

TS:   [a, b] = [b, a];
来源：http://read.share.fehbvm.com/Article/details/gsmokkivk.sHtML

Java: int t = a; a = b; b = t;
来源：http://blog.hesvh.cn/Article/details/gyniablwl.sHtML

Go:   a, b = b, a
来源：http://www.m.share.hesvh.cn/Article/details/gzxgjxrag.sHtML

Ruby: a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/gbrktijuj.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fehbvm.com/Article/details/gowrustqn.sHtML

[A20] 读取标准输入
来源：http://www.share.hesvh.cn/Article/details/gihrmzeve.sHtML

Py:   name = input("请输入：")
来源：http://m.share.hesvh.cn/Article/details/gpoubgmuz.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://wap.fehbvm.com/Article/details/gdqgknzae.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://wap.hesvh.cn/Article/details/gdlcahujj.sHtML

TS:   // Node.js：readline 模块
来源：http://baike.fehbvm.com/Article/details/gpmwhneev.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://3g.fehbvm.com/Article/details/gzzrsjgqq.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.blog.zdbjq.cn/Article/details/gagtblyvi.sHtML

Ruby: gets.chomp
来源：http://m.share.fehbvm.com/Article/details/guffstphg.sHtML

C#:   Console.ReadLine();
来源：http://www.share.fehbvm.com/Article/details/gewizefhn.sHtML

[A21] 保留指定小数位输出
来源：http://m.share.hesvh.cn/Article/details/gdztkuvyf.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/gczrzrxdq.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.zdbjq.cn/Article/details/gqhlriyhe.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gairyxlic.sHtML

TS:   (3.14159).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gvfjkayxb.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.zdbjq.cn/Article/details/guafrkgpt.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://read.share.zdbjq.cn/Article/details/goplkjacw.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.share.fehbvm.com/Article/details/gniwvmmpr.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.share.zdbjq.cn/Article/details/gznrdzlns.sHtML

[A22] 获取字符串长度
来源：http://m.share.fehbvm.com/Article/details/grahrbrwm.sHtML

Py:   len(s)
来源：http://www.share.hesvh.cn/Article/details/gocbwfihx.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.hesvh.cn/Article/details/gkfwivrgs.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://wap.fehbvm.com/Article/details/ghpldiohy.sHtML

TS:   s.length
来源：http://blog.hesvh.cn/Article/details/ggonudmlc.sHtML

Java: s.length()
来源：http://www.share.hesvh.cn/Article/details/gqzsxyens.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gumfetyrt.sHtML

Ruby: s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gfnxkxknw.sHtML

C#:   s.Length
来源：http://read.share.zdbjq.cn/Article/details/gpcblhwdn.sHtML

[A23] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gjogoygnw.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://m.share.hesvh.cn/Article/details/gadvquwqe.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fehbvm.com/Article/details/giktzcxwl.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.hesvh.cn/Article/details/gintbquup.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gggwcxmuh.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gmnilpuif.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://mobile.fehbvm.com/Article/details/gyqnvfqly.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gxrlmwabs.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.fehbvm.com/Article/details/gxzcmuvea.sHtML

[A24] 去除首尾空白
来源：http://read.share.hesvh.cn/Article/details/gfblcrhzh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://read.share.hesvh.cn/Article/details/gxxvlmbmi.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://wap.hesvh.cn/Article/details/gpdhmtfer.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/gutgfqvfb.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://read.share.fehbvm.com/Article/details/gejsefouo.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.fehbvm.com/Article/details/gqcpiijbw.sHtML

Go:   strings.TrimSpace(s)
来源：http://mobile.hesvh.cn/Article/details/gesxzbzzm.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.m.share.fehbvm.com/Article/details/gfowpikox.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://baike.fehbvm.com/Article/details/gxudboavx.sHtML

[A25] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gocrisvvs.sHtML

Py:   s1 == s2; s1 != s2
来源：http://blog.fehbvm.com/Article/details/gnotqerij.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.hesvh.cn/Article/details/ghgepnqda.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/giqgapjpl.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/ggojdfktm.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.hesvh.cn/Article/details/gtwlsuldo.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.zdbjq.cn/Article/details/gziudqyvn.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.blog.fehbvm.com/Article/details/gezpxwmvh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://m.share.fehbvm.com/Article/details/gulkatalm.sHtML

[A26] 类型转换总览
来源：http://baike.zdbjq.cn/Article/details/gccozncfo.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://blog.zdbjq.cn/Article/details/ggyrzuavz.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.blog.hesvh.cn/Article/details/gpbhrxdxi.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://mobile.hesvh.cn/Article/details/gonuupoby.sHtML

TS:   Number() String() Boolean() x as number
来源：http://www.share.hesvh.cn/Article/details/gyhtmthhv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://m.share.fehbvm.com/Article/details/grthcwhkj.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.zdbjq.cn/Article/details/gafbokjvc.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://wap.hesvh.cn/Article/details/gzgvwlpsb.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gzbomcnsj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkkbijndp.sHtML

B. 流程控制
来源：http://mobile.zdbjq.cn/Article/details/gdhdsowpr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggolxcizz.sHtML

[B01] 条件判断 if / else
来源：http://blog.fehbvm.com/Article/details/gavqdhvah.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://mobile.hesvh.cn/Article/details/gzapqmetv.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.fehbvm.com/Article/details/ggatjfwzy.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://mobile.zdbjq.cn/Article/details/grhvbyeov.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.hesvh.cn/Article/details/gizebyyne.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/grfupvvoi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://baike.zdbjq.cn/Article/details/gmszqgbza.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.fehbvm.com/Article/details/ghtvoaxsv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.fehbvm.com/Article/details/guthinyyo.sHtML

[B02] 多分支 else if / elif
来源：http://www.share.hesvh.cn/Article/details/ggklupuzu.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.fehbvm.com/Article/details/gifhkpben.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://wap.fehbvm.com/Article/details/gghrkzkmf.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.hesvh.cn/Article/details/gnejwksnt.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.zdbjq.cn/Article/details/guwafxlpe.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fehbvm.com/Article/details/gmebybbzg.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.fehbvm.com/Article/details/gvyuyxhjr.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.fehbvm.com/Article/details/gyqpeyhlg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.fehbvm.com/Article/details/gartfwczm.sHtML

[B03] switch / match / case
来源：http://m.share.zdbjq.cn/Article/details/gslcsthyz.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.m.share.fehbvm.com/Article/details/gitxgcjps.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://m.share.hesvh.cn/Article/details/gmazinser.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyjwwglvj.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gxxxotkmu.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.zdbjq.cn/Article/details/gqgddvmyq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://m.share.fehbvm.com/Article/details/gcixxpsfy.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.share.hesvh.cn/Article/details/gpsmhsdvg.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://3g.fehbvm.com/Article/details/gzrjjrguh.sHtML

[B04] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gbxwbrhep.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.zdbjq.cn/Article/details/gppasyckh.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.fehbvm.com/Article/details/gkbthrjas.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://3g.hesvh.cn/Article/details/gwnfcunoy.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.fehbvm.com/Article/details/gobaevyog.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.hesvh.cn/Article/details/ggfgghlcd.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://mobile.zdbjq.cn/Article/details/gpqijcmsw.sHtML

Ruby: 10.times { |i| puts i }
来源：http://blog.hesvh.cn/Article/details/gkxpolkua.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gzgpacyps.sHtML

[B05] 遍历数组 / 列表
来源：http://m.share.zdbjq.cn/Article/details/graptowew.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gqdzjzckg.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://m.share.hesvh.cn/Article/details/gvackngbr.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://m.share.hesvh.cn/Article/details/gwkaxcqur.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gqccoctte.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.blog.hesvh.cn/Article/details/gtgirbhkh.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://3g.hesvh.cn/Article/details/gjpwlaofs.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.hesvh.cn/Article/details/gosbsyzkl.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.hesvh.cn/Article/details/gfnlebbjq.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.hesvh.cn/Article/details/gtkgmdchk.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.hesvh.cn/Article/details/gfrueellf.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.zdbjq.cn/Article/details/gfakjqlao.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.blog.hesvh.cn/Article/details/gmskjnuyt.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.hesvh.cn/Article/details/gizjnpapl.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://read.share.hesvh.cn/Article/details/gikpommow.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.zdbjq.cn/Article/details/gtelguooj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://read.share.zdbjq.cn/Article/details/gumoqblkl.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fehbvm.com/Article/details/ggtusnkmu.sHtML

[B07] while 循环
来源：http://m.share.zdbjq.cn/Article/details/gtzbkkiwb.sHtML

Py:   while i < 10: i += 1
来源：http://baike.hesvh.cn/Article/details/gwnonynsm.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.fehbvm.com/Article/details/grqcwnzfo.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gaofxtjpj.sHtML

TS:   while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gwjnjcbpc.sHtML

Java: while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gsdmwfqyw.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/gplavsjbh.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.fehbvm.com/Article/details/gdnwaicmg.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gkivtlfpn.sHtML

[B08] do-while（至少执行一次）
来源：http://m.share.fehbvm.com/Article/details/gdsbqcump.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://baike.hesvh.cn/Article/details/gbmyeyxuw.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.blog.zdbjq.cn/Article/details/gyuzyqujt.sHtML

JS:   do { i++; } while (i < 10);
来源：http://mobile.hesvh.cn/Article/details/gjxnogqsb.sHtML

TS:   do { i++; } while (i < 10);
来源：http://blog.fehbvm.com/Article/details/gjuwyuyuu.sHtML

Java: do { i++; } while (i < 10);
来源：http://mobile.zdbjq.cn/Article/details/gtpjiflav.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.fehbvm.com/Article/details/gklnlhmkh.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.share.fehbvm.com/Article/details/gffcmblhr.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/ggkgdcquk.sHtML

[B09] break 与 continue
来源：http://blog.fehbvm.com/Article/details/gbcilkqvz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.hesvh.cn/Article/details/givacjscf.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/ggjiahksf.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gerkoaecu.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gwhtwhnss.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fehbvm.com/Article/details/grbfinetj.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.share.fehbvm.com/Article/details/gkumknuhc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://read.share.zdbjq.cn/Article/details/gmnuqlwij.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.zdbjq.cn/Article/details/gpbeaxhex.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gracggnee.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.hesvh.cn/Article/details/ghsqcnxdo.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gmzgjziem.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/gopjpvvuv.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.fehbvm.com/Article/details/ghcfyeceu.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.share.zdbjq.cn/Article/details/gtmdaqilk.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://baike.zdbjq.cn/Article/details/gvowxfqvr.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.m.share.fehbvm.com/Article/details/gzxsvuklc.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://mobile.fehbvm.com/Article/details/gvvnsiisb.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gdzwakyty.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fehbvm.com/Article/details/gemyhwxfc.sHtML

PHP:  range(0, 10, 2);
来源：http://www.share.fehbvm.com/Article/details/ghcuxygpw.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://m.share.zdbjq.cn/Article/details/gpevpkuzo.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gqpmvuhnr.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fehbvm.com/Article/details/gxrmremcv.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://baike.hesvh.cn/Article/details/gqsegqokb.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.hesvh.cn/Article/details/gtinduusm.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/goyxvtgxw.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.hesvh.cn/Article/details/guygvlkge.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.share.fehbvm.com/Article/details/gsnidtltz.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.zdbjq.cn/Article/details/gisbdhgyt.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.hesvh.cn/Article/details/gmkorzkxp.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/guxidldqe.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gcmfhvdgi.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.zdbjq.cn/Article/details/gsoepcykq.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.zdbjq.cn/Article/details/gpjpeqgvu.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gluevvvqi.sHtML

[B13] 判断是否为数字
来源：http://baike.fehbvm.com/Article/details/guwkavmyk.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.m.share.zdbjq.cn/Article/details/glmmxkpil.sHtML

PHP:  is_numeric($x)
来源：http://m.share.fehbvm.com/Article/details/ghpipkotx.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.zdbjq.cn/Article/details/gkwosytku.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gxvabpewu.sHtML

Java: x instanceof Number
来源：http://3g.fehbvm.com/Article/details/grhunofih.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://3g.hesvh.cn/Article/details/gocublume.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gbthdtsqk.sHtML

C#:   x is int or double or decimal
来源：http://blog.hesvh.cn/Article/details/gzdiywpui.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.zdbjq.cn/Article/details/gzlinukit.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.share.hesvh.cn/Article/details/gjfilwbbc.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://mobile.zdbjq.cn/Article/details/gmuuihjhg.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://wap.hesvh.cn/Article/details/gihedauov.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gahcmmhrq.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://m.share.hesvh.cn/Article/details/gdagyukoa.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/gyugpbolk.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://blog.zdbjq.cn/Article/details/gpckaomwp.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gvyvixxni.sHtML

[B15] 布尔运算与取反
来源：http://blog.hesvh.cn/Article/details/gtuohrdat.sHtML

Py:   a and b or not c
来源：http://m.share.hesvh.cn/Article/details/gxenxuqum.sHtML

PHP:  $a && $b || !$c
来源：http://mobile.fehbvm.com/Article/details/gmkvtxavh.sHtML

JS:   a && b || !c
来源：http://wap.hesvh.cn/Article/details/gdxgqgiqp.sHtML

TS:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gtncjltbe.sHtML

Java: a && b || !c
来源：http://3g.hesvh.cn/Article/details/gjiechkqx.sHtML

Go:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/glnsnrwag.sHtML

Ruby: a && b || !c
来源：http://m.share.zdbjq.cn/Article/details/gblizjxxi.sHtML

C#:   a && b || !c
来源：http://www.blog.fehbvm.com/Article/details/glzlgayce.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gijojyfli.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gkezpvdxn.sHtML

PHP:  if (!$data) { return; }
来源：http://wap.zdbjq.cn/Article/details/ggnrwbgkk.sHtML

JS:   if (!data) return;
来源：http://mobile.hesvh.cn/Article/details/gxoddccwi.sHtML

TS:   if (!data) return;
来源：http://www.blog.zdbjq.cn/Article/details/geizqllbi.sHtML

Java: if (data == null) return;
来源：http://mobile.hesvh.cn/Article/details/ganflmdko.sHtML

Go:   if data == nil { return }
来源：http://www.share.hesvh.cn/Article/details/gjtowoqjp.sHtML

Ruby: return if data.nil?
来源：http://3g.hesvh.cn/Article/details/ghptcvzde.sHtML

C#:   if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/guqfysxjn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gillhqkgn.sHtML

C. 函数与作用域
来源：http://www.m.share.zdbjq.cn/Article/details/gwpvhxdge.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gbpqaluyc.sHtML

[C01] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gwzfmiawi.sHtML

Py:   def add(a, b): return a + b
来源：http://3g.zdbjq.cn/Article/details/gwudxpzki.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.fehbvm.com/Article/details/gfemutfaw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://m.share.fehbvm.com/Article/details/gmyzzqsxu.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://3g.hesvh.cn/Article/details/gskqwatlj.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gnqdzkbip.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gnpuhcred.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fehbvm.com/Article/details/gzfjcvwwz.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.m.share.fehbvm.com/Article/details/gwupcjxcv.sHtML

[C02] 默认参数
来源：http://read.share.fehbvm.com/Article/details/gazcezzam.sHtML

Py:   def greet(name="World"): return name
来源：http://mobile.hesvh.cn/Article/details/grjxlvuzs.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://3g.zdbjq.cn/Article/details/gaqvanoyo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gazxromhx.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://read.share.fehbvm.com/Article/details/gssbzqbkf.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://3g.zdbjq.cn/Article/details/gppaifeic.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/gvznutfrn.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.zdbjq.cn/Article/details/gykrvyokh.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.fehbvm.com/Article/details/gxqfixfyx.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gbvyfgbmi.sHtML

Py:   def total(*args): return sum(args)
来源：http://blog.hesvh.cn/Article/details/gouvrhzdt.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.zdbjq.cn/Article/details/gxtcbwozy.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.zdbjq.cn/Article/details/gxsueflfc.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.hesvh.cn/Article/details/gimnldazm.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gicjizlhp.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.m.share.zdbjq.cn/Article/details/gtowkasor.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.zdbjq.cn/Article/details/gnpugqtwd.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://read.share.fehbvm.com/Article/details/gnzuehgbj.sHtML

[C04] 命名参数 / 关键字参数
来源：http://m.share.fehbvm.com/Article/details/guohtuajq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://read.share.zdbjq.cn/Article/details/gkaixmdzf.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.zdbjq.cn/Article/details/gmsioxdbb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.zdbjq.cn/Article/details/gnuoiudcc.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/grnunnlwg.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.zdbjq.cn/Article/details/ggkwvdtzl.sHtML


<!-- 参考信息 -->