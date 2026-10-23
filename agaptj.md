代发 wailian999

TS:   "A".charCodeAt(0); String.fromCharCode(65)
来源：http://www.ydjk.org.cn/Article/details/gt3lngxbmzt.html

Java: (int) 'A'; (char) 65
来源：http://www.52xcode.cn/Article/details/gt3qwtviaqh.html

Go:   int('A'); rune(65)              // rune 是 int32
来源：http://www.52xcode.cn/Article/details/gt3jjtynbhv.html

Ruby: "A".ord; 65.chr
来源：http://www.ydjk.org.cn/Article/details/gt3pgaqyagf.html

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3mqqpflah.html

[A19] 交换两个变量
来源：http://www.52xcode.cn/Article/details/gt3ukrehugz.html

Py:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3tzsqcjct.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.ydjk.org.cn/Article/details/gt3mubxvcls.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3xlfizveg.html

TS:   [a, b] = [b, a];
来源：http://www.ydjk.org.cn/Article/details/gt3eyyphbdo.html

Java: int t = a; a = b; b = t;
来源：http://www.52xcode.cn/Article/details/gt3doawfhxa.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3qmjrfmfr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3hsfrukhw.html

C#:   (a, b) = (b, a);
来源：http://www.ydjk.org.cn/Article/details/gt3ppionxgf.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3exvqkgdo.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3wdhbmjda.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3pqjqglen.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3qljumodv.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3uuepmibf.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3bxhiciyy.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.52xcode.cn/Article/details/gt3wacfmugk.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3bmqqgoby.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3uvhlxzsb.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3aqgeobjk.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3afephnwq.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ptwzixmq.html

JS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cbawzinv.html

TS:   (3.14159).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zuhiwmor.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3abpqzhai.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3qquepzpu.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dueyzxjf.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3kkypwbcs.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3irxiujdn.html

Py:   len(s)
来源：http://www.52xcode.cn/Article/details/gt3fxrjjxko.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3wrgatwck.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.ydjk.org.cn/Article/details/gt3jpyocymo.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3npsbljrj.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3esjjndou.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3zgwdxjie.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3wjflrvcs.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3bcgbfyun.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3nkmodjpv.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3xymqbsqx.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.ydjk.org.cn/Article/details/gt3yueiuhgh.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3peenzqze.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3dinsmjfm.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3ymbgzyeg.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jumenyre.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cpdjbmdz.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3pysyynnu.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3tdbgdems.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3phnrtyla.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.52xcode.cn/Article/details/gt3yisknpqj.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3ffvpwslt.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3rfusmvvr.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3bziypbvf.html

Go:   strings.TrimSpace(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rnamioss.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3iuuwitsy.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3tkxcjrpv.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ktprbyai.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3tulllujz.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3phwggglx.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3jwrkoatl.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3wlwgeyug.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3ayoemslv.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3bqwqgnqr.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3qophjuab.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3sfdekwtk.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3wztfaejx.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3fvftxrsq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt3tsiyfxtl.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3gbficyzm.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3yrtnpyrw.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3jjebqnss.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3gektlkfl.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3yltcvcqj.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3pqyalwlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evmgqcvm.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3vlyiqgyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ilnddhhm.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3gzxbabjy.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ojcjwshg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3unjxizmz.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3copkvtrm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3owtnfjck.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3scyvynwg.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3gmjkfjdl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3ybzuxoai.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3otakaglf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3zokasgid.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3mwxepfjt.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3urycayek.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3thgaskkg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bdzfbtrt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xsplbtwv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3dyccvyki.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3bxvusqdy.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rexqykfx.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3wnkntigg.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3zxanrecn.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3snirbiyu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmvyfmxd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3bsjimfre.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3zagmphzu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3cfualbjb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3xavitfur.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3dqsnikzm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ysxcqavl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3mhldvhlq.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3qdpfqytc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hjtklitt.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdfclwxm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ipclppna.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3hkvfitxo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cglimvdk.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ixobssxq.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3gvxnvjqv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3ngegebrc.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3navsniov.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdocvvco.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3faaqygwb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cblwesnq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3wzccgwok.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3fgkzwqxj.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3pyweveus.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3waddxcht.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3hvjxtebt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zmqgjkry.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3rxtutpdd.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3myszkxoh.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnvaphrq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3hmsmmyta.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3vqkoxfhp.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3prkrixfg.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3aigmqnoq.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3vbjuqbae.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpokcwpf.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vwpeyyql.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3mflparnj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3iavtrlao.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3qppwhkkp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3fvxbflsp.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wcswsuzo.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3iqgdiwar.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3layzauga.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pszbxguj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mbjokzyc.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3mpclugnc.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3gmzgutqb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3jutwdlin.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3mmuacsxv.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3aysfoxyi.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3oacwmafe.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ocnqmkps.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oneljuig.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pztkudph.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhhviqny.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3yqsxjqbt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3aqusnpox.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3rmjjbaxy.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfuhkyty.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3aqbxzexz.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3airlbioi.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3altwjcmz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3cxddpyyz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3epgfjgzk.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3htanglkt.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3blerhwfr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3lizuasmc.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3cfxwlsfe.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3tmbtgsla.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3uisaphlm.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3jhzrqbbi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3azehaqbi.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vhirodek.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3lrrcvgiu.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3izglhqjf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wqsqumut.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3skiedoac.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3xetqjtck.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3nyrrccfd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3otbmdjai.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3shoxgugm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bqufygwo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3alxvqhvy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3xquivqbp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3zwqzlydb.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3fsoxaulf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3cjyzypfp.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3gyfkpdjs.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3uqedjasl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3nicktzvf.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3aqfmyuvi.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ivllqgmn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3andqurrv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ryxpbzgx.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ocukoptq.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3zdabjrhc.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3bvarufqs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3nkjwlitk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwvwviuo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkkmkasz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eyucnnmc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mxeeqxeq.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cwmdwrdf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hijgdzfp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3bjmvixyp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3pobvcnck.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3bxwnhusi.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mtymefdy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3asbxqxgq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cphkkbjq.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gpkdogyd.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3axwbrutn.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qcfwppyq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3yzpodndy.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3yrhpfkix.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3pbjgxdci.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jptnqhmg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ebrencvk.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3veeurhux.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3eqpuyetm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3alzulzlr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mghmqyrw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fahirepp.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mlpztwfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qztexhzu.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qrkujvab.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3sjdljvxf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3skltfrck.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlqwyoxc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynrdjmyn.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgnbeaez.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gtvlxuyl.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3vyalgqah.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwtkhnaj.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3pqexcuxt.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3qbzebafr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3otpwzxcz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhosbgov.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3quwagtgr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3necptlky.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3knshczuq.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3zogrjdve.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3hrgggkhe.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3mqdraaiw.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3tvfvpboz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3rimipwwq.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ibcybxwq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjguvzjx.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lpsqrenl.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3walcryxh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3qvimpjpx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3kxjkhmcn.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3djzaeora.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mzjnldia.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3qbizlptl.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjhjnyom.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3xdcqzreh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3ihsiwhga.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3gvpgygjr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3iivjekid.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3weweqmzw.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3rnvgtxwf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3gziuhfqh.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3fufdhsho.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3oczvqvur.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ulupgfyo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3awmdxdvi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3fmdllgkc.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3vgsegktn.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3kkeaadah.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3kxxgplez.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3emxswnvh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3fclqztke.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qggosxus.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eovhqtzc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oraftbfz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hthuzftu.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3hzzfudvi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zgaafhiq.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3widpndyx.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3pgvltbbe.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ydztzvcu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3hjzlneky.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3fmdywiil.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3okuyuwdk.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3wdgebxzs.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3oahapkdw.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3jqzuhoax.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3ciomkxjj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3vlnebbtn.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ruojnadw.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jrgsjmwc.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tmezjrzw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3lfxhogwm.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3tzbtvyxj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bkxxykqb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3pzisajtc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3myogllnw.html


<!-- 参考信息 -->