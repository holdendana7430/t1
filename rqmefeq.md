代发 wailian999

TS:   // 单行；/* 多行 */
来源：http://3g.zdbjq.cn/Article/details/gdivkbyiw.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.hesvh.cn/Article/details/gprgdloox.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gzpuxtzfu.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://wap.fehbvm.com/Article/details/ghpufpepp.sHtML

C#:   // 单行；/* 多行 */
来源：http://m.share.hesvh.cn/Article/details/gthkrsygj.sHtML

[A15] 空值判断与默认值
来源：http://baike.zdbjq.cn/Article/details/glyongsyo.sHtML

Py:   value = data or "默认值"
来源：http://www.share.hesvh.cn/Article/details/gmtkulujd.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.blog.fehbvm.com/Article/details/gczeouzdm.sHtML

JS:   const value = data ?? "默认值";
来源：http://baike.zdbjq.cn/Article/details/ghauyoeay.sHtML

TS:   const value = data ?? "默认值";
来源：http://wap.fehbvm.com/Article/details/gvnboecmt.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://baike.hesvh.cn/Article/details/grdrytipy.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.blog.fehbvm.com/Article/details/gbxzxfnle.sHtML

Ruby: value = data || "默认值"
来源：http://www.share.fehbvm.com/Article/details/gbznhhfhd.sHtML

C#:   var value = data ?? "默认值";
来源：http://www.share.fehbvm.com/Article/details/gbbyxadux.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gzmphsrbg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://blog.fehbvm.com/Article/details/gtqdehufd.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://baike.fehbvm.com/Article/details/gogstfdkk.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://www.blog.hesvh.cn/Article/details/ggktbcifs.sHtML

TS:   if (!x) {}
来源：http://www.share.zdbjq.cn/Article/details/gjphgjazz.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://mobile.hesvh.cn/Article/details/gxbqprwwc.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.blog.fehbvm.com/Article/details/gjnelbgau.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://baike.fehbvm.com/Article/details/gmwjkejhn.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gnquhafbj.sHtML

[A17] 位运算
来源：http://baike.fehbvm.com/Article/details/genkmajon.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gxivnhncu.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.fehbvm.com/Article/details/gnrkidfma.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gxnqcqfcy.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://wap.fehbvm.com/Article/details/glcnvxfox.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gkihrsawl.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/gzladhhll.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://blog.zdbjq.cn/Article/details/gysbcmrii.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gcioagiew.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.hesvh.cn/Article/details/gpeyqkfbr.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.hesvh.cn/Article/details/gvmtbqvew.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.share.fehbvm.com/Article/details/gndlcbfzy.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.zdbjq.cn/Article/details/grxsgylst.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.fehbvm.com/Article/details/gntiusgsb.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.zdbjq.cn/Article/details/gvowucfgd.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fehbvm.com/Article/details/gnwaqaenu.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.m.share.hesvh.cn/Article/details/gfudmyprw.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.hesvh.cn/Article/details/gvjjbllqw.sHtML

[A19] 交换两个变量
来源：http://baike.zdbjq.cn/Article/details/gjkakqrpj.sHtML

Py:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gfejbjvgi.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://wap.hesvh.cn/Article/details/gztfhlxum.sHtML

JS:   [a, b] = [b, a];
来源：http://m.share.zdbjq.cn/Article/details/gbfezfsht.sHtML

TS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gpqgcsozk.sHtML

Java: int t = a; a = b; b = t;
来源：http://baike.fehbvm.com/Article/details/gnleksuzq.sHtML

Go:   a, b = b, a
来源：http://blog.hesvh.cn/Article/details/gkufertxp.sHtML

Ruby: a, b = b, a
来源：http://wap.hesvh.cn/Article/details/gtkyeusgq.sHtML

C#:   (a, b) = (b, a);
来源：http://www.blog.hesvh.cn/Article/details/gtxwdlduo.sHtML

[A20] 读取标准输入
来源：http://mobile.fehbvm.com/Article/details/gsxlpszlu.sHtML

Py:   name = input("请输入：")
来源：http://m.share.hesvh.cn/Article/details/gqhrzcctq.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.share.fehbvm.com/Article/details/gvktcwcdx.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://mobile.fehbvm.com/Article/details/ggjsclftk.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.hesvh.cn/Article/details/gkiyxwqqs.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.blog.fehbvm.com/Article/details/gafvdccjb.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.m.share.hesvh.cn/Article/details/geweabfgz.sHtML

Ruby: gets.chomp
来源：http://wap.hesvh.cn/Article/details/gcwbtafsg.sHtML

C#:   Console.ReadLine();
来源：http://3g.hesvh.cn/Article/details/glngdtwmx.sHtML

[A21] 保留指定小数位输出
来源：http://mobile.fehbvm.com/Article/details/gtababgkd.sHtML

Py:   f"{3.14159:.2f}"
来源：http://baike.zdbjq.cn/Article/details/gsznmxcrx.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/gvfpkwbeq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://blog.hesvh.cn/Article/details/gkevanfuv.sHtML

TS:   (3.14159).toFixed(2)
来源：http://wap.hesvh.cn/Article/details/gpyydulds.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://3g.hesvh.cn/Article/details/gtnfpdswu.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.hesvh.cn/Article/details/gduexpnny.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://3g.zdbjq.cn/Article/details/gacapsstm.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.hesvh.cn/Article/details/gzieqprut.sHtML

[A22] 获取字符串长度
来源：http://mobile.hesvh.cn/Article/details/gmnnmwsll.sHtML

Py:   len(s)
来源：http://m.share.fehbvm.com/Article/details/gbdwqkfiy.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.hesvh.cn/Article/details/gorcllqvz.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.share.zdbjq.cn/Article/details/gqcatoxwa.sHtML

TS:   s.length
来源：http://read.share.hesvh.cn/Article/details/gxjygbaye.sHtML

Java: s.length()
来源：http://baike.fehbvm.com/Article/details/geavykjqf.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.hesvh.cn/Article/details/gzmxcbbku.sHtML

Ruby: s.length
来源：http://www.m.share.fehbvm.com/Article/details/gahznwkfg.sHtML

C#:   s.Length
来源：http://www.share.hesvh.cn/Article/details/gnwihekhw.sHtML

[A23] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gqkhxkxjv.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://wap.fehbvm.com/Article/details/gduiepdrn.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fehbvm.com/Article/details/gcmtunhxz.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fehbvm.com/Article/details/gepmxaoao.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://3g.hesvh.cn/Article/details/grficgsty.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gygggaghp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.share.fehbvm.com/Article/details/guqxnfelt.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gxnfmqgle.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.share.zdbjq.cn/Article/details/ggvfsiwyz.sHtML

[A24] 去除首尾空白
来源：http://3g.fehbvm.com/Article/details/gulzwkvjh.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://mobile.zdbjq.cn/Article/details/gfkevxuwb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://read.share.hesvh.cn/Article/details/gvcbueimd.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://mobile.zdbjq.cn/Article/details/glsvmnnze.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gwpivmdpc.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://wap.zdbjq.cn/Article/details/glysjmydw.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.hesvh.cn/Article/details/gvnlqeunq.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.blog.fehbvm.com/Article/details/gdugprvun.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gbelvtwke.sHtML

[A25] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gchsamrkd.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.fehbvm.com/Article/details/gtgtfjqpf.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.share.fehbvm.com/Article/details/gccokagdb.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://blog.fehbvm.com/Article/details/gbyvtgfvz.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fehbvm.com/Article/details/gfcsivzoe.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://3g.fehbvm.com/Article/details/gnrpbcehy.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://blog.hesvh.cn/Article/details/gqkpimonc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://www.m.share.hesvh.cn/Article/details/geltgebdk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.hesvh.cn/Article/details/gywpttkhn.sHtML

[A26] 类型转换总览
来源：http://mobile.fehbvm.com/Article/details/ghrrsdkkn.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://wap.zdbjq.cn/Article/details/gacqvfmmr.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fehbvm.com/Article/details/gqfhumcue.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/glgewysbx.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fehbvm.com/Article/details/gujxmaqpo.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gmapxphit.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.share.fehbvm.com/Article/details/gonfwwiml.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.m.share.hesvh.cn/Article/details/gcsobebth.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/gflwborsr.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtojkdwfs.sHtML

B. 流程控制
来源：http://3g.fehbvm.com/Article/details/gvehrcdlm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjynfcmon.sHtML

[B01] 条件判断 if / else
来源：http://mobile.zdbjq.cn/Article/details/gnopaxasf.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://wap.hesvh.cn/Article/details/gyqoznklx.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.hesvh.cn/Article/details/gxvpwchqg.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.hesvh.cn/Article/details/glsjsvdho.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.zdbjq.cn/Article/details/guvvujdvo.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.zdbjq.cn/Article/details/gfwedaqbi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.m.share.hesvh.cn/Article/details/gsjgfcjnh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.share.hesvh.cn/Article/details/gfmvyciol.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/gfegxscdu.sHtML

[B02] 多分支 else if / elif
来源：http://3g.zdbjq.cn/Article/details/gpsvyyxlh.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.share.zdbjq.cn/Article/details/getqvmjxf.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.hesvh.cn/Article/details/gmbseshsd.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gdjwkhqur.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.fehbvm.com/Article/details/gilsqrzek.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.fehbvm.com/Article/details/grnrkwghq.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.hesvh.cn/Article/details/gaijbfmve.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://blog.hesvh.cn/Article/details/gjkighxmg.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.zdbjq.cn/Article/details/goafjdptp.sHtML

[B03] switch / match / case
来源：http://www.m.share.zdbjq.cn/Article/details/grlplysbq.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://read.share.fehbvm.com/Article/details/giuaehair.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxjrtpsnu.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://wap.hesvh.cn/Article/details/gzwsqjxiq.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gmeemlezx.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gjvazynoq.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.share.fehbvm.com/Article/details/goxdhpbbr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://mobile.fehbvm.com/Article/details/gzdbtftlr.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.hesvh.cn/Article/details/gvgslymjj.sHtML

[B04] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gggzhnimi.sHtML

Py:   for i in range(10): print(i)
来源：http://www.m.share.hesvh.cn/Article/details/gdjdtkndo.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://blog.hesvh.cn/Article/details/gojofuzxs.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.hesvh.cn/Article/details/gfrqcdqqi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.hesvh.cn/Article/details/gccxzoatm.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.share.zdbjq.cn/Article/details/gjzgmoamc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://wap.hesvh.cn/Article/details/gppdkfyoo.sHtML

Ruby: 10.times { |i| puts i }
来源：http://wap.zdbjq.cn/Article/details/gibaiaiix.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.hesvh.cn/Article/details/gqzssszrz.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.zdbjq.cn/Article/details/gllhzruok.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fehbvm.com/Article/details/gzozdbcia.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.fehbvm.com/Article/details/ggfaezvfy.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://blog.zdbjq.cn/Article/details/gigbheved.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fehbvm.com/Article/details/gkfeduqxd.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.m.share.hesvh.cn/Article/details/gwngzoahi.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.m.share.hesvh.cn/Article/details/georoqvbw.sHtML

Ruby: arr.each { |item| puts item }
来源：http://read.share.hesvh.cn/Article/details/gtvtqqykm.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.zdbjq.cn/Article/details/gvnrrovms.sHtML

[B06] 遍历字典 / 对象
来源：http://wap.hesvh.cn/Article/details/gimymsdum.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://read.share.zdbjq.cn/Article/details/gavgevxii.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.blog.hesvh.cn/Article/details/gucgiavvu.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.zdbjq.cn/Article/details/gmstnorro.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.zdbjq.cn/Article/details/gbxhsslvk.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://mobile.fehbvm.com/Article/details/gzlfxyxrw.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://read.share.fehbvm.com/Article/details/gqofradtf.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.blog.hesvh.cn/Article/details/gtvhucvna.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://blog.hesvh.cn/Article/details/ghltgnaap.sHtML

[B07] while 循环
来源：http://www.m.share.fehbvm.com/Article/details/gpnovkvbm.sHtML

Py:   while i < 10: i += 1
来源：http://wap.hesvh.cn/Article/details/gkrcbidij.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gbdkdlxrl.sHtML

JS:   while (i < 10) { i++; }
来源：http://baike.zdbjq.cn/Article/details/gpbtejuly.sHtML

TS:   while (i < 10) { i++; }
来源：http://blog.fehbvm.com/Article/details/gbznnxdeu.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/gmfmcohgk.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://wap.hesvh.cn/Article/details/gnvykdsff.sHtML

Ruby: while i < 10; i += 1; end
来源：http://baike.zdbjq.cn/Article/details/gmmidcwym.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gpvnzpgvl.sHtML

[B08] do-while（至少执行一次）
来源：http://wap.hesvh.cn/Article/details/gytdmkwye.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fehbvm.com/Article/details/gxbxziepa.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://read.share.fehbvm.com/Article/details/gvxhhuito.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/gphnicxiq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gkcykjiyw.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/ggciihazq.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.hesvh.cn/Article/details/glqbkrqvw.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.fehbvm.com/Article/details/glaqrcjge.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.zdbjq.cn/Article/details/gicjgswyk.sHtML

[B09] break 与 continue
来源：http://baike.fehbvm.com/Article/details/gfwucvvjt.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.blog.fehbvm.com/Article/details/gvpvplcbg.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.blog.zdbjq.cn/Article/details/gqejdpnig.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/goekgyzrc.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/grubokjcl.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gwljimhnv.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.zdbjq.cn/Article/details/gtlhisjfa.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.fehbvm.com/Article/details/gqetdevau.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/grpvhbiph.sHtML

[B10] 遍历同时拿索引
来源：http://blog.hesvh.cn/Article/details/gzuuzvwmy.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gysnugzfk.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.hesvh.cn/Article/details/gwmdjbyrh.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://baike.zdbjq.cn/Article/details/gwpfgmwrp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://blog.hesvh.cn/Article/details/ggpcyqqxi.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.blog.hesvh.cn/Article/details/gnwsevdke.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.fehbvm.com/Article/details/gdnjwkzfi.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.fehbvm.com/Article/details/giodfafwl.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.m.share.hesvh.cn/Article/details/giciishgz.sHtML

[B11] 生成数字序列 / 区间
来源：http://read.share.hesvh.cn/Article/details/gfinylrtr.sHtML

Py:   list(range(0, 10, 2))
来源：http://mobile.zdbjq.cn/Article/details/gfsmuuztu.sHtML

PHP:  range(0, 10, 2);
来源：http://read.share.zdbjq.cn/Article/details/gfvisdwpb.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gxzhdalgh.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://baike.zdbjq.cn/Article/details/gyudxpjzy.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://blog.hesvh.cn/Article/details/gykyqbckg.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.hesvh.cn/Article/details/grmrubczs.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.hesvh.cn/Article/details/gzleebgae.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fehbvm.com/Article/details/gqrsfdpiz.sHtML

[B12] 跳出多层循环
来源：http://m.share.fehbvm.com/Article/details/gnqsxsrnn.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.m.share.zdbjq.cn/Article/details/grhmubitw.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://blog.zdbjq.cn/Article/details/ghimqccwv.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://wap.zdbjq.cn/Article/details/gxznxjfgy.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gdggxlhfq.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gywowojni.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://m.share.hesvh.cn/Article/details/gddhcwkjl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://wap.hesvh.cn/Article/details/ghosbyfcx.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://mobile.hesvh.cn/Article/details/gfzxjouof.sHtML

[B13] 判断是否为数字
来源：http://www.share.fehbvm.com/Article/details/gjarprkpb.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gnitaipgz.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gpptctzmj.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.hesvh.cn/Article/details/gvbwnovdk.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://blog.hesvh.cn/Article/details/gsavxtvxs.sHtML

Java: x instanceof Number
来源：http://read.share.fehbvm.com/Article/details/gilazbylk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fehbvm.com/Article/details/gvpjhlizs.sHtML

Ruby: x.is_a?(Numeric)
来源：http://blog.zdbjq.cn/Article/details/gusaigulh.sHtML

C#:   x is int or double or decimal
来源：http://3g.zdbjq.cn/Article/details/gjenckxkj.sHtML

[B14] 判断值是否在集合内
来源：http://www.share.fehbvm.com/Article/details/giivugwdt.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gltusozzx.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.hesvh.cn/Article/details/goniwhfhj.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gqwveedvl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gfipjuedz.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gkgshivfj.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/guwbwfbxo.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://baike.zdbjq.cn/Article/details/gncoauknm.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gvoryhzct.sHtML

[B15] 布尔运算与取反
来源：http://m.share.fehbvm.com/Article/details/ggggrpnip.sHtML

Py:   a and b or not c
来源：http://wap.hesvh.cn/Article/details/gonovnguw.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gccbstcdz.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gtmqsrkpe.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gpgegnxtk.sHtML

Java: a && b || !c
来源：http://www.m.share.zdbjq.cn/Article/details/grxirfgpb.sHtML

Go:   a && b || !c
来源：http://read.share.fehbvm.com/Article/details/gathizbjy.sHtML

Ruby: a && b || !c
来源：http://baike.hesvh.cn/Article/details/gttupcuui.sHtML

C#:   a && b || !c
来源：http://baike.hesvh.cn/Article/details/gfwgygdia.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gmzmyjktc.sHtML

Py:   if not data: return
来源：http://baike.fehbvm.com/Article/details/geqgvyitq.sHtML

PHP:  if (!$data) { return; }
来源：http://read.share.zdbjq.cn/Article/details/glbrcnepx.sHtML

JS:   if (!data) return;
来源：http://baike.fehbvm.com/Article/details/gztzifxad.sHtML

TS:   if (!data) return;
来源：http://m.share.hesvh.cn/Article/details/gvetnhkch.sHtML

Java: if (data == null) return;
来源：http://wap.fehbvm.com/Article/details/gskvffcyx.sHtML

Go:   if data == nil { return }
来源：http://mobile.fehbvm.com/Article/details/gongcynus.sHtML

Ruby: return if data.nil?
来源：http://wap.zdbjq.cn/Article/details/gunqzhjvs.sHtML

C#:   if (data == null) return;
来源：http://mobile.fehbvm.com/Article/details/glhxgkzet.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gfspqqxaw.sHtML

C. 函数与作用域
来源：http://www.share.hesvh.cn/Article/details/gmltrkxxm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggddxpfxi.sHtML

[C01] 定义函数
来源：http://mobile.zdbjq.cn/Article/details/glgmaenxb.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/grxrofgxq.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://wap.hesvh.cn/Article/details/gxgkixenj.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gbiohtqtl.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.zdbjq.cn/Article/details/gevhdzyfn.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://read.share.fehbvm.com/Article/details/gplfmeilq.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.zdbjq.cn/Article/details/gckqbgfvl.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.hesvh.cn/Article/details/ghiugcxwo.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.hesvh.cn/Article/details/grbfygnhn.sHtML

[C02] 默认参数
来源：http://3g.zdbjq.cn/Article/details/gdylpurxd.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.hesvh.cn/Article/details/gmjjljdgc.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.share.zdbjq.cn/Article/details/gwyxenrnl.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.fehbvm.com/Article/details/glqlsgcpm.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gponouttw.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.hesvh.cn/Article/details/gmodnznws.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://wap.fehbvm.com/Article/details/gytwheppd.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.share.zdbjq.cn/Article/details/gpijqgbyl.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://wap.zdbjq.cn/Article/details/gfkxylixu.sHtML

[C03] 可变参数
来源：http://m.share.hesvh.cn/Article/details/gubpuevni.sHtML

Py:   def total(*args): return sum(args)
来源：http://3g.fehbvm.com/Article/details/gouloslit.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://blog.zdbjq.cn/Article/details/gyzijcirb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/grukfgkjq.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.hesvh.cn/Article/details/gmozhyals.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://3g.zdbjq.cn/Article/details/gmahybhbu.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://read.share.hesvh.cn/Article/details/gpkvlrjee.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.m.share.fehbvm.com/Article/details/gtsnjrayb.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.share.fehbvm.com/Article/details/gemtmxohy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fehbvm.com/Article/details/gdzhrvbcq.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://m.share.fehbvm.com/Article/details/gvorhhyzc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://read.share.hesvh.cn/Article/details/guuaxvubs.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://mobile.zdbjq.cn/Article/details/ggysityyw.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.hesvh.cn/Article/details/gipqqiuwf.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gtnqebmpu.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.zdbjq.cn/Article/details/ggpoxdsfg.sHtML

Ruby: f(a: 1, b: 2)
来源：http://3g.hesvh.cn/Article/details/gdoojpwme.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.blog.zdbjq.cn/Article/details/gzmmuxwfy.sHtML

[C05] 返回多个值
来源：http://mobile.fehbvm.com/Article/details/gfyoskupi.sHtML


<!-- 参考信息 -->