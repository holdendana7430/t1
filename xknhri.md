代发 wailian999

C#:   (int)'A'; (char)65
来源：http://www.52xcode.cn/Article/details/gt3rriepbhj.html

[A19] 交换两个变量
来源：http://www.ydjk.org.cn/Article/details/gt3penzeuif.html

Py:   a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3trehoaro.html

PHP:  [$a, $b] = [$b, $a];
来源：http://www.52xcode.cn/Article/details/gt3fztgbwvy.html

JS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3nomescgp.html

TS:   [a, b] = [b, a];
来源：http://www.52xcode.cn/Article/details/gt3kcplqnoy.html

Java: int t = a; a = b; b = t;
来源：http://www.ydjk.org.cn/Article/details/gt3tvueghdb.html

Go:   a, b = b, a
来源：http://www.52xcode.cn/Article/details/gt3nannfnfr.html

Ruby: a, b = b, a
来源：http://www.ydjk.org.cn/Article/details/gt3onicbvtv.html

C#:   (a, b) = (b, a);
来源：http://www.52xcode.cn/Article/details/gt3onqwfdve.html

[A20] 读取标准输入
来源：http://www.52xcode.cn/Article/details/gt3rxtihkna.html

Py:   name = input("请输入：")
来源：http://www.ydjk.org.cn/Article/details/gt3lxpgsejp.html

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3kljipiab.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.52xcode.cn/Article/details/gt3qwwtdpmj.html

TS:   // Node.js：readline 模块
来源：http://www.52xcode.cn/Article/details/gt3oyspxxzi.html

Java: new Scanner(System.in).nextLine()
来源：http://www.52xcode.cn/Article/details/gt3rrcitmks.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3omoqanvt.html

Ruby: gets.chomp
来源：http://www.52xcode.cn/Article/details/gt3hxbdbhdt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3diwuyvcd.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3kukaebru.html

Py:   f"{3.14159:.2f}"
来源：http://www.52xcode.cn/Article/details/gt3fwknjony.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3yyvpnmog.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tfqjnlfu.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rgjeaotq.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3edvubprk.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3rtmxsmol.html

Ruby: format("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3ebycxuws.html

C#:   3.14159.ToString("F2")
来源：http://www.ydjk.org.cn/Article/details/gt3sewhfsug.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lgjzgxgg.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ktqunzgr.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.ydjk.org.cn/Article/details/gt3umgeidbs.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3kjhkmyfi.html

TS:   s.length
来源：http://www.ydjk.org.cn/Article/details/gt3aruhhxje.html

Java: s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fuxlrdgc.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3cmolnxmd.html

Ruby: s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ezdzchvq.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3qdskilfd.html

[A23] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ezspqwwe.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3dszdqhzd.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3adzijakg.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3cqfvzcqk.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3xlbfkcee.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3kmqsruar.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3yqpiesxn.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3trsiecne.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3awrybqdt.html

[A24] 去除首尾空白
来源：http://www.52xcode.cn/Article/details/gt3crpeeqjr.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.ydjk.org.cn/Article/details/gt3vpgtiybl.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfszisql.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3letdcvhc.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3wtujaiki.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.ydjk.org.cn/Article/details/gt3gdxjzolx.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3cdymkinz.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.52xcode.cn/Article/details/gt3fbqzajpq.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.52xcode.cn/Article/details/gt3xaipbuck.html

[A25] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3iidgqqsh.html

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3jqmkzyev.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt3bmtgxioy.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3sivfhhgu.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbfggtye.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3ejlxlggb.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3raginofx.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt3rmdpmoch.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3iysittsa.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3wwiivjwg.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3rrvdmeqq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3gdebbpfj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3thofxmcj.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3lqfosjgs.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3dvnrrwmd.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3nwocjfvz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vzwezhia.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3oofumnja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obbrdqoj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3zmbyerbr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3laefymtq.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3ibiemwxr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3fbmyltez.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3cwbzebkx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mzfgexhu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3owrochbj.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3btennzju.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3ldantjeo.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3apqlayfk.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3adtmuqbf.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3bosyojvb.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3sryfganp.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivgmuczs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hufzhbix.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vcpiiufi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3nmrogqkj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3izjxqnof.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3cltbmygz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3iptlorhd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3ggcykacc.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3mrcyedko.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mkkszrfi.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuleuqku.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3swjwzcqp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3mchubmcy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3pnomzxpq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3znbesnru.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3xofwjogc.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3upobwngx.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3zdudxace.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3nsafmygc.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3yfyzaczk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3bfaqdszd.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3topyarky.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3dqmkibyk.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3ifemmjzf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3mehcmgbd.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gtusnjgh.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3qypkofuv.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3abwvksyx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yqhbutry.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzlyhmnh.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3ozhjxdxm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tfwcvmdf.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3jnxcmpkd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3flnlqwpv.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ghihhevo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3efnqxzwb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpjjxyli.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3taquhsns.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ulctvrvj.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3uklckevu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3jtmofrld.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3afqkplhm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3jlroeijn.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3atmjrzqx.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3yjjvbzvb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwgjrmgi.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpucmehl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qjlbmznt.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3xpordght.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3unqlsitg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3kuhgtuko.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3lusiumel.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3ulbecgbp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3fjrajvtx.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3siynotwf.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3accqweyk.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eifzyubm.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3qojrtohd.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3tgdydcch.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ipebsekq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jwfszwpz.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xdwbnwry.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3nzsrrozz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3czvrptkw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcgbzjjk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3axodnbxx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3edtbmfkx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3rjcptjzy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3sihpmvkn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aelnmexc.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3exirjizc.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vfohxexf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3apblyvri.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3zvriapjh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mfxybknf.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3xrsszvgg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3wboapkcg.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3tekwqksn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3efrhkazz.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3foddethw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3hqdlkfnq.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gpkzvjrz.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3rutisygn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hiuwmabo.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qggwppiy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3sdecmmzl.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ajxfqhoo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3egfpdyqv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3lzadtqem.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3skwcuaux.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3mlqqhzmy.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uiduyrep.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bvpsrfcf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3bibmtgrg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3hfkyltho.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3yztwbsmz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3itvyifkw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3vtbdgfsc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ahzqyzqp.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbkfgnsz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kdaefddm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlkkwebw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3eyceawdh.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3wqfvwwvj.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jkwmjvpj.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3alzbgoct.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3rwtflxdi.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3zemszwcb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3emgdxprk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3qkrvvsii.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wmnvkjao.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zxvpzsit.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3msltyrnw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3avehuyuf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xvzemeru.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3dpsukyea.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3nwpasjgd.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3iqrwzpel.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dwmujltp.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qbadgrmq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3motslwyr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3zzcntatw.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jgxtoetw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wxxswufs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ncyqrteb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3sirirado.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjhdfpbl.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3lbydwcdn.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tbihkfxe.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3sumivhba.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3hweashug.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3ksdqsbac.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3chrekims.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vtbwnfpy.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hpdadscv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knmgwpwp.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ertwlgco.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nfavozub.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnjppsox.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qrwibkxk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uqfuipir.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3smwvldjc.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3chspvzbr.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3oogqagnb.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3auuzjmtt.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3qegmvprb.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3wzluqngn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3svzrutas.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyouzhyj.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3leewarbw.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3fwdkfajz.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ebwpiaza.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3leweoaag.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3jzjynquf.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3yrhapbmt.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3dussoggo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3pupsrnpe.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhjguwkb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3junkxizc.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sisyudnx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3qdnihuix.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3yikxyfar.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3adwtetwy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3sfpkchex.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3gwpmtvnd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hflodxlz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3imjeqrks.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3imgyydoh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3uggpzsoo.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3dltpkzeq.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3iealexdd.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3obbslhax.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3tqyjvsgq.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ymhdxgnv.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3tbiqpenb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3syqvahkm.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zdthsqji.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3asomlvlj.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3podvsszk.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3pbrrllcc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3huhdzown.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hghwadoq.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3jnhiczgx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3mjigpvsk.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3skmmampo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3icjnvpim.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3rmxvewha.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3idskvmpb.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3fwahpetg.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3obtugjjp.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3xmxruszl.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3ggttikbw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wbyanhul.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zyexcucd.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ykxbefiq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ccuazkbd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3oobdygsc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3pkudcipm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3aoucisql.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3nzzshicc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3dpgonubx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3tvnxvgkn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3tcrkpgmn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3iumztlbh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3mqfrgdks.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3herbnsoo.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wbcpyfjz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bksnynwi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3peeufjhs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggtrufbb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kerqhaid.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yogzbywj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3riujpezn.html


<!-- 参考信息 -->