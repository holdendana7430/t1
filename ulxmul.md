代发 wailian999

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt2gkykrvks.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt2cybkzzrk.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt2nclcziol.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt2ciraqesc.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt2jxjmkwhj.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt2zmhkmubk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.ydjk.org.cn/Article/details/gt2vzplkcvi.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.ydjk.org.cn/Article/details/gt2fkleizid.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt2ryohbnbr.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2wtdqflhn.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt2quzqbwxv.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt2bddpcpxf.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt2lgfrshin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdieohjo.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2gkmrpgaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kwbsuzxi.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2rgjuattt.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2cfrgrpjb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2bftsjheh.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2ylxkvzst.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kudizizx.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2fdcjihqw.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2sijpmpxq.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2jqnjqvhm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2awlvvftm.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2kwwjkcum.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2avvqtuef.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kpeagakg.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2avsaqkca.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2fyzvwpjx.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2cwcaxdim.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2uxympskh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2hsixjppt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ssohtgsv.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2wnntgyuw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2wlvjnudx.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhavxftm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxugkgwg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtgsjhcu.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2aywfytwp.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2sodhskmq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2boopyvcn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tjmaasdj.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bclydhag.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2wbqielns.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2whrceqeh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkampqhw.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2gffowmmo.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2ftoyqdbc.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2yrymsprc.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ypowxjim.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2tfbkdidi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2dcmtayub.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2wwlthkya.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwnvmiel.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfdraeeo.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuiugvax.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2wexhmqzw.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2hrgyutcv.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2mfepklia.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2igdnxcob.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2tbcgrrtn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2kecmyfuc.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dhrjwohs.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekucppeh.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2qkihckwc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2xskkneqk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2xsrplidd.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2fvjujgvc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnyhplvx.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2hkbomtrc.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jzyxkblb.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2rrfxwsfv.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vnfgsldj.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2neeunmth.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytsjysws.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2hclwiyxw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2tfunmuja.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2allhvxvr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2zorcfgmw.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2evqyxjbc.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gqvbmpvx.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2kvjemlel.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2uulwhvjc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2molpcpsa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2qgpvouzv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2chtlwiqa.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ayjtnilr.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2sxfjpopj.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jazrrigu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2kktgnprj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2xkyqvlbn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wvlumfcr.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ydzujmdb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2kjowvemh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2yenzifau.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ososdmbb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hikxotvj.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2ckbhrycv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2pogvxwor.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2weuytoiy.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2emhavmby.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2zaasbvax.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2nwdgehmz.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qkjyzmtq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2ecrxloxl.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2eifjzvrg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2zdqxblab.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2ulzgutmo.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rbqltlet.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2mbmwzaru.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qkcvbzjk.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2murgfzen.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2kkxbpyzn.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qmbcfuiz.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2vegpilxo.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2gcaelgcu.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rcfvsqoo.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cnnagdfm.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ffxvjuup.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2zetuecxk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2gheyrzjy.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2nsquyica.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ojyaubyw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2zgetvrcl.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2kfrwtokt.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxhyfjxv.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rkkcoplg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oopzwaef.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2cgdwlkxt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2pqheuqun.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2fjaciven.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2jtgzevto.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2zwxcjetn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2jxqbmftg.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ptegqtfh.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2buvosove.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xitzljzu.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ihjmvwue.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2kkxlkdhw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2beoejexu.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dtwqvvrd.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2vdaycgzn.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2trluyogq.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2npwdyldf.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2kyyvluhj.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gppytjca.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2eglwucjc.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2pryessac.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2pltxpzqw.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2zqwspwdo.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2dbryihpz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2qdxmwcqx.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2weacuzuy.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yseankje.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2hgkecbpg.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vcrbzcyh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2iqamxcyo.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2taeniqio.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2djnenbku.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dgruzqot.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2ioaqcdlr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ywntzdnt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ogscdaei.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2pousvaoc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2zbxghwme.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkktkhhx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2gfvenzpf.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ihbuuawv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2kyivtalv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2rwzshrle.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dwwtqzxo.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2zdyfdyph.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2bbkxxmiy.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbpmtklm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qvkpgaff.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfhwzlsy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2yulcruku.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2dsdpewkj.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2przjdwxw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2okzvfwmy.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2rabrhjhp.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2nblvotkb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2akjcldgs.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zchrwdic.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2pbojtrfb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2igymkauv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2mcxicsbs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2uldagxze.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2cjinbafy.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2ukbzjtkg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2isyjzxpn.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oahavkxy.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrichflf.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dbzuvxpt.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2mkevasui.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2myhindks.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gnnqlszn.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2swossyqx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2kclvllel.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hedyacjk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2qiqvpwtw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2fuoxyzuo.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2nemvnfpq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2mtiwqgkf.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wfazowec.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2jaiqazvt.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2dchlkibz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2hkgrpyga.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2ndxhcymv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2xjwibpwb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2vdbptjif.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2vpkmidnn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2glwplcuc.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2xlxyryfp.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2ftipswml.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rczpodgu.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2rrsjajhg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2agrxqkml.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gwejsbhr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2tzjumwwt.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2iwxdugux.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zosbovzo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2iylcwutb.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2wkbpzbjx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2oxkpcijz.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2luiphjef.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2xadsvjde.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2nibaapmd.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2eqjcmnem.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2nfrgngkr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2wffwnphf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2lgszhzdl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2cobojxyh.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2kkuzdwpf.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2hqmdrzqk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2yfujcuwi.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wczlesmt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2mtkpkktt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bcmxigza.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mordwabo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2bbswsybg.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2thtntpdd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2xftilxhh.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2jgjwqauy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2xvuczrdm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2mugjqlfr.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2rvqftkug.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pvnmcajt.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uuyhdvfq.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2pbnoxjhu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kmvgonqf.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2jsxmdsqd.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2oufuenjr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2pguglefn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2tlgtnilu.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dauwgjkq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2cxqthugh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2midmspoj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2znaoygii.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ozodanrl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2hqdnvxjz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2yzbmfbny.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2ejstmzch.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2pvqbcnbk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2wuvsheop.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vndabqwz.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2stqgmxtr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2qxtkkhid.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2izhvbymc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2hbdnnkwo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2qgefctlu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2nflclloh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnfilxpu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2forpiwcc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzhrbtrz.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2inucvtuz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2pvcmhvbd.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2xtwecohm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2nkmqsjro.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2thojyxyn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2cgetjnwq.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2kkaeczeq.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zvmfmeec.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vmobjzjr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2depogako.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2kidlxqoj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2hxuhjrez.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2fpkuqtsc.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2xpvrjgch.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2doyggtww.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2tbviqvre.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2eprukeox.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpasqazk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2advhtjat.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2aywanmle.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2veqbgyde.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2iqdvcfvi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2edhxlrex.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2bwdqofji.html


<!-- 参考信息 -->