代发 wailian999

Py:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2xkcvgmvj.html

PHP:  $a & $b; $a | $b; $a ^ $b; $a << 2; $a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2ozfaqyyn.html

JS:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2piujpmdg.html

TS:   a & b; a | b; a ^ b; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ldivtjfp.html

Java: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2rtlhxjwd.html

Go:   a & b; a | b; a ^ b; ^a; a << 2; a >> 1
来源：http://www.ydjk.org.cn/Article/details/gt2olxzeqcg.html

Ruby: a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2ejrhaywm.html

C#:   a & b; a | b; a ^ b; ~a; a << 2; a >> 1
来源：http://www.52xcode.cn/Article/details/gt2dhgeoteb.html

[A18] 字符与 ASCII 码互转
来源：http://www.52xcode.cn/Article/details/gt2gjybniqn.html

Py:   ord("A"); chr(65)
来源：http://www.ydjk.org.cn/Article/details/gt2fzmncdya.html

PHP:  ord("A"); chr(65)
来源：http://www.52xcode.cn/Article/details/gt2yojjfxsv.html

JS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.52xcode.cn/Article/details/gt2wywkclgv.html

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt2kljfrqre.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt2gkgutojh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.ydjk.org.cn/Article/details/gt2iufqevbd.html

Ruby: "A".ord; 65.chr
来源：http://www.52xcode.cn/Article/details/gt2ogqcjrtd.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt2cowbykcj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt2mwpokiwp.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2ritvpykt.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt2faazqmml.html

JS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt2ebeimehl.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt2canvoshw.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt2yundtphn.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2tnkggjic.html

Ruby: a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt2sndxbxye.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt2zxvwqrpi.html

[A20] 读取标准输入
来源：http://www.ydjk.org.cn/Article/details/gt2vtneanjn.html

Py:   name = input("请输入：")
来源：http://www.52xcode.cn/Article/details/gt2ypeeanvm.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.ydjk.org.cn/Article/details/gt2whwkkwqx.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt2jjynmxib.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kmwqrgsf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt2zjwnmqnr.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt2uwvuhjll.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt2ywxhwyog.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt2elkyhvgn.html

[A21] 保留指定小数位输出
来源：http://www.ydjk.org.cn/Article/details/gt2ftkebste.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt2usllwjqj.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2iwhebrsb.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2vzjqgpyz.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wmijbxxc.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2zqxgbihe.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt2kqzwmgmn.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt2favexjqo.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt2hkfzmenp.html

[A22] 获取字符串长度
来源：http://www.52xcode.cn/Article/details/gt2khfiomoh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yaupsbcg.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt2flqxtclc.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt2mjeimsyu.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ouzocazj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vvmcvmlj.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt2eckcpmpk.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nynyjckh.html

C#:   s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zleukvsb.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2posbxaby.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt2kzspjzuz.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt2nexwepjj.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2kbqoiydd.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt2jqmuuzlw.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt2lvkbgkib.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt2cdkoanhs.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bggsaxgj.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt2ewanmqqd.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt2lncwetvc.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt2btrodogp.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt2gemgfomm.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt2ijnkswfp.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2kuqcnaee.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt2rpquidvu.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt2banoshbp.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt2jguuuzid.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt2yqlfgxue.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jkonelys.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2zknueebc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqpktnjd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2tphntysw.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2btgckltg.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2bfkuyebq.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2jclnlmcw.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2txlpscyk.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2lnzkicoc.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt2cgvntcbj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2qrcqphbd.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt2fnfwcftj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2njundflg.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt2lesgkxcd.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2zowjrygz.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2vudgnbyn.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2oddepzav.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mxboorni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2embydgti.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2yluiyqyi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mtvgqvzt.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2vwatnnta.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2nyoxdmrt.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxjhstrr.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hwgegkjp.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2emocuqce.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ixhepido.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2wvipmtzs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qhxfyetm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2fdssfkoo.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2vxpofohn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2bddiojrg.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2oaooicox.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ibfrygik.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2frbiadvu.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2snlpbldu.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2vtjwkmma.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2bvwumgfr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2pgfzvxuj.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2xybosjux.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2ytctjvqx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2urtekrkq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xcwaqemk.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2oarehrjz.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2sjdbjlvr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2puzviwac.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2xfrsljyr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2hpixrgzw.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gjwnzuhs.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2wxpzqfqu.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewxatswo.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2uztppuxq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2trwyihub.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2coknpauo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2ikarwoce.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2mrwfoqoi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgphdhia.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2jyzznsjz.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wanlbbwl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2wgrdinih.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2pxqevbin.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpahvznf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2hbjsmwzw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2nappflwt.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2xezrjgyd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2qetoefjw.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2zqrttnsb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2qanbqvmk.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2rfvtutod.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2iqxzeobb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2jihvefqo.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2sdfrsqux.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2zswogyeh.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2rucxhbjp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2owmvlxnw.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2xgmdxsfg.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2qjufdpsq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2hctxftjw.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bmurdyrm.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncszxvwt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2crxameqr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2tndxunck.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2afsmhdah.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2lgqblang.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2shoczppf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2jjcacxwr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2icspppdq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2pkbfrcds.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2hfsiijoa.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wuzslpac.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2smnmoitl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2jgqnftgg.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2eugdfdrp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2vlxnmgbf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2upmezlmf.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xqtvgiqo.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xfoyqzvu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bgvrdndi.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jcufeqny.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2jedrxpgm.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2lampsipt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2djjqivtf.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2mhafvxlg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2mirpzyrg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhdjhaav.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2idcxrivb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yzotydlf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ptmxsgmg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2tnbaukpy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2jhyfwgrl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2uaxtdbeo.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2zzpefral.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2rqdrarxr.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2bnizwkvu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2unkrbhkl.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2giiinmjs.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2vlkcvion.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2bydzrrta.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ddbhlsff.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uhuwpvln.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wdgbgobd.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hzopuplx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2oekzlsye.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wcjpocxc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tmxvjckw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fmabkrwx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2qcjnjkkx.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2cmqipsuq.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2fgzkibpb.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2ptfsghyn.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2ewkgfrcp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2eepcmlyf.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2rjwakvhy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2seszovlw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2vdfevqzb.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2lbcjteew.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2etjgxwly.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2gbbuparg.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2yvhqspss.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2hpkrjyvt.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2yeszetwo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zzngkmnu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qclpgtsw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdrpabom.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ypkgelvm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqugyzda.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uzrsardm.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2vkkcfqpf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2amuluccm.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2zzpyyida.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cxhrgeej.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2peztirql.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2egmxagml.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ezookflb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2sapfwljs.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2cwdjqzoq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2exvsuqae.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2hxkxltly.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2cnggwtcw.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zuzkiims.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wrkjimkh.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2wybojowc.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2fdikboqa.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2hisbecaq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2wtitlzha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ugcrcuxp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2cazqtqbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzwmknkr.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2dguklxxc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2caliqcam.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsmewdxp.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2pbywkyjo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ohmxsckm.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jykotfxy.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kqqzftft.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2mauxylua.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lmtzvqpz.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2wcfivxru.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2goarbluy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2zpuwivot.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tbglxgyl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcwceelk.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2lchedlhl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2aisqlhtb.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ixmbpadz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2cpcyvwta.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2dwbbiton.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2nftflvve.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2yxvshhor.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2saupxdaz.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2qfrpjsdq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2rgyuuckm.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2evgpunru.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2ikolquwy.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jffzxfhe.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2jrbrxife.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2hqthdkkd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2bszwkckr.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xrgmtxcd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qqbnrjps.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2rhmkkiph.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2drddmkqi.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fkiyjdin.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2pmbglrfz.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2ciqgftbs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ihwsjaai.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2gizikbyn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2xzepkdcx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ydlrpuew.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2lsnbjwyy.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2wxjizykx.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2xtaqqrsl.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2dfvrjpvx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2ciwummft.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vylrydzi.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2pupuwwll.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2jwoplpti.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2qkelbvxp.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2sxaiogoq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2imwxuhxn.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wihobbkr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ychmzjez.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2dznissug.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2ionatlku.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oraafnap.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2jwbcpbno.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2yaqgqvuh.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2ilsighab.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2fvcrclsn.html


<!-- 参考信息 -->