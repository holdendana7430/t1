代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2iiyvhjvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mkapbbvj.html

B. 流程控制
来源：http://www.ydjk.org.cn/Article/details/gt2wzucniur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbytiusb.html

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt2bekzyruf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2wecbcsnn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2ssmxxlwj.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2qaalmokm.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2kutqpdrk.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2edaykutk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2hsftkcez.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2ftyedysu.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2gvanpunp.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2zrbehotn.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2bkeopyqy.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kqehiiqe.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ebbbtqts.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2bttwgbnh.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2wxbalgwd.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2bpdttcff.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2lwjdmwvk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2jwowzedw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2npfihfuj.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2iwzozvfr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqdlnsid.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2ninsinyn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2lruwiohp.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xzkfbsww.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2agngfehu.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2dqpdjnhi.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2throlhxp.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bmdfogmb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2rnymbboa.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2iamrotct.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2bsgweyzf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2qtydlpjm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2exiqgsdj.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2vmwmwxtx.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2ezsmxxyh.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2twjizadq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2pbxdkxzi.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2vgryeeul.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2hmjbdlsc.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gkrfoawt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2jkaghnje.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2eyghznxq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2qxvlkfcd.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2sflpdlps.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2aorhwqhk.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2svjuzyeq.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2lctklywg.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujcffjko.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2tezqvdxy.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2iwpcxmvi.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2gsvhifhp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ylugaqze.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lojcngyn.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2velqutzf.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2qqzjndvs.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2ldpbgwee.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2foozmmax.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2idbizqek.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttxtichj.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2loiglfmm.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2kozhhttg.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2wvcmpgyg.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mcwihywd.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2pvgsgypz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2rrmgzsxl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aiodmuos.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2dngutsny.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2xoxttqdc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ybxulqes.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2zzcirusl.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2gflmhevq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tuwyavoo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2cgzdxquz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2xamhmywq.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2izcnnxry.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujjnvoja.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2elkvrraq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2puyxpmkb.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2rzbqpqvy.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2kshjcypo.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2ssanxoqw.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2dtavvvxg.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2uhpudfit.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2zeykodvw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2ehkonyxa.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2qspcslcp.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2ztjlhkce.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2xzlkeiuq.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2lmrdvjdy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jbsbmxtl.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2nbwdvmae.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2gvefkuwy.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pztmivlb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gscnmmsb.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2gslawzvj.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rsunsdhr.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2txuahnqz.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dbueotdt.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tokkywmk.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2zuwxyfbx.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2dnfcxyxd.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2jpgxkoed.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2unuoptks.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2owunrpnc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nbhhepjs.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2meudstqp.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2vvhtgopg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2uyxjpboy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2onrfblzh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2zcmkumth.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2yqbezrhb.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2pcpccixu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kggimasg.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2yycirwxw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2tjlupmxz.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2juaiyfaw.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2hrnlbyli.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2kiectuqu.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2zjufxlkk.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2dxvuaddl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sqrecnvl.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zzkuqove.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ltwxjnxi.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2imtzerue.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sfesrhov.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2udkideiq.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2icgmmkfw.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2iimboclw.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2wrzbhclm.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2vtgkgspe.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2svvkpoti.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2euzfuddy.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2iffuffaf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kwczoarf.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2iknpxmbe.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2ucmrfccu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2aiwwiyyt.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2suozgqaj.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2ksntnayt.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2dfrladxg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2izwxrnfi.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2pfudvvaq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2hlxuerxc.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ymycwuey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bzggnkws.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2jkvzizub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vkcsqftf.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2upkhylky.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jeejxrbi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzojnsen.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfshnanx.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uyyrawjp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2waejagpg.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2oftajkzd.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2zmyqdfca.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2toblcfel.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2rsagrbph.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lrgdwxhl.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjawhcyh.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzgbejr.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eozkjznh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2cqamzony.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2wtwzgojj.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2urerygad.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ojrzxekh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2kaxojgsk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt2pbwsxclt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pxahbvlr.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xeyadtae.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2zabklfsf.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2uwlcjvrx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2dvpkbwpy.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2tzygnohx.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2oezorgir.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2wgwimhwi.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2oaoqkgxz.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2djszlxdi.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2bjrteais.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2brlgdllg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2tejelujl.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2alnaxnoh.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2lcazashm.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmsmzxsj.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gbkwjrqx.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2okdtfbhc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zrctrjzo.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2jrfkygcj.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2ygkocrrj.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2krhurzhi.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2ajkpnqvm.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2zgzwxxoy.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2qlhyscpl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2fxxzngqz.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2jgzmduad.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2qquoruvf.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mtowqxwp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2jzdrpvnv.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2horjnvof.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2wafglvud.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vjkouted.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2xigkzerc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2pkxvnjqq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2zorjvmxx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2oyafntco.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2xkymxnhk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2igkgflgw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yybellka.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wesahejf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2ozhdywrl.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2jcwxogko.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2nzfgoxbk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2mcmaotad.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2ecqhktbp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2izcgrfzh.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2cyypyhrg.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2gqusmqqd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2qijbdjsf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2heutlgab.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2njcnprvl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2cysqmsft.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2qkmzmecu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2yygbzptl.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2duhxsmro.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2igavjxzg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2useodgqi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2hvnqbzms.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mbdfbigr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2dcddfnrj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vsldqwhi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2rdysgyxj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2crcitvqn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2emiyevcr.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2kngmogay.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yuhvpmfi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2wbuugknz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2dzpqzcnu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yrybntru.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2iwreztij.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2fbagaiuk.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2jmvgcxyy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2dblbmdox.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2jwitfwyq.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2siublxgh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2mlpfbyyi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2pipsjbwm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2vmddwzyf.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2brpslirp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2igkbzqju.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2duvgtrta.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kdziyfdh.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2vgkuglha.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2botprbms.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2ottnratp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zjwgwdks.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2jvufujpk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2ofodcoeo.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2oidysgvb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ishihfwy.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2egnibube.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lpwivwst.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qaprtsxz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ysofcjct.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2blaronda.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2lqjhommy.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2yuvricnl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2qsvvnsrt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zfxbogtx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2gdaywlni.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2vllpanur.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rmmsisqk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2fzjfqtce.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ucfuvuhr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2cmtuanjl.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2eijlmqsw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2njjfyxsp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2eogmnvdt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2nsfmqjqb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ndywnpit.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nwpljhua.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2jzlgrbhy.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2jpyioaqt.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2ghlzcehs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2rsitfcbn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2fspnfcrj.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2nphdlarv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2kqbqwxrg.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hegkfowk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2udhuxkuq.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vulxbdmr.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2asmdvsvv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2owwcagwe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pyxicdoq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2cykbgrph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chvzckfn.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2mxnjncvi.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2lrgpubfo.html


<!-- 参考信息 -->