代发 wailian999

PHP:  trim($s); ltrim($s); rtrim($s)
来源：http://www.share.fehbvm.com/Article/details/gchsvzslx.sHtML

JS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.zdbjq.cn/Article/details/gvdjwkcmo.sHtML

TS:   s.trim(); s.trimStart(); s.trimEnd()
来源：http://blog.hesvh.cn/Article/details/grpjiaewn.sHtML

Java: s.trim(); s.strip()             # strip 支持 Unicode
来源：http://m.share.zdbjq.cn/Article/details/gnzsxmmog.sHtML

Go:   strings.TrimSpace(s)
来源：http://baike.zdbjq.cn/Article/details/gigynckdc.sHtML

Ruby: s.strip; s.lstrip; s.rstrip
来源：http://wap.zdbjq.cn/Article/details/gwqqyvigp.sHtML

C#:   s.Trim(); s.TrimStart(); s.TrimEnd()
来源：http://blog.fehbvm.com/Article/details/gwtboqttm.sHtML

[A25] 字符串比较
来源：http://wap.fehbvm.com/Article/details/gzkqraskl.sHtML

Py:   s1 == s2; s1 != s2
来源：http://wap.hesvh.cn/Article/details/gnpqnchab.sHtML

PHP:  $s1 === $s2; strcmp($s1, $s2)
来源：http://baike.zdbjq.cn/Article/details/gjxlwycgy.sHtML

JS:   s1 === s2; s1.localeCompare(s2)
来源：http://wap.hesvh.cn/Article/details/grihldymt.sHtML

TS:   s1 === s2; s1.localeCompare(s2)
来源：http://mobile.hesvh.cn/Article/details/gwzmkefxc.sHtML

Java: s1.equals(s2); s1.compareTo(s2)
来源：http://m.share.zdbjq.cn/Article/details/gyjtmgtni.sHtML

Go:   s1 == s2; strings.Compare(s1, s2)
来源：http://www.blog.fehbvm.com/Article/details/gritribvl.sHtML

Ruby: s1 == s2; s1 <=> s2
来源：http://blog.zdbjq.cn/Article/details/gltlnnmsi.sHtML

C#:   s1 == s2; string.Compare(s1, s2)
来源：http://3g.fehbvm.com/Article/details/ghfkyijzq.sHtML

[A26] 类型转换总览
来源：http://baike.fehbvm.com/Article/details/gltpdntcx.sHtML

Py:   int() float() str() bool() list() dict() tuple()
来源：http://mobile.zdbjq.cn/Article/details/gmiqqewjf.sHtML

PHP:  (int) (float) (string) (bool) (array) (object)
来源：http://www.share.zdbjq.cn/Article/details/gxdljhhvm.sHtML

JS:   Number() String() Boolean() parseInt() parseFloat()
来源：http://read.share.fehbvm.com/Article/details/gmurniwac.sHtML

TS:   Number() String() Boolean() x as number
来源：http://blog.hesvh.cn/Article/details/gwkuqhjeg.sHtML

Java: Integer.parseInt() String.valueOf() (int) (double)
来源：http://mobile.fehbvm.com/Article/details/grlnasytw.sHtML

Go:   int() float64() string() []byte()   // 需显式转换
来源：http://mobile.hesvh.cn/Article/details/gemvdbfwk.sHtML

Ruby: to_i to_f to_s to_sym to_a
来源：http://www.blog.fehbvm.com/Article/details/gphqvholn.sHtML

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.blog.hesvh.cn/Article/details/grieptfll.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gikdtoagc.sHtML

B. 流程控制
来源：http://blog.zdbjq.cn/Article/details/gtcqdnkkq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gtbuhqnck.sHtML

[B01] 条件判断 if / else
来源：http://mobile.hesvh.cn/Article/details/gigqbdpvi.sHtML

Py:   result = "正" if x > 0 else "非正"
来源：http://3g.fehbvm.com/Article/details/galuklkii.sHtML

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://wap.hesvh.cn/Article/details/giubapkki.sHtML

JS:   const r = x > 0 ? "正" : "非正";
来源：http://read.share.zdbjq.cn/Article/details/gwzciujth.sHtML

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.share.fehbvm.com/Article/details/ggqfufrlj.sHtML

Java: String r = x > 0 ? "正" : "非正";
来源：http://blog.zdbjq.cn/Article/details/gocgqrsbm.sHtML

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://wap.zdbjq.cn/Article/details/ggmdqvudt.sHtML

Ruby: r = x > 0 ? "正" : "非正"
来源：http://3g.hesvh.cn/Article/details/glhlzjbbv.sHtML

C#:   var r = x > 0 ? "正" : "非正";
来源：http://baike.zdbjq.cn/Article/details/gohkfqczz.sHtML

[B02] 多分支 else if / elif
来源：http://m.share.fehbvm.com/Article/details/gozuzhplq.sHtML

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://read.share.zdbjq.cn/Article/details/gteotjrst.sHtML

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://mobile.hesvh.cn/Article/details/gcbfvayik.sHtML

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.blog.fehbvm.com/Article/details/gplbkacdo.sHtML

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://read.share.zdbjq.cn/Article/details/gjzbunjve.sHtML

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://wap.zdbjq.cn/Article/details/gegjcdbzk.sHtML

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://read.share.zdbjq.cn/Article/details/gveuonzlz.sHtML

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.share.zdbjq.cn/Article/details/gqkrkzjwr.sHtML

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://m.share.hesvh.cn/Article/details/gixfgzpam.sHtML

[B03] switch / match / case
来源：http://read.share.zdbjq.cn/Article/details/gkoingddm.sHtML

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://blog.fehbvm.com/Article/details/gavoxqtaz.sHtML

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://mobile.zdbjq.cn/Article/details/gwzrhzozl.sHtML

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.blog.zdbjq.cn/Article/details/gonepwmzt.sHtML

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://baike.zdbjq.cn/Article/details/gwlmvzuli.sHtML

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://3g.zdbjq.cn/Article/details/gaawxflnl.sHtML

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://baike.hesvh.cn/Article/details/gzqyqisnx.sHtML

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://blog.zdbjq.cn/Article/details/gusntswhn.sHtML

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.blog.zdbjq.cn/Article/details/glpwthfoe.sHtML

[B04] for 计数循环
来源：http://wap.fehbvm.com/Article/details/guteegpnr.sHtML

Py:   for i in range(10): print(i)
来源：http://3g.zdbjq.cn/Article/details/gsvhzhrsy.sHtML

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://baike.hesvh.cn/Article/details/ggxkwmudv.sHtML

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.blog.fehbvm.com/Article/details/goighfwcl.sHtML

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://read.share.zdbjq.cn/Article/details/goeltrhyw.sHtML

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.blog.hesvh.cn/Article/details/gzbfnzaki.sHtML

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.share.fehbvm.com/Article/details/gwgospnxd.sHtML

Ruby: 10.times { |i| puts i }
来源：http://baike.fehbvm.com/Article/details/gwmottzja.sHtML

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://baike.hesvh.cn/Article/details/gxzutmxoa.sHtML

[B05] 遍历数组 / 列表
来源：http://3g.fehbvm.com/Article/details/gcvrgofut.sHtML

Py:   for item in arr: print(item)
来源：http://blog.fehbvm.com/Article/details/ghswtsmxp.sHtML

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://blog.zdbjq.cn/Article/details/gfjhoqawi.sHtML

JS:   for (const item of arr) { console.log(item); }
来源：http://baike.hesvh.cn/Article/details/gmtczgajk.sHtML

TS:   for (const item of arr) { console.log(item); }
来源：http://read.share.fehbvm.com/Article/details/grxfdxtwj.sHtML

Java: for (var item : arr) { System.out.println(item); }
来源：http://3g.fehbvm.com/Article/details/gsnwrbwht.sHtML

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://baike.fehbvm.com/Article/details/gtxvkhxsz.sHtML

Ruby: arr.each { |item| puts item }
来源：http://3g.fehbvm.com/Article/details/gfinhwgmk.sHtML

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://wap.zdbjq.cn/Article/details/gltemhdqg.sHtML

[B06] 遍历字典 / 对象
来源：http://www.m.share.fehbvm.com/Article/details/gafdjjdia.sHtML

Py:   for k, v in d.items(): print(k, v)
来源：http://m.share.fehbvm.com/Article/details/gzydbuqsb.sHtML

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://wap.zdbjq.cn/Article/details/gckpjehan.sHtML

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://wap.fehbvm.com/Article/details/gvfgudema.sHtML

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://baike.hesvh.cn/Article/details/grmaswlzs.sHtML

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://blog.fehbvm.com/Article/details/gkglcjeln.sHtML

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.m.share.hesvh.cn/Article/details/gnkccahmu.sHtML

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://wap.hesvh.cn/Article/details/grbxoexuw.sHtML

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://wap.zdbjq.cn/Article/details/grfmwidlo.sHtML

[B07] while 循环
来源：http://3g.zdbjq.cn/Article/details/gweudaibp.sHtML

Py:   while i < 10: i += 1
来源：http://3g.hesvh.cn/Article/details/glpycuznz.sHtML

PHP:  while ($i < 10) { $i++; }
来源：http://mobile.hesvh.cn/Article/details/gdtmpccpy.sHtML

JS:   while (i < 10) { i++; }
来源：http://www.blog.hesvh.cn/Article/details/gpfvnhzpo.sHtML

TS:   while (i < 10) { i++; }
来源：http://m.share.zdbjq.cn/Article/details/ghafmmazn.sHtML

Java: while (i < 10) { i++; }
来源：http://3g.zdbjq.cn/Article/details/gzvrygkpf.sHtML

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://read.share.zdbjq.cn/Article/details/glsijnhqq.sHtML

Ruby: while i < 10; i += 1; end
来源：http://wap.zdbjq.cn/Article/details/gktgpjtcl.sHtML

C#:   while (i < 10) { i++; }
来源：http://baike.fehbvm.com/Article/details/gfzhfpsde.sHtML

[B08] do-while（至少执行一次）
来源：http://blog.fehbvm.com/Article/details/grifzaprw.sHtML

Py:   # 无 do-while：用 while True + break
来源：http://www.m.share.fehbvm.com/Article/details/gjdgxjfqx.sHtML

PHP:  do { $i++; } while ($i < 10);
来源：http://www.m.share.fehbvm.com/Article/details/grehprkyz.sHtML

JS:   do { i++; } while (i < 10);
来源：http://www.m.share.hesvh.cn/Article/details/gtxfyrgis.sHtML

TS:   do { i++; } while (i < 10);
来源：http://mobile.fehbvm.com/Article/details/geykfkohn.sHtML

Java: do { i++; } while (i < 10);
来源：http://baike.zdbjq.cn/Article/details/gmanrrjsp.sHtML

Go:   for { i++; if i >= 10 { break } }
来源：http://3g.zdbjq.cn/Article/details/gfyszisor.sHtML

Ruby: begin; i += 1; end while i < 10
来源：http://mobile.zdbjq.cn/Article/details/gehbeirsz.sHtML

C#:   do { i++; } while (i < 10);
来源：http://3g.fehbvm.com/Article/details/gjlnzarpr.sHtML

[B09] break 与 continue
来源：http://wap.fehbvm.com/Article/details/gqtyflzzk.sHtML

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.share.fehbvm.com/Article/details/gfvbvxtmx.sHtML

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://3g.hesvh.cn/Article/details/gpwqleblr.sHtML

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://m.share.hesvh.cn/Article/details/gggjfesen.sHtML

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://mobile.fehbvm.com/Article/details/gesodzvxt.sHtML

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.blog.hesvh.cn/Article/details/guqwyleoy.sHtML

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.m.share.fehbvm.com/Article/details/gxexgffjq.sHtML

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://mobile.hesvh.cn/Article/details/gwgyobxyx.sHtML

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://read.share.zdbjq.cn/Article/details/gvgnopbrt.sHtML

[B10] 遍历同时拿索引
来源：http://wap.hesvh.cn/Article/details/gbczwkfte.sHtML

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.share.zdbjq.cn/Article/details/gkahoqidp.sHtML

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://read.share.zdbjq.cn/Article/details/gstizygti.sHtML

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://mobile.hesvh.cn/Article/details/gvhmootyl.sHtML

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://mobile.fehbvm.com/Article/details/gznrmjiem.sHtML

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://m.share.zdbjq.cn/Article/details/geyykjjyg.sHtML

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://blog.zdbjq.cn/Article/details/gnpbdaiju.sHtML

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.share.zdbjq.cn/Article/details/gqlytfwoy.sHtML

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://m.share.fehbvm.com/Article/details/gqviqqlcx.sHtML

[B11] 生成数字序列 / 区间
来源：http://wap.zdbjq.cn/Article/details/gkyefsynk.sHtML

Py:   list(range(0, 10, 2))
来源：http://wap.zdbjq.cn/Article/details/gksghruej.sHtML

PHP:  range(0, 10, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gqhtefzmn.sHtML

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://wap.fehbvm.com/Article/details/gaarpsizc.sHtML

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://3g.zdbjq.cn/Article/details/gqwqvfefo.sHtML

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gajcfobpk.sHtML

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.blog.hesvh.cn/Article/details/gednadyzv.sHtML

Ruby: (0...10).step(2).to_a
来源：http://3g.fehbvm.com/Article/details/glnfssepq.sHtML

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://mobile.hesvh.cn/Article/details/gkqhgxwlx.sHtML

[B12] 跳出多层循环
来源：http://read.share.zdbjq.cn/Article/details/ggftpohub.sHtML

Py:   # 无标签跳转：抽成函数用 return
来源：http://m.share.fehbvm.com/Article/details/gzojwkmmn.sHtML

PHP:  # 无标签：用 goto 或函数返回
来源：http://mobile.zdbjq.cn/Article/details/grnjgjjik.sHtML

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://m.share.fehbvm.com/Article/details/gwnihvhib.sHtML

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gszcopffj.sHtML

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.blog.zdbjq.cn/Article/details/gbaqtgydq.sHtML

Go:   # 无标签：用布尔标志或抽成函数
来源：http://wap.hesvh.cn/Article/details/gregkvxkl.sHtML

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.share.hesvh.cn/Article/details/gbrodmkos.sHtML

C#:   # 无标签：用 goto label 或布尔标志
来源：http://blog.fehbvm.com/Article/details/gwrzjsukd.sHtML

[B13] 判断是否为数字
来源：http://mobile.hesvh.cn/Article/details/gojxrqkvg.sHtML

Py:   isinstance(x, (int, float))
来源：http://mobile.zdbjq.cn/Article/details/guhdghoys.sHtML

PHP:  is_numeric($x)
来源：http://m.share.zdbjq.cn/Article/details/ghvayuoge.sHtML

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://3g.hesvh.cn/Article/details/gwnjyftoi.sHtML

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://mobile.zdbjq.cn/Article/details/gjtfvcgqs.sHtML

Java: x instanceof Number
来源：http://www.m.share.zdbjq.cn/Article/details/grrkyxppk.sHtML

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://mobile.fehbvm.com/Article/details/gvtvtngbz.sHtML

Ruby: x.is_a?(Numeric)
来源：http://wap.zdbjq.cn/Article/details/gdychtjow.sHtML

C#:   x is int or double or decimal
来源：http://www.share.fehbvm.com/Article/details/gkxomqwtu.sHtML

[B14] 判断值是否在集合内
来源：http://3g.fehbvm.com/Article/details/gfljvvvte.sHtML

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://3g.fehbvm.com/Article/details/guefhmooz.sHtML

PHP:  in_array($x, [1, 2, 3], true)
来源：http://blog.hesvh.cn/Article/details/gflzpijaz.sHtML

JS:   [1, 2, 3].includes(x)
来源：http://m.share.hesvh.cn/Article/details/gqcldalbl.sHtML

TS:   [1, 2, 3].includes(x)
来源：http://read.share.fehbvm.com/Article/details/gdykgxths.sHtML

Java: List.of(1, 2, 3).contains(x)
来源：http://www.share.fehbvm.com/Article/details/grljatqeo.sHtML

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.blog.hesvh.cn/Article/details/ggxmlmapa.sHtML

Ruby: [1, 2, 3].include?(x)
来源：http://mobile.fehbvm.com/Article/details/grberbhtx.sHtML

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gyomgmatj.sHtML

[B15] 布尔运算与取反
来源：http://wap.zdbjq.cn/Article/details/ghsnkpxog.sHtML

Py:   a and b or not c
来源：http://m.share.zdbjq.cn/Article/details/greljqjkj.sHtML

PHP:  $a && $b || !$c
来源：http://m.share.hesvh.cn/Article/details/gewgroqqn.sHtML

JS:   a && b || !c
来源：http://baike.zdbjq.cn/Article/details/gshbgtwoy.sHtML

TS:   a && b || !c
来源：http://wap.fehbvm.com/Article/details/gyiynygwu.sHtML

Java: a && b || !c
来源：http://wap.hesvh.cn/Article/details/gtakutood.sHtML

Go:   a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/godhsyazd.sHtML

Ruby: a && b || !c
来源：http://www.m.share.fehbvm.com/Article/details/grjguhuzd.sHtML

C#:   a && b || !c
来源：http://wap.zdbjq.cn/Article/details/ggxlioxnf.sHtML

[B16] 卫语句：不满足条件提前返回
来源：http://blog.zdbjq.cn/Article/details/gxackthbq.sHtML

Py:   if not data: return
来源：http://m.share.zdbjq.cn/Article/details/ggnfnekxi.sHtML

PHP:  if (!$data) { return; }
来源：http://mobile.zdbjq.cn/Article/details/gncwochbq.sHtML

JS:   if (!data) return;
来源：http://3g.fehbvm.com/Article/details/gzkulfhey.sHtML

TS:   if (!data) return;
来源：http://wap.zdbjq.cn/Article/details/gwyscmtjp.sHtML

Java: if (data == null) return;
来源：http://3g.fehbvm.com/Article/details/gxvediqzk.sHtML

Go:   if data == nil { return }
来源：http://www.share.zdbjq.cn/Article/details/ggiykejci.sHtML

Ruby: return if data.nil?
来源：http://www.blog.zdbjq.cn/Article/details/gecrgtalc.sHtML

C#:   if (data == null) return;
来源：http://read.share.zdbjq.cn/Article/details/gmofkgzyg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqxzwgmjb.sHtML

C. 函数与作用域
来源：http://3g.fehbvm.com/Article/details/gqajidrxt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghrpbhrte.sHtML

[C01] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gpnebkfeu.sHtML

Py:   def add(a, b): return a + b
来源：http://www.blog.hesvh.cn/Article/details/ggkoqjjfc.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gibxntmgw.sHtML

JS:   function add(a, b) { return a + b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpsjfodjh.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.share.hesvh.cn/Article/details/gqwyukosp.sHtML

Java: static int add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gjdyqiguv.sHtML

Go:   func add(a, b int) int { return a + b }
来源：http://blog.zdbjq.cn/Article/details/gcaksuhyr.sHtML

Ruby: def add(a, b); a + b; end
来源：http://www.m.share.zdbjq.cn/Article/details/gxowlzkqm.sHtML

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.blog.zdbjq.cn/Article/details/gnkkofmjb.sHtML

[C02] 默认参数
来源：http://www.m.share.zdbjq.cn/Article/details/gohazpcuc.sHtML

Py:   def greet(name="World"): return name
来源：http://m.share.zdbjq.cn/Article/details/gagksvsqk.sHtML

PHP:  function greet($name = "World") { return $name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwrjbvuts.sHtML

JS:   function greet(name = "World") { return name; }
来源：http://wap.fehbvm.com/Article/details/gfcsiwbia.sHtML

TS:   function greet(name: string = "World") { return name; }
来源：http://wap.hesvh.cn/Article/details/gforipoya.sHtML

Java: // 无默认参数：方法重载或 Optional
来源：http://www.share.zdbjq.cn/Article/details/grrdhugio.sHtML

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://blog.fehbvm.com/Article/details/gutpgiupg.sHtML

Ruby: def greet(name = "World") = name
来源：http://www.blog.hesvh.cn/Article/details/geitrxbok.sHtML

C#:   string Greet(string name = "World") => name;
来源：http://www.m.share.fehbvm.com/Article/details/gbxftgsvx.sHtML

[C03] 可变参数
来源：http://wap.zdbjq.cn/Article/details/gihddbmlx.sHtML

Py:   def total(*args): return sum(args)
来源：http://mobile.fehbvm.com/Article/details/goinmxgpq.sHtML

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.share.fehbvm.com/Article/details/gzvbxgtql.sHtML

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://baike.fehbvm.com/Article/details/gwbbjtbxb.sHtML

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.share.hesvh.cn/Article/details/gtchukcyb.sHtML

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://mobile.hesvh.cn/Article/details/gszwuelij.sHtML

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://wap.hesvh.cn/Article/details/gobxytqgb.sHtML

Ruby: def total(*nums); nums.sum; end
来源：http://www.share.hesvh.cn/Article/details/gejzzcsyp.sHtML

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://mobile.fehbvm.com/Article/details/gonngjxgk.sHtML

[C04] 命名参数 / 关键字参数
来源：http://read.share.fehbvm.com/Article/details/gydfxrjrm.sHtML

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://baike.fehbvm.com/Article/details/gviwcvxbq.sHtML

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://3g.fehbvm.com/Article/details/gswvjaixi.sHtML

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.blog.zdbjq.cn/Article/details/gobguhwjd.sHtML

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/giyurudnd.sHtML

Java: // 无：用 Builder 模式或 record
来源：http://mobile.zdbjq.cn/Article/details/gesarxtwm.sHtML

Go:   // 无：用配置结构体参数
来源：http://3g.zdbjq.cn/Article/details/grbojplwp.sHtML

Ruby: f(a: 1, b: 2)
来源：http://baike.zdbjq.cn/Article/details/gztjborrg.sHtML

C#:   f(a: 1, b: 2)
来源：http://mobile.hesvh.cn/Article/details/gbaxtxzyh.sHtML

[C05] 返回多个值
来源：http://www.blog.zdbjq.cn/Article/details/gyusirwao.sHtML

Py:   return a, b
来源：http://m.share.fehbvm.com/Article/details/gwgfdvrly.sHtML

PHP:  return [$a, $b];
来源：http://wap.fehbvm.com/Article/details/gviyzdjrs.sHtML

JS:   return [a, b];             // 或 return { a, b };
来源：http://mobile.fehbvm.com/Article/details/gfhplnwfr.sHtML

TS:   return { a, b };
来源：http://mobile.hesvh.cn/Article/details/gmpridkoz.sHtML

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.share.fehbvm.com/Article/details/gguowqwst.sHtML

Go:   return a, b
来源：http://3g.hesvh.cn/Article/details/geusvukpu.sHtML

Ruby: return a, b
来源：http://blog.hesvh.cn/Article/details/gmvdvwqaw.sHtML

C#:   return (a, b);              // ValueTuple
来源：http://read.share.fehbvm.com/Article/details/gypuktjfw.sHtML

[C06] 匿名函数 / lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gazbwbuly.sHtML

Py:   square = lambda x: x * x
来源：http://m.share.fehbvm.com/Article/details/gfsdckyli.sHtML

PHP:  $square = fn($x) => $x * $x;
来源：http://read.share.hesvh.cn/Article/details/gqjczivag.sHtML

JS:   const square = x => x * x;
来源：http://www.blog.zdbjq.cn/Article/details/grmcbouhw.sHtML

TS:   const square = (x: number): number => x * x;
来源：http://www.share.fehbvm.com/Article/details/gweayhnpd.sHtML

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.m.share.zdbjq.cn/Article/details/grcrlwkie.sHtML

Go:   sq := func(x int) int { return x * x }
来源：http://3g.hesvh.cn/Article/details/gxarptmlk.sHtML

Ruby: square = ->(x) { x * x }
来源：http://m.share.fehbvm.com/Article/details/gtqrzvicj.sHtML

C#:   Func<int, int> square = x => x * x;
来源：http://m.share.zdbjq.cn/Article/details/gfrmsiltd.sHtML

[C07] 把函数作为参数传入
来源：http://m.share.zdbjq.cn/Article/details/gcsldxgip.sHtML

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://mobile.hesvh.cn/Article/details/gtzmzmfqd.sHtML

PHP:  array_map("strtoupper", $arr);
来源：http://baike.zdbjq.cn/Article/details/ghzlgxwyh.sHtML

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://mobile.fehbvm.com/Article/details/ggllcssfd.sHtML

TS:   arr.map(String)
来源：http://www.m.share.zdbjq.cn/Article/details/gxihlrlyc.sHtML

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.blog.hesvh.cn/Article/details/gxvavovam.sHtML

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.m.share.fehbvm.com/Article/details/gqcdpltgl.sHtML

Ruby: arr.map(&:upcase)
来源：http://blog.zdbjq.cn/Article/details/gswuuqmxd.sHtML

C#:   arr.Select(s => s.ToUpper())
来源：http://m.share.zdbjq.cn/Article/details/gguyitzcg.sHtML

[C08] 闭包
来源：http://read.share.fehbvm.com/Article/details/grhitmsqt.sHtML

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.blog.fehbvm.com/Article/details/ghjcwqccp.sHtML

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://wap.hesvh.cn/Article/details/gcrgxvlpg.sHtML

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://read.share.hesvh.cn/Article/details/gmcmkutmp.sHtML

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://m.share.hesvh.cn/Article/details/ghmfodswj.sHtML

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://3g.zdbjq.cn/Article/details/gwicfjmwi.sHtML

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://read.share.hesvh.cn/Article/details/gleexbjus.sHtML

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.m.share.hesvh.cn/Article/details/gruuaedpa.sHtML

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.m.share.fehbvm.com/Article/details/gdbtbcict.sHtML

[C09] 递归
来源：http://wap.hesvh.cn/Article/details/goyebggtp.sHtML

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://baike.zdbjq.cn/Article/details/gbkxfazqo.sHtML

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/ghrjprmvc.sHtML

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://baike.fehbvm.com/Article/details/gmpuarcie.sHtML

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://3g.hesvh.cn/Article/details/gxdwvyvmk.sHtML

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://mobile.zdbjq.cn/Article/details/gjpmbwadz.sHtML

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.m.share.hesvh.cn/Article/details/gpuukratn.sHtML

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://3g.hesvh.cn/Article/details/gsnzmxewr.sHtML

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.share.zdbjq.cn/Article/details/gnnuvtlpy.sHtML

[C10] 变量作用域
来源：http://mobile.hesvh.cn/Article/details/gscljmniy.sHtML

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.share.zdbjq.cn/Article/details/gvbrctfxp.sHtML

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.m.share.fehbvm.com/Article/details/gfiwmajzz.sHtML

JS:   let/const 块级作用域，var 函数级作用域
来源：http://wap.fehbvm.com/Article/details/gfmsmrxlh.sHtML

TS:   同 JS
来源：http://read.share.hesvh.cn/Article/details/gncdcgvoi.sHtML

Java: 方法内为块级作用域
来源：http://wap.zdbjq.cn/Article/details/gxsjbfqdz.sHtML

Go:   花括号块级作用域
来源：http://3g.zdbjq.cn/Article/details/ggpbbxmrp.sHtML

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://3g.fehbvm.com/Article/details/gkrqepbka.sHtML

C#:   块级作用域
来源：http://www.blog.zdbjq.cn/Article/details/grlzelzic.sHtML

[C11] 模块导入与导出
来源：http://www.blog.fehbvm.com/Article/details/gnphyfpfo.sHtML

Py:   from module import func
来源：http://m.share.fehbvm.com/Article/details/ghbloctun.sHtML

PHP:  require "file.php";  或 use App\Service;
来源：http://read.share.zdbjq.cn/Article/details/guovscyvv.sHtML

JS:   export default function f() {};  import f from "./m.js";
来源：http://3g.hesvh.cn/Article/details/gfgoqckgr.sHtML

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.share.fehbvm.com/Article/details/ggbmtleed.sHtML

Java: import java.util.List;
来源：http://m.share.hesvh.cn/Article/details/gjarsvoat.sHtML

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.m.share.fehbvm.com/Article/details/gqigtouiy.sHtML

Ruby: require "json"; require_relative "./util"
来源：http://read.share.hesvh.cn/Article/details/gccvuwwms.sHtML

C#:   using System.Text;
来源：http://www.share.fehbvm.com/Article/details/gqftiyxpn.sHtML

[C12] 立即执行函数 IIFE
来源：http://3g.zdbjq.cn/Article/details/gamnheevi.sHtML

Py:   (lambda: print("run"))()
来源：http://mobile.zdbjq.cn/Article/details/gokbqznzx.sHtML

PHP:  (function () { echo "run"; })();
来源：http://mobile.hesvh.cn/Article/details/ghfmgkcdt.sHtML

JS:   (() => { console.log("run"); })();
来源：http://baike.zdbjq.cn/Article/details/gufqchtqo.sHtML

TS:   (() => { console.log("run"); })();
来源：http://3g.hesvh.cn/Article/details/gdgojvkuk.sHtML

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://baike.fehbvm.com/Article/details/gdbeyhxtj.sHtML

Go:   func() { fmt.Println("run") }()
来源：http://m.share.hesvh.cn/Article/details/gictlryfu.sHtML

Ruby: -> { puts "run" }.call
来源：http://wap.hesvh.cn/Article/details/glnmuzzto.sHtML

C#:   // 无 IIFE：用静态构造函数
来源：http://www.blog.fehbvm.com/Article/details/gnzjqpsqc.sHtML

[C13] 类型声明 / 类型注解
来源：http://3g.zdbjq.cn/Article/details/gbvvpolub.sHtML

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://m.share.hesvh.cn/Article/details/gjiorzzjv.sHtML

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gvtpmdrlo.sHtML

JS:   // 无类型（可用 JSDoc 注释）
来源：http://mobile.fehbvm.com/Article/details/gsxsnmshs.sHtML

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://read.share.zdbjq.cn/Article/details/gavvwwzvt.sHtML

Java: int add(int a, int b) { return a + b; }
来源：http://mobile.zdbjq.cn/Article/details/gzgecgcmp.sHtML

Go:   func add(a, b int) int
来源：http://read.share.hesvh.cn/Article/details/gfopmbfjk.sHtML

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.share.fehbvm.com/Article/details/gbuqrgxap.sHtML

C#:   int Add(int a, int b) => a + b;
来源：http://www.share.fehbvm.com/Article/details/gzfmxsvpu.sHtML

[C14] 泛型函数
来源：http://mobile.hesvh.cn/Article/details/gkvurnnpo.sHtML

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.m.share.hesvh.cn/Article/details/gejunaopq.sHtML

PHP:  // 无泛型
来源：http://www.m.share.hesvh.cn/Article/details/gtswwfmxx.sHtML

JS:   // 无泛型
来源：http://www.blog.fehbvm.com/Article/details/ggkvppaah.sHtML

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://mobile.hesvh.cn/Article/details/gfhwockdk.sHtML

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.m.share.fehbvm.com/Article/details/gswpxlcfp.sHtML

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.m.share.fehbvm.com/Article/details/gwrwyosgl.sHtML

Ruby: # 无泛型
来源：http://blog.hesvh.cn/Article/details/gaykjrlid.sHtML


<!-- 参考信息 -->