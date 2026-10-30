代发 wailian999

JS:   const value = data ?? "默认值";
来源：http://m.share.fanxiaobao.xyz/Article/details/gimyvujdj.sHtML

TS:   const value = data ?? "默认值";
来源：http://read.share.fanxiaobao.xyz/Article/details/giyygonik.sHtML

Java: Objects.requireNonNullElse(data, "默认值")
来源：http://3g.fanxiaobao.xyz/Article/details/gqxmnzikn.sHtML

Go:   if data == "" { data = "默认值" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshkfrchc.sHtML

Ruby: value = data || "默认值"
来源：http://m.share.fanxiaobao.xyz/Article/details/gplcyofjc.sHtML

C#:   var value = data ?? "默认值";
来源：http://wap.fanxiaobao.xyz/Article/details/gfporyber.sHtML

[A16] 真假值判断规则
来源：http://baike.fanxiaobao.xyz/Article/details/gwttpxpcg.sHtML

Py:   if not x:        # 0 "" [] {} None 均为假
来源：http://baike.fanxiaobao.xyz/Article/details/gtagmvtdc.sHtML

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdurbmgm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.fanxiaobao.xyz/Article/details/guvkpsjdn.sHtML

TS:   if (!x) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnsrbixs.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjvtimvy.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfychxrcb.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjiznflow.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwcqodnb.sHtML

[A17] 位运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmzyvjra.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.fanxiaobao.xyz/Article/details/gemijtgbt.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbhcxfvt.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjsjzbrq.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqazrfnn.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fanxiaobao.xyz/Article/details/grffnlyki.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmdccyvp.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://3g.fanxiaobao.xyz/Article/details/gorsnbrsl.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fanxiaobao.xyz/Article/details/ghimliqkt.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.fanxiaobao.xyz/Article/details/gjgzyugpv.sHtML

Py:   ord("A"); chr(65)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcktultlk.sHtML

PHP:  ord("A"); chr(65)
来源：http://baike.fanxiaobao.xyz/Article/details/golifpift.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyjdqtpx.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcniasegx.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntvdfiif.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.share.fanxiaobao.xyz/Article/details/gibcibcaw.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.fanxiaobao.xyz/Article/details/gejtxzmps.sHtML

C#:   (int)'A'; (char)65
来源：http://3g.fanxiaobao.xyz/Article/details/gpbxqkjdt.sHtML

[A19] 交换两个变量
来源：http://3g.fanxiaobao.xyz/Article/details/gswqfnmff.sHtML

Py:   a, b = b, a
来源：http://3g.fanxiaobao.xyz/Article/details/gmxoevzsv.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamfinxwe.sHtML

JS:   [a, b] = [b, a];
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtadvggb.sHtML

TS:   [a, b] = [b, a];
来源：http://m.share.fanxiaobao.xyz/Article/details/gditgujwh.sHtML

Java: int t = a; a = b; b = t;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtactwygh.sHtML

Go:   a, b = b, a
来源：http://mobile.fanxiaobao.xyz/Article/details/gfijutmsq.sHtML

Ruby: a, b = b, a
来源：http://blog.fanxiaobao.xyz/Article/details/gcagcivzk.sHtML

C#:   (a, b) = (b, a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzykrljze.sHtML

[A20] 读取标准输入
来源：http://3g.fanxiaobao.xyz/Article/details/gmrhhpyji.sHtML

Py:   name = input("请输入：")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmfhgyqu.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqadkesoi.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcnhygjb.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkmsokux.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcgwqqdf.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://mobile.fanxiaobao.xyz/Article/details/goiajxksm.sHtML

Ruby: gets.chomp
来源：http://wap.fanxiaobao.xyz/Article/details/gjwifkath.sHtML

C#:   Console.ReadLine();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiupxcox.sHtML

[A21] 保留指定小数位输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzmhyuthl.sHtML

Py:   f"{3.14159:.2f}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpnyosjy.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtvbujawl.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqekrhsei.sHtML

TS:   (3.14159).toFixed(2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gigyrjvky.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://mobile.fanxiaobao.xyz/Article/details/grguxdcge.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://3g.fanxiaobao.xyz/Article/details/gimsgoucl.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyiqiimtn.sHtML

C#:   3.14159.ToString("F2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfnqeydp.sHtML

[A22] 获取字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ghldasmyj.sHtML

Py:   len(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gehrdpgua.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjfrdlhm.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbirsvjyb.sHtML

TS:   s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsqbeapo.sHtML

Java: s.length()
来源：http://wap.fanxiaobao.xyz/Article/details/gwndrbtjn.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gjiqjzpuf.sHtML

Ruby: s.length
来源：http://baike.fanxiaobao.xyz/Article/details/guhmxvdxp.sHtML

C#:   s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/grsnsqvwx.sHtML

[A23] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/greiqhpkq.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gfuthexlc.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzmwxgnp.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://wap.fanxiaobao.xyz/Article/details/grclegmis.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfyinalv.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://blog.fanxiaobao.xyz/Article/details/gjkleigqx.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmabqayhp.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/gnoinvomq.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://3g.fanxiaobao.xyz/Article/details/gpfljvtch.sHtML

[A24] 去除首尾空白
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhpulplp.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://3g.fanxiaobao.xyz/Article/details/gbzdsqewo.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gietzcemx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://m.share.fanxiaobao.xyz/Article/details/guqpcvbzc.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.fanxiaobao.xyz/Article/details/gxomazsro.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.blog.fanxiaobao.xyz/Article/details/glakrwwle.sHtML

Go:   strings.TrimSpace(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxgiiezba.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.share.fanxiaobao.xyz/Article/details/gundibgdg.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.share.fanxiaobao.xyz/Article/details/ggfjzjbxr.sHtML

[A25] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcbwyksv.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnqyunyem.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://blog.fanxiaobao.xyz/Article/details/gjltmvagm.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.fanxiaobao.xyz/Article/details/giakiqboy.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gkwlypqfi.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwexhkoj.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://wap.fanxiaobao.xyz/Article/details/gzexvdxxc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.fanxiaobao.xyz/Article/details/gxsbjrfwr.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://baike.fanxiaobao.xyz/Article/details/ggqjjyvpa.sHtML

[A26] 类型转换总览
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiyrkthr.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://baike.fanxiaobao.xyz/Article/details/gjtejkdfd.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://mobile.fanxiaobao.xyz/Article/details/gojhisoha.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrondvmu.sHtML

TS:   Number() String() Boolean() x as number
来源：http://baike.fanxiaobao.xyz/Article/details/grwzlfpym.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fanxiaobao.xyz/Article/details/grcfmsohb.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://3g.fanxiaobao.xyz/Article/details/gthkuicwy.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrhqmniw.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtolcxrla.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gtetvhhve.sHtML

B. 流程控制
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgzsxhos.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzbehsnzx.sHtML

[B01] 条件判断 if / else
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpieyuax.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://blog.fanxiaobao.xyz/Article/details/goomsfteo.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnytoutpr.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gposfzcqv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.fanxiaobao.xyz/Article/details/gjwbnvtjj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzzturph.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcdcknnn.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpdlbxqd.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhnlxeys.sHtML

[B02] 多分支 else if / elif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhdqlbgj.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://baike.fanxiaobao.xyz/Article/details/gjkagwwwn.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://blog.fanxiaobao.xyz/Article/details/glukkbaqn.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixggvxwy.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gcvlbegoa.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.fanxiaobao.xyz/Article/details/gebaqvbvy.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdbldcwb.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwnayqlw.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://baike.fanxiaobao.xyz/Article/details/gnmikbhnq.sHtML

[B03] switch / match / case
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpewydta.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://3g.fanxiaobao.xyz/Article/details/gtmjrkiak.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbewcofc.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtfkvsoy.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtuflvjdi.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gywukzbon.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfbylxnr.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://wap.fanxiaobao.xyz/Article/details/glociqwhp.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcudsiybb.sHtML

[B04] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/goufmcfdl.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fanxiaobao.xyz/Article/details/gmeikxiuc.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpsckwer.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.fanxiaobao.xyz/Article/details/gobnecqhi.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdkdukfg.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjprfmmg.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grigbbdve.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrdktxwp.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfrdcpou.sHtML

[B05] 遍历数组 / 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gkoijsbxj.sHtML

Py:   for item in arr: print(item)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzkzsijz.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjztngvak.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjgnaaen.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://wap.fanxiaobao.xyz/Article/details/gjpulskik.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdafmhqdk.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.share.fanxiaobao.xyz/Article/details/glpjqjaty.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fanxiaobao.xyz/Article/details/gpqbajynq.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gplhgydnj.sHtML

[B06] 遍历字典 / 对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhzvlppi.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://3g.fanxiaobao.xyz/Article/details/gczjyvqag.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gffrzkttw.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecnpgipp.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnedumyr.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gicwsujtn.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjypibcay.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwduixvu.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbefrwjb.sHtML

[B07] while 循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaavpscd.sHtML

Py:   while i < 10: i += 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfafvsnd.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzxamaxc.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyfvofez.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxpedgjiy.sHtML

Java: while (i < 10) { i++; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuuonwfz.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.fanxiaobao.xyz/Article/details/ggledrgkf.sHtML

Ruby: while i < 10; i += 1; end
来源：http://3g.fanxiaobao.xyz/Article/details/ggsuvynuw.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwfbhmjpp.sHtML

[B08] do-while（至少执行一次）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwbrcjoz.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://3g.fanxiaobao.xyz/Article/details/ggvgsiwkh.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpyrtkqzr.sHtML

JS:   do { i++; } while (i < 10);
来源：http://blog.fanxiaobao.xyz/Article/details/ghermqmhf.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtxuoojp.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdrokshb.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeakywtq.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fanxiaobao.xyz/Article/details/gkizthzuw.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.fanxiaobao.xyz/Article/details/gidrvqhdj.sHtML

[B09] break 与 continue
来源：http://3g.fanxiaobao.xyz/Article/details/gyxqzeeuz.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gispvpidz.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkueuniqa.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnxsmaqy.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://3g.fanxiaobao.xyz/Article/details/gwduznmmo.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscyvqrdc.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fanxiaobao.xyz/Article/details/gbymxwfrc.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://blog.fanxiaobao.xyz/Article/details/gfqkzvdsh.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawjhkkmd.sHtML

[B10] 遍历同时拿索引
来源：http://blog.fanxiaobao.xyz/Article/details/gfluhyfpi.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiyrqoaz.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnicviiz.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxrgehrc.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.fanxiaobao.xyz/Article/details/gkzxifltv.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fanxiaobao.xyz/Article/details/gnsacfcvw.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxutdttn.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://3g.fanxiaobao.xyz/Article/details/gocttbnmp.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://baike.fanxiaobao.xyz/Article/details/gyxmhylpk.sHtML

[B11] 生成数字序列 / 区间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhcrvhci.sHtML

Py:   list(range(0, 10, 2))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzkqttii.sHtML

PHP:  range(0, 10, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gurlmultz.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfvnungp.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://blog.fanxiaobao.xyz/Article/details/ghmionlbe.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwrflmnnz.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyqdglhy.sHtML

Ruby: (0...10).step(2).to_a
来源：http://www.share.fanxiaobao.xyz/Article/details/gljzoueuj.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://m.share.fanxiaobao.xyz/Article/details/gedtbxweb.sHtML

[B12] 跳出多层循环
来源：http://m.share.fanxiaobao.xyz/Article/details/grfcdijnk.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhnfheep.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://3g.fanxiaobao.xyz/Article/details/gjvduwhoy.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gndkqxshz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://blog.fanxiaobao.xyz/Article/details/gtertggvf.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzlttgss.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmmkxcik.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://3g.fanxiaobao.xyz/Article/details/gtqfzcwlv.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.fanxiaobao.xyz/Article/details/gdizumify.sHtML

[B13] 判断是否为数字
来源：http://3g.fanxiaobao.xyz/Article/details/gkqkfjnrj.sHtML

Py:   isinstance(x, (int, float))
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfxdoorl.sHtML

PHP:  is_numeric($x)
来源：http://baike.fanxiaobao.xyz/Article/details/gorbzigvg.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjvdglgc.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gashweujt.sHtML

Java: x instanceof Number
来源：http://read.share.fanxiaobao.xyz/Article/details/grwzkbafc.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgquiepm.sHtML

Ruby: x.is_a?(Numeric)
来源：http://baike.fanxiaobao.xyz/Article/details/glrinnrfe.sHtML

C#:   x is int or double or decimal
来源：http://read.share.fanxiaobao.xyz/Article/details/gerfwuqmw.sHtML

[B14] 判断值是否在集合内
来源：http://m.share.fanxiaobao.xyz/Article/details/gfssklqwd.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaijzwppi.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://3g.fanxiaobao.xyz/Article/details/gevdufxqe.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfhqamfm.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/grgwonkqa.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuqkuclo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnionuios.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxghdianw.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/glizucbek.sHtML

[B15] 布尔运算与取反
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmgjhtzu.sHtML

Py:   a and b or not c
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkzjnqqb.sHtML

PHP:  $a && $b || !$c
来源：http://www.share.fanxiaobao.xyz/Article/details/ghoegvlgj.sHtML

JS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztmamqfl.sHtML

TS:   a && b || !c
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqgbordri.sHtML

Java: a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/gyjartrbm.sHtML

Go:   a && b || !c
来源：http://blog.fanxiaobao.xyz/Article/details/ggchhpjck.sHtML

Ruby: a && b || !c
来源：http://mobile.fanxiaobao.xyz/Article/details/gnobzlfuw.sHtML

C#:   a && b || !c
来源：http://3g.fanxiaobao.xyz/Article/details/gneiqsoag.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqoakagcj.sHtML

Py:   if not data: return
来源：http://m.share.fanxiaobao.xyz/Article/details/geuxjfcmh.sHtML

PHP:  if (!$data) { return; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gickceygr.sHtML

JS:   if (!data) return;
来源：http://baike.fanxiaobao.xyz/Article/details/glzvnqzmq.sHtML

TS:   if (!data) return;
来源：http://blog.fanxiaobao.xyz/Article/details/gibyoibpd.sHtML

Java: if (data == null) return;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssqliula.sHtML

Go:   if data == nil { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gpymruern.sHtML

Ruby: return if data.nil?
来源：http://wap.fanxiaobao.xyz/Article/details/gbdrtfmxk.sHtML

C#:   if (data == null) return;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvouxpzis.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gbrzqlcil.sHtML

C. 函数与作用域
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdwkbuov.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guterstxc.sHtML

[C01] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gfvuakouz.sHtML

Py:   def add(a, b): return a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/givmbpfen.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmklsaofd.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcraiyup.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyuddzvnq.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtlcfobu.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gxriohqaa.sHtML

Ruby: def add(a, b); a + b; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyscyfzp.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghneeqyml.sHtML

[C02] 默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/gqtaomowr.sHtML

Py:   def greet(name="World"): return name
来源：http://www.share.fanxiaobao.xyz/Article/details/gmrwypsis.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gnibzbdgo.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grlplxqvf.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqlbilrdc.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.fanxiaobao.xyz/Article/details/gckuzncrz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtforvldy.sHtML

Ruby: def greet(name = "World") = name
来源：http://mobile.fanxiaobao.xyz/Article/details/gelaabpyq.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaowsrdy.sHtML

[C03] 可变参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goshynswk.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrpuuhqk.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://3g.fanxiaobao.xyz/Article/details/gxdanormb.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.fanxiaobao.xyz/Article/details/glvmacgbr.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gozoddwyv.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gksgelnho.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://baike.fanxiaobao.xyz/Article/details/gqdgkzhgd.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://wap.fanxiaobao.xyz/Article/details/gjvmqmnsq.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggonxjxnp.sHtML

[C04] 命名参数 / 关键字参数
来源：http://blog.fanxiaobao.xyz/Article/details/gwhbmdcxt.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.fanxiaobao.xyz/Article/details/gwmzjbvfb.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjvepamj.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://blog.fanxiaobao.xyz/Article/details/geqvzhgvd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/giisklyrx.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.share.fanxiaobao.xyz/Article/details/gxusagvel.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.fanxiaobao.xyz/Article/details/gzszkgdof.sHtML

Ruby: f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjahzypp.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrcxlezu.sHtML

[C05] 返回多个值
来源：http://mobile.fanxiaobao.xyz/Article/details/gckqvixua.sHtML

Py:   return a, b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkqxmscz.sHtML

PHP:  return [$a, $b];
来源：http://baike.fanxiaobao.xyz/Article/details/guywgkibs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.fanxiaobao.xyz/Article/details/ggbivtboy.sHtML

TS:   return { a, b };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhodzgkp.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://baike.fanxiaobao.xyz/Article/details/gkshktgdg.sHtML

Go:   return a, b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihzbjiwh.sHtML

Ruby: return a, b
来源：http://3g.fanxiaobao.xyz/Article/details/gvcoesljr.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://mobile.fanxiaobao.xyz/Article/details/gkeqyrxyu.sHtML


<!-- 参考信息 -->