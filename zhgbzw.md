代发 wailian999

PHP:  $name = trim(fgets(STDIN));
来源：http://www.52xcode.cn/Article/details/gt3uropwdwq.html

JS:   // Node.js：readline 模块或 process.stdin
来源：http://www.ydjk.org.cn/Article/details/gt3xnymkygd.html

TS:   // Node.js：readline 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vzvvohmr.html

Java: new Scanner(System.in).nextLine()
来源：http://www.ydjk.org.cn/Article/details/gt3unhfdipl.html

Go:   fmt.Scanln(&name)               // 或 bufio.NewReader(os.Stdin)
来源：http://www.ydjk.org.cn/Article/details/gt3mekttnax.html

Ruby: gets.chomp
来源：http://www.ydjk.org.cn/Article/details/gt3bmfgemlt.html

C#:   Console.ReadLine();
来源：http://www.52xcode.cn/Article/details/gt3htfamwjf.html

[A21] 保留指定小数位输出
来源：http://www.52xcode.cn/Article/details/gt3qyrkbwca.html

Py:   f"{3.14159:.2f}"
来源：http://www.ydjk.org.cn/Article/details/gt3kmlcfhtz.html

PHP:  number_format(3.14159, 2); sprintf("%.2f", 3.14159)
来源：http://www.52xcode.cn/Article/details/gt3xunxhrep.html

JS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3wjcdqeet.html

TS:   (3.14159).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3tcvkedlm.html

Java: String.format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3srqgenme.html

Go:   fmt.Sprintf("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3nsbepuzv.html

Ruby: format("%.2f", 3.14159)
来源：http://www.ydjk.org.cn/Article/details/gt3dhbhfyok.html

C#:   3.14159.ToString("F2")
来源：http://www.52xcode.cn/Article/details/gt3hkfvcxqo.html

[A22] 获取字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kvsmufqh.html

Py:   len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pyiwgufo.html

PHP:  strlen($s); mb_strlen($s, "UTF-8")   # 中文要用 mb_
来源：http://www.52xcode.cn/Article/details/gt3uhezhpfp.html

JS:   s.length                          # 按 UTF-16 单元计
来源：http://www.52xcode.cn/Article/details/gt3kprfppwv.html

TS:   s.length
来源：http://www.52xcode.cn/Article/details/gt3ftvclfhj.html

Java: s.length()
来源：http://www.52xcode.cn/Article/details/gt3kkscboyp.html

Go:   len(s); utf8.RuneCountInString(s)
来源：http://www.52xcode.cn/Article/details/gt3zlqdwysp.html

Ruby: s.length
来源：http://www.52xcode.cn/Article/details/gt3mhhitqzf.html

C#:   s.Length
来源：http://www.52xcode.cn/Article/details/gt3gtlkflzs.html

[A23] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mdxjhacn.html

Py:   s.upper(); s.lower(); s.title()
来源：http://www.52xcode.cn/Article/details/gt3faxoscsc.html

PHP:  strtoupper($s); strtolower($s); ucfirst($s)
来源：http://www.52xcode.cn/Article/details/gt3yjpoejfo.html

JS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3jdebcrdx.html

TS:   s.toUpperCase(); s.toLowerCase()
来源：http://www.ydjk.org.cn/Article/details/gt3guynqazg.html

Java: s.toUpperCase(); s.toLowerCase()
来源：http://www.52xcode.cn/Article/details/gt3wooeptjq.html

Go:   strings.ToUpper(s); strings.ToLower(s)
来源：http://www.52xcode.cn/Article/details/gt3afsrdgys.html

Ruby: s.upcase; s.downcase; s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zerudoid.html

C#:   s.ToUpper(); s.ToLower()
来源：http://www.52xcode.cn/Article/details/gt3moaylsmp.html

[A24] 去除首尾空白
来源：http://www.ydjk.org.cn/Article/details/gt3hxwphnoz.html

Py:   s.strip(); s.lstrip(); s.rstrip()
来源：http://www.52xcode.cn/Article/details/gt3ccbdiuit.html

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.ydjk.org.cn/Article/details/gt3dythlqqp.html

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3atklowjs.html

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://www.52xcode.cn/Article/details/gt3vnotqlil.html

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://www.52xcode.cn/Article/details/gt3swowdmnv.html

Go:   strings.TrimSpace(s)
来源：http://www.52xcode.cn/Article/details/gt3ouoxnjdh.html

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://www.ydjk.org.cn/Article/details/gt3qefcayfr.html

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://www.ydjk.org.cn/Article/details/gt3jiipflku.html

[A25] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3avuebknj.html

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt3qxykhloy.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3tgquaprv.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3lrtmxana.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3dzpzdvqc.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3jsqxzijy.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3kdidndtl.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3lqkynrxa.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3hqijzwuu.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3cmdkoluo.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt3rrwcmrsu.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3awkbcjkq.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3owdnrslr.html

TS:   Number() String() Boolean() x as number
来源：http://www.ydjk.org.cn/Article/details/gt3evcozhkp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3lvwjlwxs.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3uitrqgqp.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3bfnofegr.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3zkjoughn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpuhhuch.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3yowgvvye.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsvfknjf.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3quqrmsuv.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3qinvuixb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzsioqwl.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vdtpgvkt.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3isxouzxu.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nkqyqcpd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ksqaqiog.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3aqeuqhfw.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3saigackl.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3fxacbpil.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3lrkzmokn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cylzobbm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3wftlgeow.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bzrazidh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3eyqijnsb.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3eezwxcay.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3zuglydmt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3pgxvocwo.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3krtpljpp.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ntpgnsqs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vymvxcih.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3hfsjkygm.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xrnpnhao.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqmeuisn.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3zjuwlhyp.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3bwhcumio.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3evcsyqsu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3nfvjwhqj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3zcejsele.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3udvxyymg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogrbdbwb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcmmqamp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ruyuxrrm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3yoxzosnn.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3sjrgrpfz.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3qisqtnjy.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3umtxchkv.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3ekdbrgul.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3epshsbca.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pegcwkqf.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iirzqyfs.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kwmpdzoy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vjkjkwqz.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3pbafdclg.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3unspkbhi.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3xagkxelg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3arpgwjgi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkybhbre.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3pzhfkpek.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3amvzohmg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfduzjrj.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3fljyhpml.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3yyjrgbpw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3wxijafcl.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3iebmkfev.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3ihmavosw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3suulgqyv.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3eilkytni.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtglcnkk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rbjsyqoa.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3giqpjivd.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3umlrhzfg.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3leaandwk.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3gwthtyuc.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3ckjgzhev.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zjdonuww.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bfsbilqx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jkbtbqdq.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3donyizak.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3divtuumk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wwutwptp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tyzbesev.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3wkbtehoj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3myzjzzfc.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqrjzukr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxazjgui.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3ezrzijsf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3baumbshu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3nhbuslsj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3opxqbwqj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgyyhryk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3dhzrfcuv.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3tcrgmilx.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3delgsgom.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tjarlxxe.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3rbdztnnb.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhxfncft.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3cizqyjsw.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3mpyeoeoe.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3omkgqqiq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3asecanmw.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bfafkale.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gcefjckc.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3mxmxfpth.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3qnhqcgvq.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3hoiiwtnq.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3huzwpgyj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3vfrjhmkw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kifusqdm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ihhwljue.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lsnzdfqk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ymyyyihp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jdmkjzhc.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3chxuurdd.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3thnmixoe.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3xqilkaqa.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3klmpyssv.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3chdqybuc.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3xktcworm.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qxmpzsys.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3mahjjnkp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zjllzleh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iauemvjt.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3jrhrqopy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3mmpiitbf.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ccvtqxdp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3aucrmvrl.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ambldntd.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3zazxyuef.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3kjvjwdxa.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3beihoexc.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wyunktvq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qhdaivcn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3pwptwkuy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3jtrjzrcd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nunpgsft.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3llwuwjov.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3rewlhwwp.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3rseuzhuq.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vgjmifwy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3luhfwtuv.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vzmsibnx.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mmceulis.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sdjbwewv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3aqmqugit.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ufjevqbr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vbzuexys.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3llnxyhcq.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3bbzlrufw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rakznbuq.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pjtkpnks.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3navokfuh.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3lkfkvgvl.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3vamtnsvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvifgqwn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3ruoqgbkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxeyqdkt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3buhzmofw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fvfmngdv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3svecutlf.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3eqjmnvvi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lthhwgrh.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hlyphdrq.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3oehzecqs.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3wjaqvvzr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3avnudghy.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nhlbbivt.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3ksmliins.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlmctyqz.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3svujwxrf.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zavlhmum.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3uninffce.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tktxfjew.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3fhvpqgak.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3kqelmijl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3ntzhdlyr.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3qzqwzptv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3inrlkvup.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nchiqdiy.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3ymivupak.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3smlvsuvi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3gegvfnov.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3zabovqsv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3cmkifbwe.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3htvcvzzs.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3yeemwfde.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3krvkwzlc.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmmpdfpd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3slpsztcp.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3bvpsvdvs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3wxkeprve.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfvmvicl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3wdebaovd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3nsqvwnby.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ktapdanc.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3oxlahjcd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3pfjbtxzf.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3naanxwwi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3zxsstmoy.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qswregdt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3hzdflqfb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ektrgmdv.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3peseymyh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3ygamybrv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3ilnbgvsj.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fvgmscoe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3jrukgfhe.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3crtolizr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3nhbffxvs.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3ozgilumr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fpphdywn.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rihgtoqq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3wfdddgvl.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cdjqcfha.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3wmudtbnk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ukfuasva.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3jafmxsmt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3klzecukc.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3fwlfascx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3xkplmmrc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3wmdgdiep.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3pivbrlht.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygvldjjl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhphgryr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipvzsqzt.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3edgphudz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3dhduqjgu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3mcpmccfg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ebiiursh.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3oxpdjrqe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3kblvtrzm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zsnfsrwd.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3szokcebq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kdqqhdfp.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3collxkcv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3vtdwpnlv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3plhkbvmu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rvfpnrjw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uibffqdf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3gufrduzp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vnnfvytw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3jrcojirp.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3dyjtsefp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hluwvxrs.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zmxbrbue.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3lsyhtcdd.html


<!-- 参考信息 -->