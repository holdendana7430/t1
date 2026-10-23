代发 wailian999

[B01] 条件判断 if / else
来源：http://www.ydjk.org.cn/Article/details/gt3cksnufvf.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt3txsuvtbd.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3ehrncbxx.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3etjebwmy.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3gwkspsqh.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3jbhbgvav.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3xihcodtz.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gktkigzg.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3bxvbzspv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3pmvcxwkx.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt3xxouhmvu.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3esfthirz.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3syzrewba.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3swqepwaa.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3bqvpzkhk.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3vgoubinh.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3wsxionpz.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3ubynbhtw.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3ybkqvlbm.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3dqpydykl.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3voedvxsv.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gpqztqmt.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqdhkmmd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gclnnvdr.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3upeymjvn.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ixdeqghz.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3vtsmmvav.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lwzusgdi.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3rqftynnh.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3kqiujifb.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppztadsl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3erloqjau.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3flafniwn.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3jfzeshre.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3mzpecdsg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdwumckn.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jhblwzib.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3jbbpcyhd.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3qgxorqld.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3smowckpc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qpzfhnie.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3agbgygen.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3vyujswlf.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3zrsunrjv.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3syzcttwm.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3dkdtyakc.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3tfyobrxy.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3kgkvnbow.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnkpoeol.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3anzvbdxv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ubddcknl.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3qncankew.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ssfglazb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pfzcnfxu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3oakwhaak.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3udwwsmyc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3bxpbemsw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3svfwblzy.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bwcjgjvk.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcufqwzi.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3ystmrbzl.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3oplmdkqz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3oouzgnfq.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3bxakhlne.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3taqphfiv.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tyiqhpzi.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3umkhmdjb.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3mvzkiobw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jmiuccze.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3couucdds.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3viibqtwr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3vzfzxfgi.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3ddzxkewq.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3ogapdbyz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjxoxggv.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ykgtbkur.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3auelswee.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dgsnmxju.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3lllkdvxh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3qplklpdw.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zcbujnyg.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3grgajixb.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3gmvzhbbh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3bhftccmc.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ieeqdosz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3eozunnze.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3fhmiovrp.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3ygngpcxf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3iplcixcv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3uskqrjeu.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3xqkfwsag.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3qyoclypc.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3gcajhdcr.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xdsiwebr.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3usadqezt.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3otjiwsfe.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mrrorcqf.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lnpnpxxs.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kwyaktqm.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3etzuusme.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3juskctit.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3txixbgjf.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3hgjvfbzp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3soysbtba.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ajmnuirv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3pvntfqhg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3yaqgikqy.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3vpogfbcq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3nowzwqyh.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3wwasepew.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3zdjlliyh.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3llcwjeiq.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pimgkrqf.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ixacizre.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3myngjqhb.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3vghpgicf.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3ufhsffif.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ohwivlll.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gykhsjny.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3yaphvfmq.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zmfvzsze.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nthatrni.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3pvdzwkjg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3nbxifore.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ebtzhudx.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rsdxgldm.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3auztnedp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3vepnmzlz.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3ixthvcta.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3dvbgckpq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3athhzriy.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3nkjohmvo.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ewlojqev.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3yyhrbfng.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ixlybeox.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ghxipdog.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3podcwssc.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3wsmoklen.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fpyffnkz.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3aqdvzuqe.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mcxxfxmz.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3hwcjqaab.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3lbpqbcit.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3okswbheq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rdokorye.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3iguwlegf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yadktzej.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wcbqidup.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fhnufmtz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jyztxosb.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tlrwknvn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gsmcbobs.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uwlemjkt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3xdqhrexy.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3inesemhr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bdqkyqcr.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3mveenfsu.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3khbsvgef.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3uxibveqm.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecoyyobp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zbpbxwfh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3hktqqqzl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3euqlydpr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3usviizdv.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3ommfgsnh.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3tnutmzbs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3wcyrolfo.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3rqiprgds.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3lttkjghc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3auoohbem.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zbeyneoz.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3feqmsxrm.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3cccjvvnc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3dyvmoutk.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3utvyzciu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3egzrmwjg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3xaoaqgdt.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lkoazijd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3kopnjwhg.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3mgvdcjwv.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3pwhitwzo.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3gshdjsma.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bzcwyspt.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3fgzdtiqe.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ukiansjh.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3ayehcyhq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ixcpwjpq.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3mfmnnssq.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3jvjyrtmh.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qlrqasns.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ldnfnnjd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3hckilupc.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3vjvfowhw.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dbocehme.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3ihbqlqng.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xpcnyhvp.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3nubbtqzd.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3daayislt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hcecpgwn.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3wqmvccdo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kvtwhwkj.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3tqirvtjj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3rgjpwvpn.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3orgqkiir.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3ljokolkh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3dpuexwca.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3dbdcxsjj.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3bxhmniox.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3xdmheubx.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ngcvkixm.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3epwfyadq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3nwjejzqj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3mibussby.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3bpokvscm.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3sdxvhdss.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3uzodszij.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3yhnkquyv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bmibjqpz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3okyhfyxr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3iqvctqhq.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwfulmpj.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdlocoet.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3mznlwzwy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3saykqrux.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pdpfliom.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3megmnmtf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bjdvniad.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ibclncpm.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cwltdudi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3inaxynsf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3uakohjsj.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kqsxwymd.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3btmzruif.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kvcsyazk.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3aeblyzlv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3zvxilfji.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3snnotola.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ncsurdhv.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3hgrimvca.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3kihxqyff.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3aawnuwuj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lopkfzex.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jatitbwk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3imiyhoat.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3irndiqkd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wzwivarj.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3afutdavq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ystigxlz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3yporvqoh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tjwjaxwu.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3yklodxvf.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3rhqnmist.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3kkgxdztd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3ggapdzeu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vbjhqnjn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hcykfxbw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3nsalesnb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bmkqeqvm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ecwjqpcy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qeokxqcr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mkbcaosz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3shdtmroz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ycibkura.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3gawnkwrw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vkoqbrja.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3sqfkmkzl.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ufyuigio.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3fnqlstwk.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mntxcoxm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3aqneomrb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3nesbhjfx.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qgrzbltd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3qlazjeul.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3feuoxazd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3gffsgtoa.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3tcrjvyep.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlnqutrl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3inlizscy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3ahcjyusk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3xtnogobe.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3fvqlfcah.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3sefcpfgc.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3eeavmmnf.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nnexwxxv.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3eaaqlxpp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nmotbeta.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3krbziyvc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3onegwcpl.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3oxbbbobl.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ewwgxzhd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3dfdrekiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3olxuilcn.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lcnysupd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uohxcuck.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3esvmzlhq.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3uomxfqhq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wmpjwybj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3jxxvwdna.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3dclnzpme.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3sadbjppd.html


<!-- 参考信息 -->