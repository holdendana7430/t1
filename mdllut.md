代发 wailian999

Py:   s1 == s2; s1 != s2
来源：http://www.52xcode.cn/Article/details/gt3votfhzav.html

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://www.52xcode.cn/Article/details/gt3xnxqwzdd.html

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3xlfprspt.html

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3nvmobhaj.html

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://www.ydjk.org.cn/Article/details/gt3zycnsuos.html

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3xsxazsvd.html

Ruby: s1 == s2; s1 <=> s2
来源：http://www.ydjk.org.cn/Article/details/gt3aewiykkc.html

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://www.52xcode.cn/Article/details/gt3qxcmankm.html

[A26] 类型转换总览
来源：http://www.52xcode.cn/Article/details/gt3eknuhygb.html

Py:   int() float() str() bool() list() dict() tuple()
来源：http://www.ydjk.org.cn/Article/details/gt3eaukextq.html

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.52xcode.cn/Article/details/gt3rnslvjyd.html

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://www.52xcode.cn/Article/details/gt3jafloine.html

TS:   Number() String() Boolean() x as number
来源：http://www.52xcode.cn/Article/details/gt3aexpqzoe.html

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://www.ydjk.org.cn/Article/details/gt3eiutbqdh.html

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://www.52xcode.cn/Article/details/gt3yrnnptif.html

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.52xcode.cn/Article/details/gt3ezxzksyx.html

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt3vrqdrriu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aydkbnne.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt3tmaxfdde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rqepwecx.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3dzfrjvvj.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3qvxmbhfr.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3sroychin.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gmotbaer.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3vurpawtm.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3icuyykfs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3wtyzpzki.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ssrlwsuj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3jpazgplc.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3dbeemjsh.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3dwgkkovv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3llzjfzrl.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3qruucmgd.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3mdyabtuj.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ezdumlal.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3pqqaibvo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3kadrwrzr.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3vycevghe.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3gzmiruoi.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3ygevytom.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hmzfxubz.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwvxbzhs.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ponhkuaf.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3kajjcrjw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3xtovfigh.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3shlzsiqy.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt3rwltaqmt.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3nvnjzcga.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt3eaedyrow.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3ulynqped.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3taexdsde.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3iuvdqhvm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3tkbveyfz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3vknvkehs.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3wnvkwsgy.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3eqsrrxww.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3fgkmyfdw.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3fhilfzir.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3rozilgie.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3opfrqgde.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yylxkkgl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3vnbqthpi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3bsgfbvqe.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3gghfoprr.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkvjbskf.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3lijtrjju.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3uuxqlcnt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3wjujabzq.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qwozflau.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3bzswpbuf.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hmvllqyq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3lfyeyykb.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3xxlmlpkt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3rckxqgtg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3vxfzjgsv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3dtxojvau.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3whhopejw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiitpelt.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cshfsfut.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bnrnkwza.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3gtmssehh.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3ejbonuye.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctnlxvjm.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vdoaxjdr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3bxjopryo.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3elffwyix.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3dndakgwq.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3lrlemmgj.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3akgpgulz.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3dtdnlxzi.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3qhfgwizf.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3izzylmao.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3dqchgacd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ehrostca.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3jvovnyrw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxabvxpo.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3rvwerhio.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hseitlhx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3utaqxfey.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3wwtnaina.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuofvlom.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ptzasmem.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3qtulsdbf.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycmpdekv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3jpurlaqf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3amrthcgz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlamcsgz.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3sokaogyp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3bxxipkgz.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3nveyfqjx.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3bpmlzixe.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3bzjcklnd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gaoyqjvb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lwqcaett.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3hiplylfl.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vbncqqrc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3sxxjloxj.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3hcjlvifo.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rwwatnqo.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bzrnrtxz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3zdxrhnsg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3dnbaezty.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ndxtfxpv.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3phfpevuj.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3yqgvnqap.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3fymtqmjt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3uhjrhwut.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3fdikkyji.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3gqvhcljc.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3nmvhlfvw.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wcuwyauz.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3dtfregju.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3hdcbusrm.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3xtugffwt.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3ggndjeam.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3jdzjotrt.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kridfpqo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3mamqjhim.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3xaopjpfy.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3vxdeaplk.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eqbwnjek.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3khpahicq.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kgsqepyr.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3rkmtuicx.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3buazznkx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qwtymccx.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3xdtsaxkj.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3xnkrmgws.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3okghsqja.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kmrwsumw.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vgiayucw.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3lbnsdict.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yryvoaad.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tegkqlzw.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3qwiadcaz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rliqejqf.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3vhiddzou.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3cvqfpeed.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rxfmwwrr.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3cezjichl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3aqmgcxyv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3ioeouydz.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zaoeoect.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dknnspzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rwdxbbdx.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3xjvgaycn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zrtvkwbe.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3sluyblox.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fvxueodl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ogvcoukk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rruymupu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqledilk.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xngeanyb.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3fwdbmrig.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3robmixia.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvaregfv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3msoqqhlb.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3rbgmjbza.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3ylhvnlyg.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3amqdrvhi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3btbakoqy.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3rinmybfa.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3tlzbtihv.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3peggmnsa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3lksyxfxc.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3lhiglvqy.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3anxbvefr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3txbjasfr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lweasatx.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3kjerzwrq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jggiywkc.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3kungxjqx.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3stiepkiw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3hivtcngs.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3pevjfhvy.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3mbcrvgwc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3errzdyml.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3galhjlup.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3rttnuqne.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3fddtungf.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3yfwyewln.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wqqmrxce.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3pevsglyy.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3aistcnba.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3vfaetjxt.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3tpbnmxhm.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3pprswnow.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3anffjvzc.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3vzjswjlq.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3lgcxhkss.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3pdtdxjhc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3oegypizv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3giqbpfgp.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3wfwhccwu.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3xwltjvkx.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rdqaoiyh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3omofvfhn.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3voienoho.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rityhwth.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3nlpkzqdw.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3dmwoxnei.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3hanwckzj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3sgxzraxh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3njcbpviv.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3tnqmdwot.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3xckfgjld.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gkwrkisa.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3vpvrurqw.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3sfgjvtlb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3bummerey.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3vhgumfiq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3eqtexsfw.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3xkqsuqgk.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jaoilbmi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3btgozlqs.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3csmzrhba.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3hizizlsj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3gviebonv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qmctslmh.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3zxdwkoge.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3exgyliiz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xoduquvz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xaghibcb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3poqykcvq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3bwcshcqu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ktzuoxbs.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qcxcjdbv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3juxkmrhd.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vfvndawb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3rkqbaqcv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3apzrgqkd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3tirqdpjn.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3towbmvqe.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ddhvfapk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xfydzvol.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3vcrqcrhj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3odfohaqy.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mqtfurcu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3dgtzqbiq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3egjoizbh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3tprorflz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3cxnagrdb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ywdmohek.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3nfkmgnsp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3lckuzrwi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3sqiyhgzd.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gbzwuuus.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3didohhcq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3lzyxnsyn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qoxqrfho.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jaaubckj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3vcypfycf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3ezcmblal.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ozkcednk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lgkcqitz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3csxvldeu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3mrkofgnc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3mfnxzahg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yicdmrkr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hyplaqob.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3swfgiyif.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ztvkxczi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ljugivlj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wpdciwgo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3cvhkeasi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ndjtxafe.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ovhdywkb.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pjeqgmgt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmvhnwgu.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qhnsnnia.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ysobhtzl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cezvbslw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3abumuoze.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3jebvjxse.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wspqwdaj.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xeirlqok.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wbdrwpur.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3buzgvmks.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3lphlsrln.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ctfdzgkc.html


<!-- 参考信息 -->