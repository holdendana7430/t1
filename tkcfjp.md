代发 wailian999

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3uemidrxr.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3wgwjgeyg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3kltifbyk.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3nhvngzsc.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3sxljhtzs.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3dybezqcs.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt3urrxzdcx.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3erkvhfsj.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3falewuou.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3lzpvahji.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3nagutvjn.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3nbifjwje.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3rtfrkgab.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3umulvcdt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3molugygj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3ugxbwplp.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3pzgpqdjd.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ucmrmbpk.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3kzzhtlsk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3mmddacdm.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3iwnkokjq.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccavhhes.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3thaaavyj.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3dzgkwodu.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3zrbjxbea.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3jhhafsuv.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ppyjgoak.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mrfqqtrf.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3dsmzahga.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3pqgqmefl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3qagwvcwb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3lafvfzgs.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3vmftjlkz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3qatywhrh.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3bkmcorze.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3angkrsix.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3bivcvjhk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jmogmkdd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3abgxjvqa.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhcvkqbp.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3pjqxzdmb.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3fctuxhqi.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3ganzxdhc.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3jnamkyir.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lquujtre.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vsypwemn.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3zpwfnbnr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3zrzvpzym.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3acqggiys.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3omqhsxdm.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3zocudtgo.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3khkolysr.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3snejvsgc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3pqcegwca.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3ksydkxvv.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3infkzrfq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3hgrylubf.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3upzgpqqe.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3cqjarkzu.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3zyihtxxz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ydehyaqp.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xybwkftk.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3wzfhtxtl.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3enznmgsn.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kfzdbfku.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kxxgardy.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3vtegskpd.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3nrxvcpna.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pxnxpbws.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3qlzfrjfv.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3fccnbcjk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fxcuynlv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3eandhonu.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3vufphbzv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rccqdqza.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sztrjznl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnroziuh.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqnizjgo.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3sqdyronh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3paophssc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3hsgghvmc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3awrzesha.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3hpbgaxqw.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypvxxuxv.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3xupstgas.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tikyhhyz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3dpsyjkgn.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3rrrhkzsu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3zsinwywy.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3koiacsrw.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3kxyegzoc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3xgvlewwd.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3hszhrdkj.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3njdbytzd.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xnderhhw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3phlxdfwa.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3fufkoksv.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3homzdxkx.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3sfshrvds.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3dwtddyfb.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3gultssir.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ifehazap.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rwepionx.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3gtvfjruo.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3alhxsjnt.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3whuckysg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3wjeuscgg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3hnwqmduy.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3hrzkuwes.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3ztcmxvjr.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3lvccszct.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3mpumsujh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmwmyvoo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3qrzwhipw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3fvmvxuld.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3qrwbbvod.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3uslsynqo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3acjphcak.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3dcldtpvm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3vdjvsboo.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3yiwhwsmm.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wqtgvlzb.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qwdhvobn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qdtanlib.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wrodpvwo.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mgerboem.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3otlwobcx.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3qwdmrcnv.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3twgxravs.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hntjhfmo.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hlnxepmz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mzeyugdu.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nkfspfnu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3gknxtrbt.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gbuykksz.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3njtzzlxz.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3uimzojvm.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3qwtsmtig.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3syxikvqf.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3dfdjospl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3tpvgojyp.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3dgfgojnx.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3hwveaqsm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3hrjqlnek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lwcauryf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3weyiyzyk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jybiqcjx.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3aolgmywz.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3riwjtjiu.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmaajsxh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hyglvwkc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3urzprbzp.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aqiattca.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3twatvekc.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3ynrlusef.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekexykde.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3isbodjon.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ehobtvbn.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vpbwngnt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sttaddoi.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tcwxfhxx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3wazkiblm.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3wnifxjit.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3ibmnjiru.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3esvhdlig.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3xgeiobjj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3cpbspshz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3vppgptbv.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fmwbgjja.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3wmolcdgz.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bgpcnwsf.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3uerehudz.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3uccywalt.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3xjdabuwj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rflurseg.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3pbgqavga.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3hjbgnlcb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3acyrkicw.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3jwfwnjtl.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3icylavjs.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3fvbonanf.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3igikqsfc.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3cgihizya.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3abhmhvbi.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3bacitfyl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3qcqxvcio.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3jdkksrnx.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3efdkpzxp.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3hoiyfohm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3wuxbkazl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3qnwqirze.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3twgtiiwl.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3darocvxi.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3gyvqlxev.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3nsokshjc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ayelwpkp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oqfoydyo.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3vsanddad.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3wfeanumh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3cmfuaiyl.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ioqhpgyy.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rfbllsaj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3ztqqxvtn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3wfyjlies.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3twgkjkew.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3rkjqgjnu.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mdxkjwek.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3pjdbbbqy.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3remlatcs.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3uykozagk.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3txfqjkso.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3wrndoxmq.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3powhazvc.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmbbaxce.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3szdssbdw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3czvrcisd.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3uddozbbn.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3vsxfzwsv.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3icsenoxm.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3msiltduy.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qenlegxu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ysnwdjxa.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ubvbyfnf.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kxtabavb.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vvtoevox.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3djeqjodn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qsngabyd.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sssagmji.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3ckpqroul.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3iuokmklm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3rwcwewrm.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3vedjgojl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xeqwuukd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mpfsotoz.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3yyezqbdi.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3cpqzyxsi.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wkpeuuns.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mnvvbghj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ngutwndq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3twctvhwy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3gyyofnnv.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rhmbunuk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fbldgete.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3fhpvihfk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3sbhqcias.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3awycyatl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zeatzezz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ozgmavnq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ykyiyogb.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xzzrwjtk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3qyvyazff.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3irwxtjrl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3jpilvwjp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3uiladdqx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3opcuvynk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3eqezvnxy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3aodhbzck.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fhaqnsgg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3caemboqn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iarmivcx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhznipst.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hwdveeus.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ykcrrwou.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3lmanjcmw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3xldfjxcs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3rxgyrpiz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3xzderruy.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3psiiwsof.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3brtgfvkp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3kyqekpgk.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3pvoegizc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uacwyreb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3lofgitdy.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3zdasxeyp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3jhrpalxl.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3kcgyrbor.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3danjmmfy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcwyoyhg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hagrloep.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rquewoxy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3odvkncaa.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dowexsgs.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3xvckqkhb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lonpzzob.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3xwibfrhn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ffrjxstw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3sjpikxsw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuswcehi.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3xeschfbd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3btooiwxy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elhsxrtv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gbdstsuc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3cmtifxeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zkgyticn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3njxxnfqs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xuafqyjw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ystfbvga.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qtavtwfu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3wgomgfdg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3kcfbarzv.html


<!-- 参考信息 -->