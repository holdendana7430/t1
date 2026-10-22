代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.ydjk.org.cn/Article/details/gt2mzawyrai.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.ydjk.org.cn/Article/details/gt2uzxpkinz.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt2jqfhtffy.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt2wrpevwfy.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2emawdlpt.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2azgzaaof.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.52xcode.cn/Article/details/gt2xibdtulj.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2vfethyro.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2easumbhu.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.52xcode.cn/Article/details/gt2mmlrcmkt.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2hspvunok.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt2iehmiqbt.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2wpxyityp.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2mfzjcctm.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt2wdyywysk.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mzbvumpn.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2hzkztnbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izdrlecf.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2lcbszmoi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xihjddyt.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2dotwmayb.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2qjdgxlqk.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chyvdqnh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2hdcinxzu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rhesjafv.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ulbeexie.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2jkdjconh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2hvatfzbc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2pvwesjrs.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2pbjepqby.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2cusuhkxk.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2nqmrttgg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2dakeecku.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2mltfpjie.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2yhksrclk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2xcltapmn.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2cgbmeupn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2amqafkiw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2ottmvbsm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2wjjdahha.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqelhomd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ucabacps.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjildbkf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxomhwuo.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2oaorksfx.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qqfzfrom.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2wityagmf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gqthmzxa.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2zgrfxdsf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmutrfjy.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uktnzgzx.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fjtcjsaq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2fevdmmpb.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2bzltvaxm.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2oelvpbia.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kwjieaca.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2xnqfprrm.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2xhhmmrfy.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2xhcwlshx.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2simrqeje.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhhasqwt.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2iszobbza.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2qruaweux.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2uphaywra.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrpwvpcz.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2albtfmgp.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2lcdlaobv.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2likcxbtc.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2wxvsitww.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fwazodea.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2zqifyhiw.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2tfmrtndj.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2bxlkdajl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2ajydiqsb.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2vxbedjws.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2huxfpbua.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uahekhwv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbnjagkf.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2guewqykf.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2exiajuyf.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kckskmfp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2euhaaozx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mxgpafse.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2vemhfmsm.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2sjcszxbr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2bklgxqcq.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kxpyqfww.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2bdzukvdp.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2kqhxoohr.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lziyptzt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2rwryplmq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2amxfcrkl.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2tvmfgycb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2lwlmaqqh.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nilnxvad.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2uqglneap.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qipgbxuq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xssseobf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fwftihps.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2qhmytwtl.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zjwprboa.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2gopsbyco.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2zhvsoxat.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2xipybyqo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vrheqskb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2isdoofdw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2afabilgx.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2wcaulgtk.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2pdwfhkij.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2wrrxdrkz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2azywjcbe.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2awkzsdks.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2qxwpjdlo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2paalvsdj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kxzqlyok.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tfzzgxgc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2gdhmdjkx.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2psebuswu.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2zzezzwst.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2wytfacrb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2kdunbhrs.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2sjgysgcl.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qjmpllen.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2qctskuzp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ililvktp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2pusjazut.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2crtegzzk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2xpglpjrf.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2kbynlgqa.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2cyzzvvpa.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtucykuu.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2anmwfitm.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2eymuvxak.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2paxcflzo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2xurkcrqs.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2gislfhbo.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2ehkcgawc.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2dfdccejv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2secpanzh.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2beuvyszv.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zuzlnses.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2imzytjaz.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfyhrblw.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cojseqwz.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfdlvebt.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2puqikcpm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2gptvuixj.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2xgkbmedk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2umtyxgqg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aqsolsaz.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eqptdzwx.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2tmbzqsef.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jgultkds.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2vkwlruqe.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qochwpwb.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2effhhqkp.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2sxmlgfgb.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdjqzdft.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ackqksky.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xszzgxss.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uanjjpiu.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2unefquep.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2okewmmxr.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2zneiogfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqqczmve.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2wqijtdfg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2laywwznw.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fhsxxqwg.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2vvdprusv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oisotpua.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rfjucrol.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2kncccdju.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgzzbwsu.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2ujcrmuuz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2ilrsrijf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vtvrejbh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2xpkytfka.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2hkrxmqiu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aoxzwimd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2fnzegapy.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2iklyhjiu.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2zlztbxmb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ruuduwif.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2asjyhoir.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ykwsofzz.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2gyzpkzpg.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2mtptckgd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2mpxotdhv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2sgkhwail.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2zlttxkcl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jdthqiln.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2pqcgegmr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2csiyzmzd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2nqxnfwmt.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2kfaxcyln.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2tsqvonto.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2ocfwmcox.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2znnmsoum.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2mfnogvxd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2nagppgve.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2ucmyzomp.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yuhiddrc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2ltgjxebk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2lqommsrg.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2sbzlaogp.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2uccegffk.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ofruijqk.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2pvubznyd.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2dmcioirb.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2kvdyauxs.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jjkezlgz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2ccxlmnit.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pscqunkv.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2eituurmv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2fclffzui.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zonqewfe.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2oidsllru.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2bweuxlrj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2qxasrqlp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2kmfaodtq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2uirtugcz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ntaqlryf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2dvytfscr.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ndclvese.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2zaqtgxcj.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2ftimnoli.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2mrmagqyc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2sxpmqfjo.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2aflnipvz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2wugemyuo.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2huspvvrc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2mljhotab.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2okzoemof.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2dcjgjiof.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2tajvwwjh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2vhaqyeia.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pqhwbppk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2zrokjgwt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wmtrhmxr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2fflszgdw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2wqaaqzzm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlzactug.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2akxkliny.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2duncmiaa.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpzmymgb.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2esqfbrew.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2huqxeeaa.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2piqzbbla.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lttzhucs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ruoitori.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2muhbkmnp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zfgivwwz.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2odpxgvwi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2undwtzrx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qioitlqw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2binavxmx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jfhxotgr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2yvzrwzwv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2bgwonixz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2irpobsmf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2rxkjdyxd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2dxaquajo.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2ecmzxfum.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2zmkikuej.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2ksepxvsg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ejnguveg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2evnxarxo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2dvfssfil.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pxnosivr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2cwqgdgqc.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2iebezcij.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2quumnujk.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2tooqlqvq.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2bbzmxzlw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2kjskrtqw.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2xdftarjq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pjwzochv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ppsyhqog.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2xsettveu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfvqkaly.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhyormag.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2xpjamhif.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2fllllqta.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vdpsqykw.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2gntjqaxu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2swugvuxa.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gbooaudv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2clvwxunx.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ykznvjrw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2bekthxfl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2yqqpsjwk.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2vozwvgbb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ujlpyhqb.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2uiaqwzlf.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2enuhvhip.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2ibqtcpvf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2fllywosf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2spyuaqea.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zdsgsfxf.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mtvverdw.html


<!-- 参考信息 -->