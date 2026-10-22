代发 wailian999

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2mhxinjnv.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2iwdllqgf.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2qldyxcux.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2korbofbr.html

[A18] 字符与 ASCII 码互转
来源：http://www.ydjk.org.cn/Article/details/gt2ecqkqjlh.html

Py:   ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2ihncxcro.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2vtlcdqff.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2qihcelwy.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2mzxhkwqu.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2aavledie.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2uvxmdwtw.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2fqoopevh.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2psdfthjs.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2txgagovo.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt2twrgbsmr.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt2prfpqvtv.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2qqxizkcd.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2gutlwpra.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2ndyijvsn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2dcyqzerm.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2bqqdebfb.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt2kkrskyec.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2ygdwlbtw.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2affeeuun.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2jfypucgi.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt2yjdsysjt.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt2grjjtdnp.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2qqiwyfhl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt2ebytngod.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2wcrxrkxf.html

C#:   Console.ReadLine();
来源：http://www.ydjk.org.cn/Article/details/gt2cvrdhwum.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt2qofiyjbp.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt2jijimxob.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2qxxqehne.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qzxdhgjm.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pddxkirs.html

Java: String.format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2jxnhsfnf.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2vkkyvjbc.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2odjmujbz.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2owfdrufz.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fluydweo.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt2qmtdzmpn.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt2jfzojayw.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2rdfjfzzx.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt2iqzuiihk.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt2kwdpycjw.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2cdxbtttb.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2udujoltu.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt2ecfttjzm.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rsecwzah.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2gmrruxzy.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt2cgwtlgoc.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2fboehswk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2refjftvr.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2acajnmry.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxzdkofa.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fchwglny.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2dsfykpnp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt2xkjzouly.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2favfuiaf.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2foxebjfy.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2tspblnxa.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2uldhthel.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2zssatwlo.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bruvukdq.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2lvylmkdq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2xpftrvia.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qikaomlt.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt2pbcwjqaq.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt2hebqugsu.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2mnzckkze.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2hlzovcue.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2dloanudz.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ydebokkx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2sukcudej.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2vcntfdpt.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2rzyudqjb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2hiheblch.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2womsbqbh.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2qyepgeom.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2pbpyrusr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2aehsiunf.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2pafwbnmp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2wlozzhie.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2icsxgssl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jdnetrze.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2bdxosyui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2buewmeyj.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2rysypumv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2vdowdjpt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2duwtofsf.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2gmydxcfd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2dhqjaewj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hprlzpnh.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wdmhteuw.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2mnfrdnjl.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2lqryfkyu.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2kdjcufpj.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2tojdtdmo.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzvuhiiv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2vdhqsojz.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ngfsdtbs.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2cfqxrpsj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2itoutfpg.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2eeqkwrex.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ttlgefdv.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2vazssirk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2yliovrgu.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jfhesdpr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2twfchjys.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2mhnqmimk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jiumrlxx.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hweuyisx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dkuntomm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2ipwvtqlx.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ywgozyiw.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hsltlvhg.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpbuypwa.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2avfpnpwq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2cstcjeim.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2jztyqnri.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2xunxtbzf.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2khunruhg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2akcvkdik.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wkxwfoqx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2qqcorqwa.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2pxibogvo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2augpwszr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2txdhdzdh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2rbidqctq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zjyoftht.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2twsctran.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2okbgpqky.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2ltqcarmx.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2jdehjddj.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2cnehrefa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ybtysylz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2sfdhotrn.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rbekubko.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2lqwtvowf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2cysbtgny.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2svzsaooe.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2abzpnnzc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2zpnimvse.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvhdalye.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2catttlwu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cuzuihfa.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hemungxs.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2mgvmgnwx.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2xjwqewot.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ycirmjus.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2eddnvwji.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2wpuiayhv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pdbdcqiq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pnfkkvey.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yfcplopd.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2lawetrzr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qokpcwbx.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2cwnlxjwo.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wqfnvbgr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2gkidjytm.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2orhfowkt.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bpvowrbk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvmallpt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2chvhdstu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhwbqilq.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2hcapksgk.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2jbdaeapq.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kyguvpdw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2awtfgndf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2jdvwbhrp.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zozfyywl.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2wnypmjkf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2cfcixspt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2zzwpcdgx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2uwnbytsn.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2mjatqfyu.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktnzqoqd.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vmzozvmv.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wxuvbipm.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qljcweft.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yfpgthac.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nhfepzsm.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2xziwfnnf.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2ttgrmblf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mdcapzri.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2giodcscr.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2konntmzi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2vvjojnhn.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2belskukh.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lbhokcuk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2ntrzzqye.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ryhfiaur.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2lfhthqai.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2fycbtffh.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2vzfoyfwk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2ytdbbrvk.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2vgojycmv.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2ktojzsai.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kicupdru.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ntcxnzuy.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2ywujuegv.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2edwseonc.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2ueeilrjc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2eoqpvqkb.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2aiaqgliw.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2epzyqrjd.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2wtdhvgul.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cqtsrsku.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qcnazxfz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2zgdctlyd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2atybiscu.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bvzxqfuf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2limwnskm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2daalynvq.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2usptqtqj.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2amdoghxa.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2eezrfyvh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2buvedfoh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wlqtgbvc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2getrnpcw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cdzlfhgn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ejmuljxx.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2yndqibhe.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wdoviegf.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2izyeojbx.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dphginau.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2edhyyuvm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vudnqars.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fglwtmcs.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2rzvibtbn.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2cywjedjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpvhtjkd.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2czlctpdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jsbrpcro.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gidwlcmc.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wmarpuqk.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ocgwaigr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2caaepzjz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zxerlpvy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2skchqlgl.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wfvicdjf.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2qcanfisa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2uipazcdb.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2cwkqqvvc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2rjtedkpb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttfvzhak.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ypdgyclj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vpmqtrol.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2wqlxhzxl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2fagqbgfg.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2acflqrdn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2rxugvoyy.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2ttwwafjh.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2djwheckc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2tebeamml.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ymqamcww.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qglhmiic.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2icpaenpu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2amzulsfc.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qjyadltx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2meemaicn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ddlabuev.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2jiclhyeg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2sldhmoef.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2puzcbmia.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fkmdgtey.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qacsvzbd.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2qsihcina.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ukytwyuu.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2azftdbhf.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2xfdezlhf.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2tvnlvcrt.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vgqgjiuu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2zcapuedh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2byobekyz.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2eqjjrbxb.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2vhtytdry.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2usaohuxv.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ezhduylt.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2sjlhbdzh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2rvxqajjo.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2imsaeuay.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2kiwvahqn.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qcdrbfzn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fyuviaxg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2bhvimoby.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2tfozsxht.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qldrsegm.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2avnypkto.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2inqtzzjv.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2lptwdwpy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2jgbbavca.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2pvgvuebx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nwssamqj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2zybmffjv.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2snfutecu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hfdvbxzv.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2yghvytua.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2hmmcaxlg.html


<!-- 参考信息 -->