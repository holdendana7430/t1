代发 wailian999

[A18] 字符与 ASCII 码互转
来源：http://m.share.fehbvm.com/Article/details/gauwzcnqe.sHtML

Py:   ord("A"); chr(65)
来源：http://www.blog.zdbjq.cn/Article/details/gynvhelxu.sHtML

PHP:  ord("A"); chr(65)
来源：http://m.share.fehbvm.com/Article/details/gugddiqle.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://mobile.fehbvm.com/Article/details/gxojydusq.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://blog.hesvh.cn/Article/details/gszvjbtjd.sHtML

Java: (int) 'A'; (char) 65
来源：http://blog.zdbjq.cn/Article/details/gogbbauyq.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://blog.hesvh.cn/Article/details/gwzkqydfm.sHtML

Ruby: "A".ord; 65.chr
来源：http://m.share.fehbvm.com/Article/details/gjirefnjp.sHtML

C#:   (int)'A'; (char)65
来源：http://read.share.fehbvm.com/Article/details/gqodkzszz.sHtML

[A19] 交换两个变量
来源：http://wap.fehbvm.com/Article/details/gtbutfkag.sHtML

Py:   a, b = b, a
来源：http://blog.zdbjq.cn/Article/details/gbnhxlfnc.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://blog.hesvh.cn/Article/details/gxdihddfy.sHtML

JS:   [a, b] = [b, a];
来源：http://3g.zdbjq.cn/Article/details/grsehvxhk.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.zdbjq.cn/Article/details/gpogrizwf.sHtML

Java: int t = a; a = b; b = t;
来源：http://m.share.zdbjq.cn/Article/details/gposocrwd.sHtML

Go:   a, b = b, a
来源：http://baike.fehbvm.com/Article/details/gmwnvcqzb.sHtML

Ruby: a, b = b, a
来源：http://wap.zdbjq.cn/Article/details/gcmrrpylb.sHtML

C#:   (a, b) = (b, a);
来源：http://wap.fehbvm.com/Article/details/gtstybxpf.sHtML

[A20] 读取标准输入
来源：http://www.share.zdbjq.cn/Article/details/grwuaeocy.sHtML

Py:   name = input("请输入：")
来源：http://mobile.fehbvm.com/Article/details/guiuuvklj.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://www.m.share.hesvh.cn/Article/details/gmzlhzxzd.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.share.hesvh.cn/Article/details/gckihtfkd.sHtML

TS:   // Node.js：readline 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gpgkxjiln.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://m.share.hesvh.cn/Article/details/gykzflpvv.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://blog.hesvh.cn/Article/details/gcascgkqy.sHtML

Ruby: gets.chomp
来源：http://www.share.zdbjq.cn/Article/details/gixxqewqb.sHtML

C#:   Console.ReadLine();
来源：http://mobile.hesvh.cn/Article/details/gdkndicms.sHtML

[A21] 保留指定小数位输出
来源：http://read.share.fehbvm.com/Article/details/gmxpmypdx.sHtML

Py:   f"{3.14159:.2f}"
来源：http://wap.fehbvm.com/Article/details/gvieomiwz.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://wap.hesvh.cn/Article/details/gizzhsyfq.sHtML

JS:   (3.14159).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gdoeafdan.sHtML

TS:   (3.14159).toFixed(2)
来源：http://baike.hesvh.cn/Article/details/gmajxocgj.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://www.m.share.fehbvm.com/Article/details/gnijcajzy.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://wap.zdbjq.cn/Article/details/gycdbbuih.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://mobile.zdbjq.cn/Article/details/gcpjhwdrf.sHtML

C#:   3.14159.ToString("F2")
来源：http://read.share.hesvh.cn/Article/details/gzvfcixst.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/gfylrdjdl.sHtML

Py:   len(s)
来源：http://wap.hesvh.cn/Article/details/gnknqjrfl.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://read.share.fehbvm.com/Article/details/gvbfuvvbh.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.fehbvm.com/Article/details/gxvvecxvs.sHtML

TS:   s.length
来源：http://m.share.fehbvm.com/Article/details/gwcquxich.sHtML

Java: s.length()
来源：http://read.share.zdbjq.cn/Article/details/gdkwqvypw.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://3g.fehbvm.com/Article/details/gjihugfuh.sHtML

Ruby: s.length
来源：http://wap.hesvh.cn/Article/details/gtiwkvpzq.sHtML

C#:   s.Length
来源：http://mobile.hesvh.cn/Article/details/givpnciyz.sHtML

[A23] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gsflmpinb.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://mobile.hesvh.cn/Article/details/gsbwjhsgd.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.blog.fehbvm.com/Article/details/ghoeiydam.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.zdbjq.cn/Article/details/gpenxwhhe.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.share.zdbjq.cn/Article/details/gdbyailtl.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://m.share.fehbvm.com/Article/details/grklsetfl.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://3g.hesvh.cn/Article/details/gmcielupl.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gblkxrupr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.zdbjq.cn/Article/details/gbtavpidh.sHtML

[A24] 去除首尾空白
来源：http://mobile.zdbjq.cn/Article/details/gcocvmiuo.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://blog.zdbjq.cn/Article/details/geklseilz.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.hesvh.cn/Article/details/gzzkvipxp.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.hesvh.cn/Article/details/gdpcjevfd.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://wap.hesvh.cn/Article/details/gsjhrxntl.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://blog.hesvh.cn/Article/details/glxnyzepy.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtqsulqb.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://blog.zdbjq.cn/Article/details/grmftauqt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.zdbjq.cn/Article/details/givrtqezn.sHtML

[A25] 字符串比较
来源：http://baike.hesvh.cn/Article/details/ghwgxohxg.sHtML

Py:   s1 == s2; s1 != s2
来源：http://m.share.hesvh.cn/Article/details/gzyuhkuhq.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://wap.hesvh.cn/Article/details/gwypnoldj.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://read.share.zdbjq.cn/Article/details/gwhtvgahr.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://baike.hesvh.cn/Article/details/gpnuepamh.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/gzwhqisvf.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/glhiezmoc.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://3g.zdbjq.cn/Article/details/gynxdmgfz.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpgitsrus.sHtML

[A26] 类型转换总览
来源：http://wap.hesvh.cn/Article/details/gzwqjfeqh.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.blog.fehbvm.com/Article/details/gxvpanqot.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://wap.hesvh.cn/Article/details/gexuvbuut.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.m.share.zdbjq.cn/Article/details/goymjzyas.sHtML

TS:   Number() String() Boolean() x as number
来源：http://wap.zdbjq.cn/Article/details/ggmooytys.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://3g.hesvh.cn/Article/details/gipxmwyof.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://read.share.hesvh.cn/Article/details/ghpwnddzr.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.share.hesvh.cn/Article/details/gqdwmvlki.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkykwkbu.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gyhggxtvl.sHtML

B. 流程控制
来源：http://m.share.hesvh.cn/Article/details/gpjwckmuq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gschkszuk.sHtML

[B01] 条件判断 if / else
来源：http://wap.fehbvm.com/Article/details/gsaiyaltp.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://m.share.fehbvm.com/Article/details/gfgqfahzn.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://3g.zdbjq.cn/Article/details/gvbjvlkrs.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://wap.hesvh.cn/Article/details/gkvpmtlqv.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://blog.fehbvm.com/Article/details/gmlnestqr.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.fehbvm.com/Article/details/gbkxgfesp.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.hesvh.cn/Article/details/gkcbjlhoy.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://read.share.fehbvm.com/Article/details/gygidyeye.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://3g.fehbvm.com/Article/details/gsldnyvse.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.zdbjq.cn/Article/details/ghkpblyme.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfnkqyoy.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbxbiomqp.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://mobile.zdbjq.cn/Article/details/guutkhzzw.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gvuchbuda.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.hesvh.cn/Article/details/gjzvvizju.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.blog.zdbjq.cn/Article/details/gfcmixvzw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.blog.fehbvm.com/Article/details/gdjwwviai.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://blog.hesvh.cn/Article/details/gibizykzb.sHtML

[B03] switch / match / case
来源：http://m.share.hesvh.cn/Article/details/gtzezowyh.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.fehbvm.com/Article/details/gkddcwovp.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/glcmhftye.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.share.fehbvm.com/Article/details/gwgfkfshv.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://read.share.zdbjq.cn/Article/details/gzebjbxil.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.hesvh.cn/Article/details/gbuswplmn.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gsxbxwwqe.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/ggvpwtmjz.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://blog.fehbvm.com/Article/details/gzufarrxg.sHtML

[B04] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gxyvserkr.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.fehbvm.com/Article/details/gnsjexkhs.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://3g.zdbjq.cn/Article/details/gkyeoevqc.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gtgqxysur.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://baike.zdbjq.cn/Article/details/ggnokkgra.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://blog.zdbjq.cn/Article/details/glxsyoabc.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.m.share.zdbjq.cn/Article/details/gtbxrglau.sHtML

Ruby: 10.times { |i| puts i }
来源：http://mobile.hesvh.cn/Article/details/gzzhycwhd.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://3g.fehbvm.com/Article/details/gvrlrhkpv.sHtML

[B05] 遍历数组 / 列表
来源：http://www.m.share.hesvh.cn/Article/details/glrqffcvo.sHtML

Py:   for item in arr: print(item)
来源：http://blog.zdbjq.cn/Article/details/glydvyunu.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://baike.zdbjq.cn/Article/details/ggtqchona.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gejznoymp.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://baike.fehbvm.com/Article/details/gruaequdv.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://baike.zdbjq.cn/Article/details/gcidzyevy.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gduvwickk.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.share.fehbvm.com/Article/details/gveuixbtu.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://baike.zdbjq.cn/Article/details/gydgdtgbj.sHtML

[B06] 遍历字典 / 对象
来源：http://read.share.zdbjq.cn/Article/details/gdjzeatym.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://baike.zdbjq.cn/Article/details/gdfdqzpri.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.share.fehbvm.com/Article/details/ggrzfydxx.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://m.share.fehbvm.com/Article/details/gjsupumyf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.fehbvm.com/Article/details/gidmchtok.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.zdbjq.cn/Article/details/ganagelvu.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://3g.fehbvm.com/Article/details/githfnzcj.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.share.zdbjq.cn/Article/details/gubncnpox.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://3g.fehbvm.com/Article/details/gzymgjljw.sHtML

[B07] while 循环
来源：http://wap.zdbjq.cn/Article/details/gxncpqedi.sHtML

Py:   while i < 10: i += 1
来源：http://www.blog.fehbvm.com/Article/details/gvtdkpqxj.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://www.m.share.hesvh.cn/Article/details/gdioedzbs.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/guzdmvuyp.sHtML

TS:   while (i < 10) { i++; }
来源：http://read.share.zdbjq.cn/Article/details/gpkqdiyob.sHtML

Java: while (i < 10) { i++; }
来源：http://baike.hesvh.cn/Article/details/gjsifkhcv.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://baike.zdbjq.cn/Article/details/grcozqxuk.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gbcawpryo.sHtML

C#:   while (i < 10) { i++; }
来源：http://blog.zdbjq.cn/Article/details/ghlbiwftj.sHtML

[B08] do-while（至少执行一次）
来源：http://read.share.fehbvm.com/Article/details/gxjkqptrf.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://wap.hesvh.cn/Article/details/gmyvpkcat.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.zdbjq.cn/Article/details/gmtjcncpl.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.blog.fehbvm.com/Article/details/goiucfxlk.sHtML

TS:   do { i++; } while (i < 10);
来源：http://m.share.fehbvm.com/Article/details/guejabudj.sHtML

Java: do { i++; } while (i < 10);
来源：http://blog.zdbjq.cn/Article/details/gysmqcclr.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://www.m.share.hesvh.cn/Article/details/gavzzhbyd.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://www.m.share.zdbjq.cn/Article/details/gurboxisn.sHtML

C#:   do { i++; } while (i < 10);
来源：http://m.share.hesvh.cn/Article/details/gowrvbrlp.sHtML

[B09] break 与 continue
来源：http://www.m.share.hesvh.cn/Article/details/gmulfaacp.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://3g.hesvh.cn/Article/details/gvcxxioux.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://read.share.hesvh.cn/Article/details/gxmuwpgef.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.fehbvm.com/Article/details/gplpulqzf.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.share.hesvh.cn/Article/details/gfueinhvx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://wap.fehbvm.com/Article/details/gfwzmulrh.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://m.share.hesvh.cn/Article/details/gekirhfdu.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.m.share.hesvh.cn/Article/details/glwrwlbay.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzownslsi.sHtML

[B10] 遍历同时拿索引
来源：http://3g.zdbjq.cn/Article/details/gnmxcvxii.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.m.share.zdbjq.cn/Article/details/getkhgrpm.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.blog.fehbvm.com/Article/details/gdzfmridg.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://wap.fehbvm.com/Article/details/grkzhhsuy.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://wap.hesvh.cn/Article/details/gtvzyjagx.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://3g.fehbvm.com/Article/details/gcrekdwnu.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/gkfpeynqv.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://read.share.hesvh.cn/Article/details/gyxcgumvs.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://read.share.hesvh.cn/Article/details/gafnsytbt.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.fehbvm.com/Article/details/glzpczely.sHtML

Py:   list(range(0, 10, 2))
来源：http://read.share.fehbvm.com/Article/details/gyaiyvxxj.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gstpmcsgq.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.zdbjq.cn/Article/details/gippgaouz.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.fehbvm.com/Article/details/ggrjgmhcz.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.share.fehbvm.com/Article/details/gcwikswis.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://wap.hesvh.cn/Article/details/gwupxbpau.sHtML

Ruby: (0...10).step(2).to_a
来源：http://blog.zdbjq.cn/Article/details/gugbskupt.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.blog.hesvh.cn/Article/details/gxkgjiyqw.sHtML

[B12] 跳出多层循环
来源：http://mobile.zdbjq.cn/Article/details/gajwwrtkc.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://read.share.zdbjq.cn/Article/details/geuynlwgm.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gwztclpqe.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.hesvh.cn/Article/details/gxvmvxgiz.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.share.zdbjq.cn/Article/details/gggkuoczn.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://m.share.hesvh.cn/Article/details/gkugrljpw.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.hesvh.cn/Article/details/gnkafwznh.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.zdbjq.cn/Article/details/grktsfnaf.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gmmnvwhcn.sHtML

[B13] 判断是否为数字
来源：http://wap.hesvh.cn/Article/details/gdwgjfqzz.sHtML

Py:   isinstance(x, (int, float))
来源：http://www.blog.zdbjq.cn/Article/details/gviacwxeq.sHtML

PHP:  is_numeric($x)
来源：http://www.share.zdbjq.cn/Article/details/gtyjnundp.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://m.share.zdbjq.cn/Article/details/gvqpryhka.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.zdbjq.cn/Article/details/gpurkbnzo.sHtML

Java: x instanceof Number
来源：http://mobile.zdbjq.cn/Article/details/gkrimytdm.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gucnisxey.sHtML

Ruby: x.is_a?(Numeric)
来源：http://mobile.hesvh.cn/Article/details/gxtwbutsi.sHtML

C#:   x is int or double or decimal
来源：http://wap.fehbvm.com/Article/details/gvmtprftu.sHtML

[B14] 判断值是否在集合内
来源：http://www.blog.hesvh.cn/Article/details/gtuqmtynb.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://baike.hesvh.cn/Article/details/gcivjbggs.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.blog.fehbvm.com/Article/details/gfiuhsppt.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/ghbnodjmg.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/gcqvvwask.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://read.share.hesvh.cn/Article/details/glesptzcf.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gcghjbgur.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://wap.fehbvm.com/Article/details/gndnjtkwt.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gmdykfkdm.sHtML

[B15] 布尔运算与取反
来源：http://www.blog.fehbvm.com/Article/details/grdgohvop.sHtML

Py:   a and b or not c
来源：http://www.m.share.zdbjq.cn/Article/details/gucoyjuxa.sHtML

PHP:  $a && $b || !$c
来源：http://www.m.share.fehbvm.com/Article/details/gruhlemxs.sHtML

JS:   a && b || !c
来源：http://3g.fehbvm.com/Article/details/gnxmxyjfd.sHtML

TS:   a && b || !c
来源：http://www.m.share.hesvh.cn/Article/details/gnlerrjjp.sHtML

Java: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/gfuywdmkj.sHtML

Go:   a && b || !c
来源：http://www.blog.zdbjq.cn/Article/details/gkublwpkc.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gfcjqhqqa.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gxomyscyz.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://m.share.fehbvm.com/Article/details/guftrecke.sHtML

Py:   if not data: return
来源：http://www.blog.hesvh.cn/Article/details/gnqnmeqpy.sHtML

PHP:  if (!$data) { return; }
来源：http://m.share.zdbjq.cn/Article/details/gjcwzyixl.sHtML

JS:   if (!data) return;
来源：http://www.share.fehbvm.com/Article/details/gjmuicdyz.sHtML

TS:   if (!data) return;
来源：http://baike.hesvh.cn/Article/details/gducfpjqb.sHtML

Java: if (data == null) return;
来源：http://blog.hesvh.cn/Article/details/gxpusfqoh.sHtML

Go:   if data == nil { return }
来源：http://3g.fehbvm.com/Article/details/ggkywujer.sHtML

Ruby: return if data.nil?
来源：http://blog.fehbvm.com/Article/details/gsjasxkiu.sHtML

C#:   if (data == null) return;
来源：http://baike.fehbvm.com/Article/details/gxfilikiz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gglmhzuyw.sHtML

C. 函数与作用域
来源：http://www.blog.zdbjq.cn/Article/details/gxnwwiacc.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtopkkkwf.sHtML

[C01] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gsywtvnhp.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.fehbvm.com/Article/details/ghnzadnyw.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gqhrecyjy.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://3g.zdbjq.cn/Article/details/gmuvnomea.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://wap.hesvh.cn/Article/details/gmbaymrcs.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://3g.fehbvm.com/Article/details/gieeibodn.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://wap.hesvh.cn/Article/details/gxhyyixwv.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.fehbvm.com/Article/details/gmblletzr.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://mobile.hesvh.cn/Article/details/gteqfwknv.sHtML

[C02] 默认参数
来源：http://mobile.fehbvm.com/Article/details/gqbhecgim.sHtML

Py:   def greet(name="World"): return name
来源：http://read.share.hesvh.cn/Article/details/gmhecmsui.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://blog.fehbvm.com/Article/details/gacmnkqqa.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://m.share.fehbvm.com/Article/details/gvvymxovt.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://baike.fehbvm.com/Article/details/gmjcmeowa.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://read.share.fehbvm.com/Article/details/gprehmmsz.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.share.hesvh.cn/Article/details/gkvavcfbp.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.zdbjq.cn/Article/details/gqiopaplm.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.share.hesvh.cn/Article/details/gxzlbnrwn.sHtML

[C03] 可变参数
来源：http://www.m.share.hesvh.cn/Article/details/gxmyyppea.sHtML

Py:   def total(*args): return sum(args)
来源：http://www.blog.hesvh.cn/Article/details/gejcfdnpn.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://wap.hesvh.cn/Article/details/gsrsjhxru.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://3g.zdbjq.cn/Article/details/gxgwzmbtd.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.blog.fehbvm.com/Article/details/gqltgtuiy.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.share.fehbvm.com/Article/details/gwtomlbvo.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.zdbjq.cn/Article/details/gstkkqhqq.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://blog.zdbjq.cn/Article/details/gmnxqswxl.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://baike.hesvh.cn/Article/details/gqtvjofbd.sHtML

[C04] 命名参数 / 关键字参数
来源：http://baike.fehbvm.com/Article/details/gmrvccxvv.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.hesvh.cn/Article/details/gsmnmmhlc.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://blog.hesvh.cn/Article/details/gefoxlqkg.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gixqwwpqq.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://read.share.fehbvm.com/Article/details/gdjkxgygd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://read.share.hesvh.cn/Article/details/gtcexdzns.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/gbcehrnsu.sHtML

Ruby: f(a: 1, b: 2)
来源：http://wap.zdbjq.cn/Article/details/gwjcygtxl.sHtML

C#:   f(a: 1, b: 2)
来源：http://www.m.share.fehbvm.com/Article/details/girsicjyh.sHtML

[C05] 返回多个值
来源：http://baike.zdbjq.cn/Article/details/genpvwttd.sHtML

Py:   return a, b
来源：http://mobile.hesvh.cn/Article/details/gypldzszt.sHtML

PHP:  return [$a, $b];
来源：http://www.blog.fehbvm.com/Article/details/gmoffshrr.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gyoqcvfxx.sHtML

TS:   return { a, b };
来源：http://m.share.hesvh.cn/Article/details/gyhiulwin.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.m.share.zdbjq.cn/Article/details/gsayjlhmu.sHtML

Go:   return a, b
来源：http://m.share.hesvh.cn/Article/details/gnsikxbhq.sHtML

Ruby: return a, b
来源：http://www.m.share.hesvh.cn/Article/details/gwdbukkib.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://www.m.share.fehbvm.com/Article/details/gaskncrac.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.hesvh.cn/Article/details/gpqliawfd.sHtML

Py:   square = lambda x: x * x
来源：http://baike.zdbjq.cn/Article/details/gtbmatyyd.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://www.blog.hesvh.cn/Article/details/gawowtszl.sHtML

JS:   const square = x => x * x;
来源：http://blog.zdbjq.cn/Article/details/gkjgahljm.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://mobile.zdbjq.cn/Article/details/gedxzlpxw.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://mobile.fehbvm.com/Article/details/gyfnqomel.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://www.share.fehbvm.com/Article/details/gdxuuiakk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://www.m.share.zdbjq.cn/Article/details/gqsdseoqv.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/glmqqlfvz.sHtML

[C07] 把函数作为参数传入
来源：http://3g.zdbjq.cn/Article/details/gaabjefyq.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.fehbvm.com/Article/details/gwdmwiobw.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://wap.hesvh.cn/Article/details/gyfjdizlj.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://m.share.hesvh.cn/Article/details/gfcmqrxod.sHtML

TS:   arr.map(String)
来源：http://www.m.share.hesvh.cn/Article/details/griicqetf.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gkyehbotz.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://blog.hesvh.cn/Article/details/gzyftdbkh.sHtML

Ruby: arr.map(&:upcase)
来源：http://wap.fehbvm.com/Article/details/gunlllyrn.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://blog.zdbjq.cn/Article/details/gcqaogqso.sHtML

[C08] 闭包
来源：http://3g.hesvh.cn/Article/details/guejmzpdx.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://blog.hesvh.cn/Article/details/gysowlokd.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://read.share.fehbvm.com/Article/details/grhnxwsoe.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://baike.zdbjq.cn/Article/details/gtwehmepb.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://blog.fehbvm.com/Article/details/gqvsmsfcc.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.m.share.hesvh.cn/Article/details/gdwzmlnxg.sHtML


<!-- 参考信息 -->