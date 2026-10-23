代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3qtoenuwc.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3bojjdics.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3weusbczt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.52xcode.cn/Article/details/gt3okkslbxv.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.52xcode.cn/Article/details/gt3cxunupsg.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.ydjk.org.cn/Article/details/gt3yqgctsps.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3dzilersh.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3zcgwinju.html

[A26] 类型转换总览
来源：http://www.ydjk.org.cn/Article/details/gt3jkfiednb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3svgfnysk.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rtjzlgqj.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3nltrfgll.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3rnzvfiri.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3avrgvgul.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.ydjk.org.cn/Article/details/gt3firlzvzz.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rmvgmqfq.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vlosgvlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbhlgguz.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt3pgajhdse.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ypuddnmm.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3gdqejycl.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3yojzcajb.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qmvoxday.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3swpdeocd.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3aenxkrec.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3vwptkedj.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3zpvkbdxy.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt3trovkikz.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3tlpelxer.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3niyubapc.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3vajqsuap.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wccbofvm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3jybquqwj.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mkvvsljt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ztafwatf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3igppbmoc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3wkxkfich.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vsexnokf.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3walfifbm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3bpnbjsoa.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbcytlfh.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3crhlcchd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwujybql.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsmqooge.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3bojiohba.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3voecartu.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3raqfbarr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ppwhfpvt.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ssjzpyaa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3bvkrlxno.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3hfvrlyjp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqyqtnpr.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbilplpx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3ltlqwwro.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3zjyubgqp.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3muizsfuu.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3koplzpiu.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3uypccwwk.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3iblnffpm.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3kzbzkgll.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uroyocww.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3xbnqcrze.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ybxtaheo.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3kpyholho.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzacofja.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3iomhnhco.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3sdrxjolt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nguexzrz.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ggwswscv.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mzmspvau.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3kxczifjf.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3vntmwlzk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3muhmystj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zoztvkjb.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3ulvspiya.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3cdobhlog.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaxunwqb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgrqakko.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezzjqcuz.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtmjkdcy.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3gvzjvxpt.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3loyojvdl.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbhdhorr.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3zxosqyny.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3wlslcwpb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fuksepyq.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sqdzgumv.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wzhwbkne.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nggxvisa.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3uhetvlrj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3mcsvdtvp.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yttnsqjw.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3mvclrlqp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3zihvrjas.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pyfnrtga.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qlmvirnt.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dpdnaroa.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvwzzmgu.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qyethnay.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3kxmotivc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3eusuqrsn.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3azqdivfw.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3ysbskqdn.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3ymqwkdhi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3fjimcecx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ffweciro.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3pxzahixc.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3noybbgng.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3iqosxgxh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3xhciloif.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ochwxfpi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3gcdrogak.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gyfqigom.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lcpdcaaj.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3zxixbvoc.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3qdhiqytc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3plbhwfqk.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3loxgwnri.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3inbhdiyt.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3qnvwbsiy.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3lnsbrkdx.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3jistptru.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3btaydvxk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ljcejmiw.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3dxxsitqt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ijzvlhbq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3gswrcfqz.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3debhyzwy.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3whtiocru.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3iggjtnel.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3ueieyhsj.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vsqhwrzr.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xiujazgc.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3gnxavrgt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3apgweerc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ayllmerc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vmbmatwk.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mcydbbbz.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3vghtozga.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3tpxjjyip.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bcmjoybf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pekeiwpc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ktgsyfjk.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nejjiavf.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hboozhgk.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sbjpbajz.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3wimbcuhx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3vdjfeuvc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uqghbive.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3noplpqnr.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uzsyqebu.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3dlpnmakr.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xvbugowf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lrrxssdp.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3tiqqzgit.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3uawyjjzr.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3mvgqzhov.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlaencoc.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3uhikfqbg.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3pgagydst.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ipponccv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3upnkfixf.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3cclyqfgi.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xzdyfwry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wwqcskjm.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3uyrcqchx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3awlfpmih.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3emyvehmm.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3horpztnm.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zrxznmuk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhmjarai.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ldmwaozj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kucxorid.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rpbmjqsp.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3zrzkrvfd.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dijjptdm.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ugnrjajj.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3klbqveqc.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zetqwhmm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fhbssqjl.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eykovcqm.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3ebclzzxa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3lwuoeugb.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3fpoxwnjh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3pbhhwxsh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3gcefnrrx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3fjssryhl.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3lebfehwv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmpyzfod.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxkoeawe.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddljcbch.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3buvmtzfr.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3fmjameds.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3iswnwebu.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3srcrkkib.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3symlvogg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xckfckxj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcpaikwj.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3wtgoesvw.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3otkxjgkd.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3waknakkl.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3reydqpqy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dpgdeqgb.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3wlnnhysb.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3acducqmg.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ccgteplx.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pwjpjvgp.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jrjblwsy.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3dxztvwps.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3mjlonyde.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3jigdyphu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3sstugvgz.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3gqacgdao.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3qvgtymnm.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3xlowwhcv.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3jlwasoss.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3npkvpyua.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vbesyozl.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dadcczro.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3tsirjezr.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ulboxedi.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3knwtccol.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3oxxfyxyf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3stgycdwq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3upbdaulx.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3pncilusq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3ekjhpddh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3cugubksv.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3kqhwmppr.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3oynsgygw.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ywosgjbz.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3jczezzsg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xyrgvrsa.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpgztktr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sayxivqc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3fudjoapz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3bsybvcqt.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3mgtklokx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3hhrhxuya.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3jsfmgpdw.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zeqzescf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kikjswti.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ooskcwgf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3dtxyggee.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3disqirgk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nlwsxaqm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3glymfdng.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3chqflbro.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zqygerpd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3dpviramf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3stklxizn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rhuosnmg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3vvlrkxij.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ccdlwpud.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ayajbofv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zopvuhlt.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3upstsphm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3sgwwiipg.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3oqvsmksz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3kdfbgpvg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3zmjpvrkt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3ugmyfutb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3qkbkuprj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ryjhckce.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3upmgittv.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3uacarmwg.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3iebwhlka.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ayzfakph.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3gatgmoal.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ghkofwlf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xwspzlab.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3csglqehb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jxjkkenh.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3vxhthmzy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3knbdjfvn.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3shzsvmtl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wnqrfmjq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mszkmhug.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3qwngijeg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tyawxili.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rfqilzop.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3eqjpxmhh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3kquocbdg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3qlaapmcg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3iznahswe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3dysmbqox.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oorumyyg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ttltxxfd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3etwycezh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3umwrofrx.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3moypputm.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3qvakngwh.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rfbntqtt.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cremkmfh.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hmasbdwf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3orekbsxz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3iprbiyrc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3keopgsgi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kfogrrmp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sqtllavl.html


<!-- 参考信息 -->