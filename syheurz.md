代发 wailian999

[A14] 注释写法
来源：http://baike.fehbvm.com/Article/details/gjrdudsux.sHtML

Py:   # 单行；三引号字符串可作多行说明
来源：http://mobile.hesvh.cn/Article/details/gvgwxcgus.sHtML

PHP:  // 或 # 单行；/* 多行 */
来源：http://read.share.hesvh.cn/Article/details/gmpxdzllm.sHtML

JS:   // 单行；/* 多行 */
来源：http://baike.hesvh.cn/Article/details/gwhemevuh.sHtML

TS:   // 单行；/* 多行 */
来源：http://wap.fehbvm.com/Article/details/gwizmoewq.sHtML

Java: // 单行；/* 多行 */；/** 文档注释 */
来源：http://blog.zdbjq.cn/Article/details/gfbpbazsp.sHtML

Go:   // 单行；/* 多行 */
来源：http://www.m.share.zdbjq.cn/Article/details/gupfgrvnk.sHtML

Ruby: # 单行；=begin 多行 =end
来源：http://www.blog.fehbvm.com/Article/details/gqechiycy.sHtML

C#:   // 单行；/* 多行 */
来源：http://www.blog.fehbvm.com/Article/details/gzwmswtdi.sHtML

[A15] 空值判断与默认值
来源：http://3g.zdbjq.cn/Article/details/gobycnmps.sHtML

Py:   value = data or "默认值"
来源：http://3g.fehbvm.com/Article/details/gdnjnwggj.sHtML

PHP:  $value = $data ?? "默认值";
来源：http://www.share.hesvh.cn/Article/details/gakntsbln.sHtML

JS:   const value = data ?? "默认值";
来源：http://mobile.fehbvm.com/Article/details/gqfafiwtm.sHtML

TS:   const value = data ?? "默认值";
来源：http://m.share.zdbjq.cn/Article/details/gjczhjqgk.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://read.share.fehbvm.com/Article/details/graizrwbm.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.zdbjq.cn/Article/details/gsrijzurv.sHtML

Ruby: value = data || "默认值"
来源：http://read.share.fehbvm.com/Article/details/gkvlluzvu.sHtML

C#:   var value = data ?? "默认值";
来源：http://blog.zdbjq.cn/Article/details/gqwswwecg.sHtML

[A16] 真假值判断规则
来源：http://wap.hesvh.cn/Article/details/gzpgygrpi.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.hesvh.cn/Article/details/ghutfvxwy.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://read.share.hesvh.cn/Article/details/gjffxbhbf.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://mobile.zdbjq.cn/Article/details/gvofzxken.sHtML

TS:   if (!x) {}
来源：http://www.share.fehbvm.com/Article/details/gndwarzgq.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://wap.zdbjq.cn/Article/details/gdurmsbwx.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://m.share.hesvh.cn/Article/details/gbrmmmare.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://m.share.fehbvm.com/Article/details/gfenplfni.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.share.hesvh.cn/Article/details/gmmgawzsf.sHtML

[A17] 位运算
来源：http://www.blog.fehbvm.com/Article/details/gfbtmzrcd.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gftdxrqnp.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://wap.hesvh.cn/Article/details/gyobdgwnm.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.hesvh.cn/Article/details/gdfeqvktv.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.share.zdbjq.cn/Article/details/gvfkpcueb.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/glvfstvjx.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://3g.zdbjq.cn/Article/details/gafmqpnva.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://m.share.hesvh.cn/Article/details/gkmcdsejm.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.zdbjq.cn/Article/details/gbtyxnzip.sHtML

[A18] 字符与 ASCII 码互转
来源：http://mobile.zdbjq.cn/Article/details/gzvbkqtxi.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gstshtcqz.sHtML

PHP:  ord("A"); chr(65)
来源：http://3g.hesvh.cn/Article/details/gbfwigkxe.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://3g.zdbjq.cn/Article/details/gljquwekc.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/ganeqfduk.sHtML

Java: (int) 'A'; (char) 65
来源：http://baike.fehbvm.com/Article/details/gmrpkxmtw.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.fehbvm.com/Article/details/gjnhpdxgb.sHtML

Ruby: "A".ord; 65.chr
来源：http://www.share.zdbjq.cn/Article/details/gmbojmibe.sHtML

C#:   (int)'A'; (char)65
来源：http://www.m.share.fehbvm.com/Article/details/gmvpqpiim.sHtML

[A19] 交换两个变量
来源：http://www.share.hesvh.cn/Article/details/gwsnyvsvc.sHtML

Py:   a, b = b, a
来源：http://www.blog.fehbvm.com/Article/details/ggtgdhzfx.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://3g.hesvh.cn/Article/details/gclohlzbo.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.fehbvm.com/Article/details/gmxsefoet.sHtML

TS:   [a, b] = [b, a];
来源：http://blog.hesvh.cn/Article/details/gxexzjuwn.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.m.share.zdbjq.cn/Article/details/gewkexxml.sHtML

Go:   a, b = b, a
来源：http://mobile.hesvh.cn/Article/details/gcwmejsyt.sHtML

Ruby: a, b = b, a
来源：http://3g.hesvh.cn/Article/details/glgbvgdwy.sHtML

C#:   (a, b) = (b, a);
来源：http://www.m.share.fehbvm.com/Article/details/gevlbehjg.sHtML

[A20] 读取标准输入
来源：http://read.share.zdbjq.cn/Article/details/gtfkctnvh.sHtML

Py:   name = input("请输入：")
来源：http://blog.zdbjq.cn/Article/details/gycfcxbvn.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.blog.zdbjq.cn/Article/details/ganguysss.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.m.share.zdbjq.cn/Article/details/gqchrffmg.sHtML

TS:   // Node.js：readline 模块
来源：http://www.share.fehbvm.com/Article/details/ghyozkqhr.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://read.share.fehbvm.com/Article/details/gyngkhbgz.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.zdbjq.cn/Article/details/gggydedrp.sHtML

Ruby: gets.chomp
来源：http://3g.zdbjq.cn/Article/details/gjmrhlgff.sHtML

C#:   Console.ReadLine();
来源：http://read.share.fehbvm.com/Article/details/gpeicaita.sHtML

[A21] 保留指定小数位输出
来源：http://baike.zdbjq.cn/Article/details/gknetlkxc.sHtML

Py:   f"{3.14159:.2f}"
来源：http://read.share.fehbvm.com/Article/details/gizovrwwt.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gwivwulad.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gmalnptlr.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gzptmxzka.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://blog.zdbjq.cn/Article/details/gisgznyxc.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://m.share.hesvh.cn/Article/details/gedjnsqqb.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://blog.fehbvm.com/Article/details/glevvgfmp.sHtML

C#:   3.14159.ToString("F2")
来源：http://blog.zdbjq.cn/Article/details/gyggatboi.sHtML

[A22] 获取字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gbzdhqzyb.sHtML

Py:   len(s)
来源：http://m.share.fehbvm.com/Article/details/gxzbahplm.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://wap.fehbvm.com/Article/details/gkhqqpxkf.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://3g.fehbvm.com/Article/details/gekwolquh.sHtML

TS:   s.length
来源：http://read.share.zdbjq.cn/Article/details/gpqosjdip.sHtML

Java: s.length()
来源：http://blog.hesvh.cn/Article/details/guojzfciu.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://baike.zdbjq.cn/Article/details/gakvbozwc.sHtML

Ruby: s.length
来源：http://wap.fehbvm.com/Article/details/gscoliffe.sHtML

C#:   s.Length
来源：http://blog.zdbjq.cn/Article/details/gznhgaojw.sHtML

[A23] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gvkiqgfjl.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gjcfxnvih.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://wap.zdbjq.cn/Article/details/geytxfant.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.zdbjq.cn/Article/details/gvpovcvsk.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://baike.fehbvm.com/Article/details/gvczvcdtd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.m.share.fehbvm.com/Article/details/gcutywtxp.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://read.share.hesvh.cn/Article/details/gduywdssh.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://3g.hesvh.cn/Article/details/ggqnedjsd.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://www.blog.hesvh.cn/Article/details/gejazzpvc.sHtML

[A24] 去除首尾空白
来源：http://3g.hesvh.cn/Article/details/gtpkavvgc.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.hesvh.cn/Article/details/gfmbmrcml.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/gkaquageq.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.fehbvm.com/Article/details/gphchydfq.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://baike.hesvh.cn/Article/details/geuchzxqk.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.share.fehbvm.com/Article/details/gvbdyeipk.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.zdbjq.cn/Article/details/gbikhvbcc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://baike.zdbjq.cn/Article/details/ghaftiyzz.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/glmsbvdji.sHtML

[A25] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gxqimdmtg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.share.zdbjq.cn/Article/details/gaqimnjwy.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://m.share.fehbvm.com/Article/details/gzczpadxa.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.fehbvm.com/Article/details/gilenbhqq.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/godpmbeqv.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.fehbvm.com/Article/details/guolfuybp.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/gnofageup.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.fehbvm.com/Article/details/ggrbmphlh.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://read.share.fehbvm.com/Article/details/gstszhegl.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/gdvubqdgi.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.m.share.hesvh.cn/Article/details/gpscirlss.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.hesvh.cn/Article/details/gmhtelzmb.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://3g.zdbjq.cn/Article/details/gezxdcwge.sHtML

TS:   Number() String() Boolean() x as number
来源：http://read.share.hesvh.cn/Article/details/gbbyxlmfm.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://baike.zdbjq.cn/Article/details/gjhyfnoyw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.zdbjq.cn/Article/details/ghoksclcv.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://baike.fehbvm.com/Article/details/gstbtkhfi.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.zdbjq.cn/Article/details/gjivnzlxv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxyfqsiap.sHtML

B. 流程控制
来源：http://www.share.zdbjq.cn/Article/details/giwokboop.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvuluicrs.sHtML

[B01] 条件判断 if / else
来源：http://mobile.fehbvm.com/Article/details/ggmhebxxn.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.zdbjq.cn/Article/details/gjpixmoge.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.share.hesvh.cn/Article/details/gaaictlxd.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.hesvh.cn/Article/details/glhexvrnt.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.blog.zdbjq.cn/Article/details/gorkhbhdn.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gfyzofgiw.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://m.share.fehbvm.com/Article/details/ggqmswbrh.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.blog.zdbjq.cn/Article/details/gdrgpiidx.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://mobile.hesvh.cn/Article/details/gbvnjvdyc.sHtML

[B02] 多分支 else if / elif
来源：http://blog.hesvh.cn/Article/details/gpgtumsep.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.fehbvm.com/Article/details/gflgygaqt.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://baike.hesvh.cn/Article/details/ggmnanygi.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.share.hesvh.cn/Article/details/gaiidvlqi.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gfiyyunga.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gkxdcilml.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://3g.hesvh.cn/Article/details/gksihjbrc.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://mobile.hesvh.cn/Article/details/gpseiqjbt.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gkbsckcxs.sHtML

[B03] switch / match / case
来源：http://wap.fehbvm.com/Article/details/gqszwruxb.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.share.zdbjq.cn/Article/details/gsyyrbnfw.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.blog.hesvh.cn/Article/details/gyhnnnnsm.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.fehbvm.com/Article/details/grrqctbwm.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gjdzgdzau.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gbnztwcwl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.hesvh.cn/Article/details/gktxevots.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.fehbvm.com/Article/details/ggvmtxroi.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://baike.fehbvm.com/Article/details/ghicwdunr.sHtML

[B04] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/ggvjvdoks.sHtML

Py:   for i in range(10): print(i)
来源：http://read.share.zdbjq.cn/Article/details/gedsezrfn.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.m.share.hesvh.cn/Article/details/gyuvgelbp.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.m.share.zdbjq.cn/Article/details/gglnyyzjj.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://blog.zdbjq.cn/Article/details/gptywgqon.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.m.share.fehbvm.com/Article/details/gkyygkest.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.hesvh.cn/Article/details/gwahafuwj.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.fehbvm.com/Article/details/guaupjsvj.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://mobile.hesvh.cn/Article/details/gqeyqjhde.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.hesvh.cn/Article/details/gdxkqebuz.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/gxhknnviq.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.hesvh.cn/Article/details/gwafjvdmm.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://3g.hesvh.cn/Article/details/gvrdcwamh.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fehbvm.com/Article/details/gjvrcajlx.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.hesvh.cn/Article/details/guhcpqeje.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.hesvh.cn/Article/details/giasplyzl.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.m.share.fehbvm.com/Article/details/gsukufgzz.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.zdbjq.cn/Article/details/ghmxduajt.sHtML

[B06] 遍历字典 / 对象
来源：http://blog.zdbjq.cn/Article/details/gtitpkeid.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.hesvh.cn/Article/details/gqozygkug.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://3g.hesvh.cn/Article/details/gkuckdbpf.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.share.fehbvm.com/Article/details/glaundlzc.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.zdbjq.cn/Article/details/grtbjjsso.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://wap.hesvh.cn/Article/details/ghhtyfhow.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.zdbjq.cn/Article/details/gnlszyduj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fehbvm.com/Article/details/gfihlshxx.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://read.share.zdbjq.cn/Article/details/gptzfvhgv.sHtML

[B07] while 循环
来源：http://wap.hesvh.cn/Article/details/gxmapzqec.sHtML

Py:   while i < 10: i += 1
来源：http://blog.zdbjq.cn/Article/details/gmzggubhx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fehbvm.com/Article/details/gzrvpfwxg.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gpkwjbqcz.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.zdbjq.cn/Article/details/gmltepmst.sHtML

Java: while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/gevwpdgba.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://blog.zdbjq.cn/Article/details/gtjvitltl.sHtML

Ruby: while i < 10; i += 1; end
来源：http://blog.fehbvm.com/Article/details/gijhwyusi.sHtML

C#:   while (i < 10) { i++; }
来源：http://www.share.fehbvm.com/Article/details/gidzmioov.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.hesvh.cn/Article/details/gtxorqgqg.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.share.zdbjq.cn/Article/details/gtkcbsluj.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.share.hesvh.cn/Article/details/gghnnejtb.sHtML

JS:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gylzcatmc.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gkitxvshu.sHtML

Java: do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gmiyzkyzd.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://mobile.fehbvm.com/Article/details/gggyjihak.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://blog.zdbjq.cn/Article/details/gxwpdqutg.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.blog.hesvh.cn/Article/details/gsmoawuqj.sHtML

[B09] break 与 continue
来源：http://baike.zdbjq.cn/Article/details/gfzqnwzzx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://wap.zdbjq.cn/Article/details/geghixnbx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/grpdzeaal.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/grllnubxz.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fehbvm.com/Article/details/giudlgbvj.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.zdbjq.cn/Article/details/gyogafhzg.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/ggljxvfxd.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.blog.hesvh.cn/Article/details/gpfdytbcb.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.hesvh.cn/Article/details/gxdbmljlb.sHtML

[B10] 遍历同时拿索引
来源：http://read.share.hesvh.cn/Article/details/grdftnbpb.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.fehbvm.com/Article/details/gspkznzdy.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://3g.fehbvm.com/Article/details/gkhmexhln.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.blog.zdbjq.cn/Article/details/glwizkerk.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.blog.fehbvm.com/Article/details/gglkhjymb.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://baike.hesvh.cn/Article/details/gxgeqymfn.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://mobile.hesvh.cn/Article/details/gqmqcvmlv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.blog.zdbjq.cn/Article/details/gahrlxbpu.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.zdbjq.cn/Article/details/gdjqkmgzu.sHtML

[B11] 生成数字序列 / 区间
来源：http://baike.fehbvm.com/Article/details/gdqmyvuta.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.share.fehbvm.com/Article/details/gmygnscrb.sHtML

PHP:  range(0, 10, 2);
来源：http://3g.fehbvm.com/Article/details/gthdpdglv.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gjgjykhrv.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.fehbvm.com/Article/details/gbppsbywm.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.zdbjq.cn/Article/details/glhjcsahc.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://3g.zdbjq.cn/Article/details/gpwowotkl.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.zdbjq.cn/Article/details/gxsexpwqa.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.zdbjq.cn/Article/details/gecstgmgy.sHtML

[B12] 跳出多层循环
来源：http://www.m.share.fehbvm.com/Article/details/gltkjtlub.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.hesvh.cn/Article/details/goyloohfv.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.blog.zdbjq.cn/Article/details/gcmsoqhvk.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fehbvm.com/Article/details/gvgsmttlu.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.zdbjq.cn/Article/details/gxbfgqxdv.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gsudxvlyk.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://3g.hesvh.cn/Article/details/gfqfxvndb.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gzrysginb.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.m.share.fehbvm.com/Article/details/gndderert.sHtML

[B13] 判断是否为数字
来源：http://wap.fehbvm.com/Article/details/gmbfaaizh.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/gkzwyftro.sHtML

PHP:  is_numeric($x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcpqcrchq.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.share.hesvh.cn/Article/details/gotmilsba.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.hesvh.cn/Article/details/gdmacoodq.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gfwtxsgbk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.blog.fehbvm.com/Article/details/grmygxffd.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gkdwrugkl.sHtML

C#:   x is int or double or decimal
来源：http://read.share.zdbjq.cn/Article/details/gfmfnhngy.sHtML

[B14] 判断值是否在集合内
来源：http://read.share.zdbjq.cn/Article/details/gsyvjvwku.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://wap.fehbvm.com/Article/details/geqensjfy.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.hesvh.cn/Article/details/gqpeitdyu.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://blog.fehbvm.com/Article/details/gdssiurko.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gyckccwxh.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.hesvh.cn/Article/details/ggauwnhhg.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://3g.fehbvm.com/Article/details/gyghqzxvy.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.zdbjq.cn/Article/details/glcvlaxpq.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gsyctkdfy.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/gbllfjrvh.sHtML

Py:   a and b or not c
来源：http://blog.zdbjq.cn/Article/details/gzwavsbvs.sHtML

PHP:  $a && $b || !$c
来源：http://wap.hesvh.cn/Article/details/gktcrvkic.sHtML

JS:   a && b || !c
来源：http://read.share.zdbjq.cn/Article/details/gkzreotso.sHtML

TS:   a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gbxxgskbp.sHtML

Java: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gdruzsoou.sHtML

Go:   a && b || !c
来源：http://m.share.hesvh.cn/Article/details/gpzzdmzwk.sHtML

Ruby: a && b || !c
来源：http://www.share.hesvh.cn/Article/details/gxqzinijx.sHtML

C#:   a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/glgeizghx.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gyhifanpn.sHtML

Py:   if not data: return
来源：http://read.share.zdbjq.cn/Article/details/gxrdcxspp.sHtML

PHP:  if (!$data) { return; }
来源：http://blog.zdbjq.cn/Article/details/gpbfbdvsi.sHtML

JS:   if (!data) return;
来源：http://www.share.hesvh.cn/Article/details/goguukuix.sHtML

TS:   if (!data) return;
来源：http://www.blog.hesvh.cn/Article/details/gxaysmdqt.sHtML

Java: if (data == null) return;
来源：http://www.blog.zdbjq.cn/Article/details/gofmghgqh.sHtML

Go:   if data == nil { return }
来源：http://www.blog.zdbjq.cn/Article/details/gwlycmnbu.sHtML

Ruby: return if data.nil?
来源：http://3g.fehbvm.com/Article/details/gbgccnfqg.sHtML

C#:   if (data == null) return;
来源：http://www.blog.fehbvm.com/Article/details/gxzbzntdk.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggkrgjmue.sHtML

C. 函数与作用域
来源：http://wap.zdbjq.cn/Article/details/glmkorkeo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzyceqprb.sHtML

[C01] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gmsqczhgv.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.zdbjq.cn/Article/details/gpsrhgauc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/golxznmfa.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fehbvm.com/Article/details/gktqfphdj.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://baike.hesvh.cn/Article/details/gtyisggfo.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.share.fehbvm.com/Article/details/gdxoiiplk.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://3g.fehbvm.com/Article/details/gnugluuir.sHtML

Ruby: def add(a, b); a + b; end
来源：http://m.share.zdbjq.cn/Article/details/geynspenk.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://baike.fehbvm.com/Article/details/gnetumzbh.sHtML

[C02] 默认参数
来源：http://read.share.hesvh.cn/Article/details/ghvlrycml.sHtML

Py:   def greet(name="World"): return name
来源：http://wap.zdbjq.cn/Article/details/gxeavdlul.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.fehbvm.com/Article/details/gojfdtkpv.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://mobile.hesvh.cn/Article/details/gdonzkkhj.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://blog.hesvh.cn/Article/details/gchmksmux.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.fehbvm.com/Article/details/gpigaojjl.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.fehbvm.com/Article/details/ggfoowluz.sHtML

Ruby: def greet(name = "World") = name
来源：http://wap.zdbjq.cn/Article/details/gyuvcroyn.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://read.share.fehbvm.com/Article/details/gmmdbgawr.sHtML

[C03] 可变参数
来源：http://m.share.fehbvm.com/Article/details/ggdxsyxek.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.hesvh.cn/Article/details/gbiaoenvg.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.blog.fehbvm.com/Article/details/gmuxhmlnv.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fehbvm.com/Article/details/gbfkytycb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gyvrmmlcr.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.zdbjq.cn/Article/details/gkvxflxtg.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.zdbjq.cn/Article/details/gvaeiztgi.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.hesvh.cn/Article/details/gjbyndyxo.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.hesvh.cn/Article/details/gxwjdbijy.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.m.share.fehbvm.com/Article/details/grfqwjzxh.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.blog.hesvh.cn/Article/details/gdufmlosm.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.m.share.zdbjq.cn/Article/details/gjjctpsdb.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://read.share.zdbjq.cn/Article/details/gndtxkxpe.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://mobile.zdbjq.cn/Article/details/gpsqeohyu.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://baike.zdbjq.cn/Article/details/gaoteowgt.sHtML


<!-- 参考信息 -->