代发 wailian999

PHP:  if (empty($x)) {}   # 松散比较，注意 "0"
来源：http://www.blog.zdbjq.cn/Article/details/gsbnozpbm.sHtML

JS:   if (!x) {}         # 0 "" null undefined NaN false 为假
来源：http://wap.hesvh.cn/Article/details/gkestvoza.sHtML

TS:   if (!x) {}
来源：http://www.blog.hesvh.cn/Article/details/gnsyqfrgm.sHtML

Java: if (!Boolean.TRUE.equals(flag)) {}
来源：http://baike.zdbjq.cn/Article/details/gsnfyhqxq.sHtML

Go:   if x == "" || x == 0 {}   # 无隐式布尔转换
来源：http://www.m.share.zdbjq.cn/Article/details/gjwyhhosr.sHtML

Ruby: unless x            # nil 与 false 为假
来源：http://www.blog.hesvh.cn/Article/details/gnecxjefm.sHtML

C#:   if (string.IsNullOrEmpty(x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gdgkjkovd.sHtML

[A17] 位运算
来源：http://m.share.zdbjq.cn/Article/details/gneyxxjig.sHtML

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gpdmlshcq.sHtML

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.share.fehbvm.com/Article/details/gwvfumdwy.sHtML

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://wap.zdbjq.cn/Article/details/gbzcosgze.sHtML

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.m.share.hesvh.cn/Article/details/gdeyrbnlh.sHtML

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://mobile.fehbvm.com/Article/details/gewpcdouh.sHtML

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.blog.zdbjq.cn/Article/details/gqvncxqtg.sHtML

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://baike.fehbvm.com/Article/details/geoodevwp.sHtML

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://read.share.zdbjq.cn/Article/details/gfzgzgtay.sHtML

[A18] 字符与 ASCII 码互转
来源：http://3g.zdbjq.cn/Article/details/golgbsfzj.sHtML

Py:   ord("A"); chr(65)
来源：http://www.share.zdbjq.cn/Article/details/ghnprodnx.sHtML

PHP:  ord("A"); chr(65)
来源：http://www.blog.fehbvm.com/Article/details/gqdrrfytv.sHtML

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://wap.fehbvm.com/Article/details/gbmbtdgqo.sHtML

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.share.zdbjq.cn/Article/details/gjorjilwi.sHtML

Java: (int) 'A'; (char) 65
来源：http://www.m.share.hesvh.cn/Article/details/gfbptcabz.sHtML

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://mobile.hesvh.cn/Article/details/gvwwydxfo.sHtML

Ruby: "A".ord; 65.chr
来源：http://read.share.hesvh.cn/Article/details/gdjodlyey.sHtML

C#:   (int)'A'; (char)65
来源：http://www.share.fehbvm.com/Article/details/gddslaleb.sHtML

[A19] 交换两个变量
来源：http://mobile.fehbvm.com/Article/details/guibalflg.sHtML

Py:   a, b = b, a
来源：http://www.blog.zdbjq.cn/Article/details/grpfonxny.sHtML

PHP:  [$a, $b] = [$b, $a];
来源：http://baike.fehbvm.com/Article/details/glbsjfznq.sHtML

JS:   [a, b] = [b, a];
来源：http://read.share.fehbvm.com/Article/details/gtckdxute.sHtML

TS:   [a, b] = [b, a];
来源：http://www.m.share.fehbvm.com/Article/details/goufktmje.sHtML

Java: int t = a; a = b; b = t;
来源：http://www.blog.fehbvm.com/Article/details/galiqkgof.sHtML

Go:   a, b = b, a
来源：http://www.m.share.zdbjq.cn/Article/details/gniptajig.sHtML

Ruby: a, b = b, a
来源：http://blog.fehbvm.com/Article/details/gioqpbulm.sHtML

C#:   (a, b) = (b, a);
来源：http://www.share.zdbjq.cn/Article/details/gvxsxkwev.sHtML

[A20] 读取标准输入
来源：http://wap.zdbjq.cn/Article/details/gxukhxkqj.sHtML

Py:   name = input("请输入：")
来源：http://www.share.zdbjq.cn/Article/details/gpocaqtuy.sHtML

PHP:  $name = trim(fgets(STDIN));
来源：http://m.share.hesvh.cn/Article/details/gbjnwlhhn.sHtML

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.blog.hesvh.cn/Article/details/gekwerdhb.sHtML

TS:   // Node.js：readline 模块
来源：http://blog.zdbjq.cn/Article/details/gemqrcvrj.sHtML

Java: new Scanner(System.in).nextLine()
来源：http://www.m.share.hesvh.cn/Article/details/guvprshoe.sHtML

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://m.share.zdbjq.cn/Article/details/gkkovahql.sHtML

Ruby: gets.chomp
来源：http://mobile.hesvh.cn/Article/details/gqqexgrhl.sHtML

C#:   Console.ReadLine();
来源：http://wap.hesvh.cn/Article/details/gcajppxos.sHtML

[A21] 保留指定小数位输出
来源：http://baike.hesvh.cn/Article/details/gmugiaghm.sHtML

Py:   f"{3.14159:.2f}"
来源：http://mobile.hesvh.cn/Article/details/ghspngfnm.sHtML

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://m.share.fehbvm.com/Article/details/gxrwxoigv.sHtML

JS:   (3.14159).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gagrslnyj.sHtML

TS:   (3.14159).toFixed(2)
来源：http://www.blog.hesvh.cn/Article/details/gxrwisyfm.sHtML

Java: String.format("%.2f", 3.14159)
来源：http://baike.hesvh.cn/Article/details/gdyfhlsjs.sHtML

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.blog.zdbjq.cn/Article/details/gvvxyxtxn.sHtML

Ruby: format("%.2f", 3.14159)
来源：http://read.share.fehbvm.com/Article/details/grqaxxsaa.sHtML

C#:   3.14159.ToString("F2")
来源：http://baike.fehbvm.com/Article/details/guctxwzop.sHtML

[A22] 获取字符串长度
来源：http://blog.zdbjq.cn/Article/details/ggcvklfmi.sHtML

Py:   len(s)
来源：http://blog.zdbjq.cn/Article/details/guuijlmfv.sHtML

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.m.share.fehbvm.com/Article/details/gvibzebrr.sHtML

JS:   s.length                          # 按 UTF-16 单元计
来源：http://mobile.hesvh.cn/Article/details/gkqdfqtov.sHtML

TS:   s.length
来源：http://baike.zdbjq.cn/Article/details/glpvggnhp.sHtML

Java: s.length()
来源：http://www.blog.fehbvm.com/Article/details/gowswonoh.sHtML

Go:   len(s); utf8.RuneCountInString(s)
来源：http://blog.zdbjq.cn/Article/details/ggelgpxrf.sHtML

Ruby: s.length
来源：http://mobile.zdbjq.cn/Article/details/gqmcllcum.sHtML

C#:   s.Length
来源：http://read.share.zdbjq.cn/Article/details/gfbypdgsi.sHtML

[A23] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gksckwznx.sHtML

Py:   s.upper(); s.lower(); s.title()
来源：http://www.share.zdbjq.cn/Article/details/gzrafypqo.sHtML

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://m.share.zdbjq.cn/Article/details/gtbkjjoop.sHtML

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://read.share.zdbjq.cn/Article/details/gfguglvya.sHtML

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://m.share.hesvh.cn/Article/details/grjgvayzd.sHtML

Java: s.toUpperCase(); s.toLowerCase()
来源：http://read.share.hesvh.cn/Article/details/gbugxcizz.sHtML

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://baike.hesvh.cn/Article/details/gjakhwqcv.sHtML

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gnafkpudr.sHtML

C#:   s.ToUpper(); s.ToLower()
来源：http://wap.fehbvm.com/Article/details/gwfijnalr.sHtML

[A24] 去除首尾空白
来源：http://m.share.zdbjq.cn/Article/details/gagjyctqj.sHtML

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://wap.hesvh.cn/Article/details/glnwsnstb.sHtML

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.m.share.hesvh.cn/Article/details/gumaatalc.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.blog.zdbjq.cn/Article/details/gjopulsmk.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.m.share.hesvh.cn/Article/details/gehjlsqir.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.hesvh.cn/Article/details/gatxihbmy.sHtML

Go:   strings.TrimSpace(s)
来源：http://www.m.share.hesvh.cn/Article/details/gmwhpkmow.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://m.share.zdbjq.cn/Article/details/gbwjvzabt.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://mobile.fehbvm.com/Article/details/gbkkrlmdb.sHtML

[A25] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gkpkegeol.sHtML

Py:   s1 == s2; s1 != s2
来源：http://www.m.share.fehbvm.com/Article/details/gidnxabri.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://mobile.hesvh.cn/Article/details/gahpanyhq.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.blog.fehbvm.com/Article/details/gjmbeqind.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.m.share.hesvh.cn/Article/details/gabrwlaoo.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://blog.hesvh.cn/Article/details/gynyirzib.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmcdwppko.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://m.share.hesvh.cn/Article/details/gdaroxxqk.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gwthxvkch.sHtML

[A26] 类型转换总览
来源：http://wap.fehbvm.com/Article/details/gbcknfkiy.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.share.zdbjq.cn/Article/details/gjgygsjwt.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://blog.fehbvm.com/Article/details/gnszvcxbr.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://wap.zdbjq.cn/Article/details/gryowknas.sHtML

TS:   Number() String() Boolean() x as number
来源：http://m.share.hesvh.cn/Article/details/gsxgdvbsv.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://blog.fehbvm.com/Article/details/gdtwsajne.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/gqgxicbgi.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://blog.fehbvm.com/Article/details/gopqtrbee.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.share.fehbvm.com/Article/details/gzwrndkws.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/guyafqeop.sHtML

B. 流程控制
来源：http://m.share.hesvh.cn/Article/details/gnbhkryfj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/getsqexgn.sHtML

[B01] 条件判断 if / else
来源：http://www.m.share.fehbvm.com/Article/details/gcjlchxel.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://www.blog.fehbvm.com/Article/details/gktrvmcmg.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://baike.zdbjq.cn/Article/details/gbflnpiwt.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.m.share.fehbvm.com/Article/details/gqjmngooj.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://baike.fehbvm.com/Article/details/gurlqjzfk.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://wap.zdbjq.cn/Article/details/geuoppdhi.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://mobile.zdbjq.cn/Article/details/gbnlufkgq.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://m.share.zdbjq.cn/Article/details/gdeoejpar.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gbsmvcjwq.sHtML

[B02] 多分支 else if / elif
来源：http://blog.zdbjq.cn/Article/details/gdczdpwcx.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://blog.fehbvm.com/Article/details/gkfztdtud.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://read.share.fehbvm.com/Article/details/grsysiakr.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gyrxbclut.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://3g.fehbvm.com/Article/details/gsroqqohr.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.m.share.fehbvm.com/Article/details/gmoeeeyqb.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://mobile.zdbjq.cn/Article/details/gkzybqufw.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://wap.fehbvm.com/Article/details/gowwzfsjn.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.zdbjq.cn/Article/details/gsttldqbi.sHtML

[B03] switch / match / case
来源：http://www.blog.zdbjq.cn/Article/details/gmclwmfnr.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://wap.zdbjq.cn/Article/details/gftjdlfyt.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gowecivgv.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.fehbvm.com/Article/details/gcjmvhlbb.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmvnduyrv.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://blog.fehbvm.com/Article/details/gxlyjsdwl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://read.share.hesvh.cn/Article/details/gtzgoqdfl.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://3g.fehbvm.com/Article/details/gwnkoxtds.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.share.hesvh.cn/Article/details/gdempybcw.sHtML

[B04] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gzjnayfsy.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/gnvptlhxe.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://mobile.fehbvm.com/Article/details/gspjhhbiu.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://m.share.zdbjq.cn/Article/details/gsvyruxms.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.share.hesvh.cn/Article/details/gvuiaxvjx.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://baike.zdbjq.cn/Article/details/gkhavehob.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.blog.hesvh.cn/Article/details/grwxbjpkz.sHtML

Ruby: 10.times { |i| puts i }
来源：http://read.share.hesvh.cn/Article/details/gcnhkhfse.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.blog.fehbvm.com/Article/details/gcokdvufc.sHtML

[B05] 遍历数组 / 列表
来源：http://mobile.fehbvm.com/Article/details/glkjfgakl.sHtML

Py:   for item in arr: print(item)
来源：http://wap.zdbjq.cn/Article/details/gbsyfgpvn.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://read.share.zdbjq.cn/Article/details/gjwbpggni.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://mobile.zdbjq.cn/Article/details/gtyzdidax.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://www.m.share.fehbvm.com/Article/details/gygwvpkkz.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://blog.zdbjq.cn/Article/details/gzaldegqp.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://blog.fehbvm.com/Article/details/gwaypeksn.sHtML

Ruby: arr.each { |item| puts item }
来源：http://www.blog.fehbvm.com/Article/details/ggkaonnrc.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.blog.fehbvm.com/Article/details/glhspnvnr.sHtML

[B06] 遍历字典 / 对象
来源：http://www.share.hesvh.cn/Article/details/gclnexcas.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://wap.zdbjq.cn/Article/details/gohrwnkit.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.m.share.hesvh.cn/Article/details/gjpvrauwn.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.m.share.fehbvm.com/Article/details/gqrbpzuwf.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://blog.zdbjq.cn/Article/details/gyvygcmia.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.share.fehbvm.com/Article/details/gtdhzvdcz.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://wap.fehbvm.com/Article/details/gypoexras.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.zdbjq.cn/Article/details/gagujtnqo.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://baike.zdbjq.cn/Article/details/gxjfqkywr.sHtML

[B07] while 循环
来源：http://www.blog.hesvh.cn/Article/details/gdadvfcnd.sHtML

Py:   while i < 10: i += 1
来源：http://blog.fehbvm.com/Article/details/glejsqumx.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://baike.hesvh.cn/Article/details/gmwpureug.sHtML

JS:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/gdhlgnodo.sHtML

TS:   while (i < 10) { i++; }
来源：http://wap.hesvh.cn/Article/details/gxunnomqs.sHtML

Java: while (i < 10) { i++; }
来源：http://blog.hesvh.cn/Article/details/gkwxtgxun.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://m.share.zdbjq.cn/Article/details/grwzhydjb.sHtML

Ruby: while i < 10; i += 1; end
来源：http://mobile.hesvh.cn/Article/details/gpshihivx.sHtML

C#:   while (i < 10) { i++; }
来源：http://m.share.fehbvm.com/Article/details/ghviiplxi.sHtML

[B08] do-while（至少执行一次）
来源：http://mobile.hesvh.cn/Article/details/gghdhepxh.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://read.share.zdbjq.cn/Article/details/gbgcfwniz.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://m.share.fehbvm.com/Article/details/goivyorlm.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.share.hesvh.cn/Article/details/gvzlpfrmq.sHtML

TS:   do { i++; } while (i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/gnrpufpgd.sHtML

Java: do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/grjxznhmi.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://wap.zdbjq.cn/Article/details/gtvdqnozf.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://read.share.fehbvm.com/Article/details/ggrihscvu.sHtML

C#:   do { i++; } while (i < 10);
来源：http://www.share.zdbjq.cn/Article/details/gygnbcsbm.sHtML

[B09] break 与 continue
来源：http://m.share.hesvh.cn/Article/details/gzizvdnwx.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://m.share.fehbvm.com/Article/details/ghnuzokwn.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://blog.zdbjq.cn/Article/details/gfeoqtngn.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.fehbvm.com/Article/details/gplsadeaq.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://baike.zdbjq.cn/Article/details/glfccrkyx.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://blog.hesvh.cn/Article/details/gjibkyznb.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://blog.fehbvm.com/Article/details/gjxayudei.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://wap.zdbjq.cn/Article/details/gaeqmuahp.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.zdbjq.cn/Article/details/gyclmuvaj.sHtML

[B10] 遍历同时拿索引
来源：http://m.share.zdbjq.cn/Article/details/gbwkrwatj.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://blog.zdbjq.cn/Article/details/gexcismbw.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://blog.fehbvm.com/Article/details/gyeatlwjx.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gnkyyfcxp.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.share.hesvh.cn/Article/details/gnsvoxofr.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://blog.fehbvm.com/Article/details/gmfjoldal.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.share.hesvh.cn/Article/details/gmvcmmxhd.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://baike.hesvh.cn/Article/details/glkjsegig.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://wap.fehbvm.com/Article/details/gqocmhfqm.sHtML

[B11] 生成数字序列 / 区间
来源：http://mobile.hesvh.cn/Article/details/grazjkruq.sHtML

Py:   list(range(0, 10, 2))
来源：http://m.share.hesvh.cn/Article/details/gabnumhbh.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gbaktzafm.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://mobile.hesvh.cn/Article/details/grdwkkrxu.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.share.zdbjq.cn/Article/details/geemihdyx.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://read.share.fehbvm.com/Article/details/gnkavonsi.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.share.zdbjq.cn/Article/details/gsnjmanvf.sHtML

Ruby: (0...10).step(2).to_a
来源：http://mobile.fehbvm.com/Article/details/gkscjzpgy.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://baike.fehbvm.com/Article/details/glqpbvgln.sHtML

[B12] 跳出多层循环
来源：http://www.share.hesvh.cn/Article/details/gnntpyqhl.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://wap.zdbjq.cn/Article/details/gauczzlqs.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://read.share.fehbvm.com/Article/details/gqwpxoklo.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://mobile.zdbjq.cn/Article/details/gwjagdoyc.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://baike.hesvh.cn/Article/details/guvimyzxu.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://blog.hesvh.cn/Article/details/grjqbhtot.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://read.share.fehbvm.com/Article/details/gqrbqnmol.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://blog.fehbvm.com/Article/details/ghgpfvuuk.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://wap.zdbjq.cn/Article/details/gkmbvnntv.sHtML

[B13] 判断是否为数字
来源：http://wap.zdbjq.cn/Article/details/grlymcvsf.sHtML

Py:   isinstance(x, (int, float))
来源：http://read.share.hesvh.cn/Article/details/grkkciakz.sHtML

PHP:  is_numeric($x)
来源：http://mobile.hesvh.cn/Article/details/gbnimnzgc.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://read.share.fehbvm.com/Article/details/gydmtnrqh.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://wap.hesvh.cn/Article/details/grilsvntf.sHtML

Java: x instanceof Number
来源：http://www.share.hesvh.cn/Article/details/gduxkmlwl.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://read.share.fehbvm.com/Article/details/gqdgktwfw.sHtML

Ruby: x.is_a?(Numeric)
来源：http://www.share.fehbvm.com/Article/details/gmheaomgo.sHtML

C#:   x is int or double or decimal
来源：http://baike.fehbvm.com/Article/details/gwnfjprha.sHtML

[B14] 判断值是否在集合内
来源：http://3g.zdbjq.cn/Article/details/gkkqvobii.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.hesvh.cn/Article/details/gbmrcvsqq.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://baike.zdbjq.cn/Article/details/gyeaqxeoo.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://baike.zdbjq.cn/Article/details/guymtzeic.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gbjizyumi.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://blog.hesvh.cn/Article/details/gkqadiwey.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://mobile.hesvh.cn/Article/details/gkljehptj.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://m.share.zdbjq.cn/Article/details/gmnbtphfy.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gmyrrxmvj.sHtML

[B15] 布尔运算与取反
来源：http://3g.fehbvm.com/Article/details/gcptkipqm.sHtML

Py:   a and b or not c
来源：http://m.share.fehbvm.com/Article/details/gqpkgylcz.sHtML

PHP:  $a && $b || !$c
来源：http://read.share.hesvh.cn/Article/details/gqeolfabi.sHtML

JS:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gvatfxvfb.sHtML

TS:   a && b || !c
来源：http://3g.hesvh.cn/Article/details/gwnmopxar.sHtML

Java: a && b || !c
来源：http://mobile.zdbjq.cn/Article/details/gekqnsdpz.sHtML

Go:   a && b || !c
来源：http://3g.zdbjq.cn/Article/details/gohriutci.sHtML

Ruby: a && b || !c
来源：http://3g.fehbvm.com/Article/details/gbwboobpr.sHtML

C#:   a && b || !c
来源：http://mobile.hesvh.cn/Article/details/gfdkswihr.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gfqyplcvs.sHtML

Py:   if not data: return
来源：http://3g.zdbjq.cn/Article/details/gevpjcsmk.sHtML

PHP:  if (!$data) { return; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkhwxeaza.sHtML

JS:   if (!data) return;
来源：http://www.blog.fehbvm.com/Article/details/gqezccpyy.sHtML

TS:   if (!data) return;
来源：http://read.share.hesvh.cn/Article/details/gaeoprevu.sHtML

Java: if (data == null) return;
来源：http://baike.zdbjq.cn/Article/details/gtflquibq.sHtML

Go:   if data == nil { return }
来源：http://www.share.fehbvm.com/Article/details/gpkfsqvtw.sHtML

Ruby: return if data.nil?
来源：http://www.m.share.fehbvm.com/Article/details/gbbprzcpt.sHtML

C#:   if (data == null) return;
来源：http://www.share.zdbjq.cn/Article/details/gdzhzuclv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggajlrpgz.sHtML

C. 函数与作用域
来源：http://m.share.zdbjq.cn/Article/details/gbvqjbfmg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gagfaajlm.sHtML

[C01] 定义函数
来源：http://baike.fehbvm.com/Article/details/gkerbtktn.sHtML

Py:   def add(a, b): return a + b
来源：http://wap.hesvh.cn/Article/details/gtmmafkhb.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://mobile.zdbjq.cn/Article/details/gxekdzmxz.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.blog.fehbvm.com/Article/details/gnjxgiyfm.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.blog.hesvh.cn/Article/details/gmuoxcztm.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://blog.zdbjq.cn/Article/details/gdmvkdpmz.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://m.share.fehbvm.com/Article/details/giouozopz.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.share.zdbjq.cn/Article/details/golcehnxd.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://3g.hesvh.cn/Article/details/guhhorqvl.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gshjgppdk.sHtML

Py:   def greet(name="World"): return name
来源：http://baike.zdbjq.cn/Article/details/gttjvuujn.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://wap.hesvh.cn/Article/details/gjvxsaigu.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/glwzszeiy.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://www.blog.zdbjq.cn/Article/details/gjdhcblqh.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://blog.hesvh.cn/Article/details/gyfvofitu.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.blog.hesvh.cn/Article/details/gjxznjpeb.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.m.share.hesvh.cn/Article/details/gzomotlmc.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://baike.zdbjq.cn/Article/details/gmimiayls.sHtML

[C03] 可变参数
来源：http://3g.fehbvm.com/Article/details/gihibyrij.sHtML

Py:   def total(*args): return sum(args)
来源：http://read.share.hesvh.cn/Article/details/gtnwyjush.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://baike.hesvh.cn/Article/details/gqvlebmvr.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://blog.hesvh.cn/Article/details/ggqlkhbro.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://wap.hesvh.cn/Article/details/grjnzxibl.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.m.share.hesvh.cn/Article/details/gkpgqomry.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.blog.hesvh.cn/Article/details/gadnuepjh.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/grrgnhceg.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://m.share.zdbjq.cn/Article/details/geyuejmkl.sHtML

[C04] 命名参数 / 关键字参数
来源：http://www.share.hesvh.cn/Article/details/gobcuewrr.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://wap.zdbjq.cn/Article/details/gbynwlexd.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.hesvh.cn/Article/details/gksxzqvbc.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwgelimig.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.blog.fehbvm.com/Article/details/gcdoeaeez.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://www.m.share.hesvh.cn/Article/details/giiptjqzr.sHtML

Go:   // 无：用配置结构体参数
来源：http://wap.fehbvm.com/Article/details/ghdtkuofj.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/ghxxkqxex.sHtML

C#:   f(a: 1, b: 2)
来源：http://blog.zdbjq.cn/Article/details/gjcdmsjwn.sHtML

[C05] 返回多个值
来源：http://www.share.hesvh.cn/Article/details/gzsebklfp.sHtML

Py:   return a, b
来源：http://blog.zdbjq.cn/Article/details/gmsofbtzj.sHtML

PHP:  return [$a, $b];
来源：http://mobile.hesvh.cn/Article/details/gypwgfxbi.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://blog.hesvh.cn/Article/details/gebdarkca.sHtML

TS:   return { a, b };
来源：http://3g.zdbjq.cn/Article/details/gwveiosln.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.zdbjq.cn/Article/details/gymzhymvf.sHtML

Go:   return a, b
来源：http://wap.fehbvm.com/Article/details/gqknymgpd.sHtML

Ruby: return a, b
来源：http://m.share.fehbvm.com/Article/details/ginwlznuz.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.hesvh.cn/Article/details/gstqhkczy.sHtML

[C06] 匿名函数 / lambda
来源：http://baike.fehbvm.com/Article/details/gqytzirci.sHtML

Py:   square = lambda x: x * x
来源：http://blog.zdbjq.cn/Article/details/glkccdbvi.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.fehbvm.com/Article/details/gwlngmkuk.sHtML

JS:   const square = x => x * x;
来源：http://mobile.hesvh.cn/Article/details/gcqsmntuf.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.m.share.hesvh.cn/Article/details/gihpettvm.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://3g.zdbjq.cn/Article/details/gbsnngllc.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://mobile.hesvh.cn/Article/details/gkuiowvhi.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.zdbjq.cn/Article/details/gauacgyhs.sHtML


<!-- 参考信息 -->