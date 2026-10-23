代发 wailian999

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3wnapxpwh.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3wefcjprn.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3sizwntiw.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ipmipdku.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ckpkhypg.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3eslkcdnk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3ltehleky.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3ncszrioq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3ksfmgunr.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt3hqsfawrf.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3jcquywqd.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3eqphjefs.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3bzjtyirg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3sqsmntfn.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3khyfrgyt.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3lnezeufu.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3fvaqwkpf.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3somwayhh.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3wqdqvzsw.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3bnijbaee.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vrsitpqj.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aidbpsdg.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyboebhl.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dukcvpss.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3ivbmmcdr.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3zwcahkyn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3uakkopub.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wbrrcrph.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3zuhdidam.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3owqloaof.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qhdjbipf.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3cwmxwvxc.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3nlltbjia.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3hnhajypg.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3dxzklidi.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3wvdxnmdi.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3zyovnflc.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3wzwzltvo.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3dxlseypo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdvhzgtv.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3poawrsya.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksnffxqz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3cmgsdrjj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3qcszjlst.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jhgxgwjq.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3ckkhpvyy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3gflnwaly.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqcaycli.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3vldclodf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3fhbmzyjc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3qoqhbxjy.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3rqqwgrgw.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3hatuhdcq.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vcoedyoa.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3bogdivkr.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3dmgsvyxj.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jgecgpxz.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tkujlmxh.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fwlstcyv.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeikcvop.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3kpdwpiyf.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3sdqovnvj.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3omjuccah.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3pbmwtnqu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3xnydhnxt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3pqqhezgn.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rlcmosjx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xtqxrmjs.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3uxmzoebk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3cmwwjgah.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3ythrpovd.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xzytwgmp.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3xmqbgbqz.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3fjxhflpw.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsjcwifc.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzzlazll.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkfjgqmu.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pekrayaa.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qcgliauf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3kvswkmzh.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3cbhfmsls.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3lyeguuuf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3vxjutlcv.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3rwrseazo.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3wlzxbkvw.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3iwtahnsl.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3szcbyfgg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3ichffjqr.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3sreermst.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxdeubig.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hyayppdx.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3zfeemfvp.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3libllfsu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xcaiggol.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3dtmelwtn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aarkvacg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3eokazjql.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3oohcelod.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fzeecqgv.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3xvurtzbp.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3mxucsksy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3gcevqulz.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vokndkho.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3abushiuy.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3avqecrec.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3tlkrpfhu.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3tjkzbirn.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3ygwarkuu.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3zsgaofqa.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3lsirdoyp.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3rsokkhud.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zhuxztho.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lyyomatv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3khrlbfay.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3kugitlyu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3dbvfzvdi.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3illwzpnu.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3frceqhub.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3cqsoexkc.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vsnvxtut.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mzogwzvn.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3wlfrfywb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ixaefuvh.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3dekqjhiy.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uwnxzjqi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xuyzlnwk.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3lbtgroqs.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3fekgzlbt.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3lnebawfi.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3stqlilcr.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3qxjgiunn.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ktyjldak.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nclmbhmx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tkqrgueq.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mqpwlahp.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3sdpxbgkd.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rfkuvglq.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrtnkxim.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3kauijlbg.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dmmhfati.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3mmuxkazz.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3tehodkgw.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3zebhylfp.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3pnfbejhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3acneiapw.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3mqiquyuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywemyykx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3frpdjqfx.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ovpbbmsf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3bievnpyt.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qkpkusxb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hlanzubu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3lxiruxlm.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3ncrasait.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3asryfyzo.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xfrxdvby.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gxrxlske.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3dchtejtr.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eowglzdm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oiczzpua.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lmpqtdlf.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3cedgbptb.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3nraqrsgw.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3tymbhwec.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3prxpamcl.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3jxnrctej.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3jpewgnbs.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3qhukregy.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hduurirw.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ytpqhsxq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyczudtx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3bhwnedmo.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3vdeiemna.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3lszdxcog.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3bxxougsl.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3yaylchup.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3eaniwjul.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrrjooag.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3hjgdirgr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3pjxsirar.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3vuquitxh.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vtruqdlk.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vsbpdhfp.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3joyikvhs.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3xqafbxwx.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3czartwrc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jwmfrdne.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3bqlzmkpx.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3erfnkctr.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dbqwwgto.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3orefthbj.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3isvfaqyb.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3gewlkpif.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3gvzcprcw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3jxadseio.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kaoqbobr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3zokpmruc.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3cteijhuw.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3dzhqhkpq.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3ylgynduu.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3klilwlgw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3wgmoegoq.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ojrxyrnx.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bgtgfhuc.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3egnmjnus.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3njsenolb.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3uoeskznp.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3drbncqrd.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mvchbnrj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3lltdanzg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3tzhthyxo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qlryljnp.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3euafwzlf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dxredwxw.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fhribjhn.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3eqhctxmg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ozhtrzlv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3vgzcguus.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3igffqowy.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3wtmvgzjj.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lwaqngoa.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ajhjxvjp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ypllitkz.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qskgurul.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3aqteuuaj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nszhabbq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nnwkxsiw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3msvpfsba.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rydntyzi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3wilpkvbf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3oaweaakc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3otshzewg.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3arjwrqlh.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bcsjtiwj.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pzowvoqp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3shnarnku.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3msqzpgav.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3kqxrfyla.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3opqvtfvz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dbpdpddf.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3prkerobt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zeklfnik.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3uqloisfv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3fdjunrxe.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wxdoimhg.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3cywpjpel.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3ngfsotrw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3jbbixdvi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3emiydpck.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3xbuxeaoy.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3antzqqkf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3icoujkee.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3syjmcove.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3piqusjkf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yovokexg.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3nkumlclf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ddhfrqlq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wypmvbuh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3axwznqht.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3ypjbmcmv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ayjhquzc.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ysdbmwdh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3nrnyvuhl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3inkgqcxj.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wstpyoob.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ymovycmw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3thonmrrs.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qfmjdles.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntmxqoob.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ujluomed.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dwvuceob.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nfuzkrfk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3inngijkj.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ymanmarx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vtlemfxq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3uxbnijsl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3bgpmtaan.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3yjpatyui.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3iksxoybe.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3olvajecz.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wcmombom.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ltuvaifo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3gfqqmpmy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3soztmdhs.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qdfwwdkr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3zzeuhpsv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3kxaxbniz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3knrmglrn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3qoupawwt.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3javnkkjg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3aogxtonj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zyrvasbc.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3aboxqtia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qgjqryjl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vbltcnlf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3irasmxbq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3vbyrokma.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nmatviyt.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3zlyicpeo.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wqsvrhzq.html


<!-- 参考信息 -->