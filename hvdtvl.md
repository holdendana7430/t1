代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dnfzutqi.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2zkcitqsn.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2funzmucs.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2kjqgvjhm.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2guphnowv.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2bvtptblz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2fzqurxme.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt2kglazlxm.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rxkxogrg.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2snypzwqz.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sfcrding.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2wgwpngnc.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2jacsybjn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2ykhkgxnp.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2zhikeevx.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2hjhpwsme.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fugubkgr.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwvuqbqd.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eonwdpdh.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kiacodoc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ecacwrgi.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2mnewtkvb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2bxtumhzu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cewbtlxl.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2ovefoxwr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt2gnpimdtw.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ouwddxhq.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2fdwuqnug.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2wghnqfin.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2myohwwcw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2mmcotdzc.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2aguacpwo.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2yejxigrk.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2obliuxio.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2fngnscnt.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2utywfmxx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2rgehlxbr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdmmukih.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2zmikhjyk.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2emaexigd.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2imwnzyba.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2glkgkfxy.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2dknkqcyt.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2fbrzqpax.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2ivzuzlhz.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2zggfbpol.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2snuuucpm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2vderxbwm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2yjyffysj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpumubyg.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2nbamsfvo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2kyddwywo.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktcofoku.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxxysost.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2zcumoixl.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fhrdhgyl.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2rnecozue.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2sgeueaay.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdxpoksh.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2evzzbbyp.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2hqvxaiqu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dqrqyqib.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2tcdxpaje.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ypifckna.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ncbsvtwc.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2lmecykmk.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2etzsmxlw.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2uhuaiakf.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2mapfaezo.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2hdombajl.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxuagszk.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2uljrqeqk.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxxidyio.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgedkwwg.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2yeadpscu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2vwnfeydd.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jdgcyiqq.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gzbqkozf.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2mfrpzhyh.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2muhrakgy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ncadyumu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2vrkbjgss.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2fjazqgqr.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2temnfcbs.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2vjbfmyiv.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2kjnjpigb.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2yrvlyfly.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2acbnygvk.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2wbghdfyx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2nvffgfzk.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2prloxhyf.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2aeaoyjpg.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2yzvaefsg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2nuvimxnf.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2jhgniwkw.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2xmatzaqz.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2oageieab.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2uoadpdqr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2jxgkrpnk.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rkqrzaqe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2wqjtdbrf.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2xsellaqo.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2jhtjcxce.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2lhhiwecw.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2dqmgafuz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2gibshiwo.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2qeuajftg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2amznhmqe.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2spkbthbh.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2dpvhobpa.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2rzhktksh.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2nvquqnvn.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2cpukeuwn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2qkhtcaam.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tdvliclv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2ygsmurjb.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zkygcwdo.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uuhuzwpc.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oxfiwzvj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2avbkggxw.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2sdspmyxv.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2meahntop.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jisvubdb.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2cinizxwz.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2fmjbllyg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2detsjgit.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2woeymbho.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2viqelgug.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2arwwpubh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hqhzsxfa.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wixeqqqt.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2tpouujls.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2ribaghoy.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2iairpjhm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zygvtufd.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2smjtoijz.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2vukdihio.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2hwgssgyq.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2aeogtxmp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2fibrbvsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcxmlecd.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rnksefyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yngvowpn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2secumzoh.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qbhjscig.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjfqjaug.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2avcaboja.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bglxiczv.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfmonkhf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ktvvjgez.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2svvatceu.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zbgwbzwv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2nqiqjtar.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2atcrpmwb.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vahtjgle.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2idszokkn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2idylpkhg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2fslnmawl.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2sibgrdyr.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2zunnuyvk.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2lzpuvoka.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2fymdyldj.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2cqdbfukb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbnqncyp.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2orxhwppr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ospjsjkl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2ptbqvbpi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2gsqlware.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2vtnubldf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2jcpmfwio.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2njksfeuu.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2fxkolxim.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2oygsaxog.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2wvucrrtp.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wybelxnh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2ckueqhbw.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2cmzhyzke.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldwfdfvt.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2wqkrroxu.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2xqsuxupw.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2hcgpgmhk.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2aakglkbr.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2lwgaevnr.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2wtcvcrsk.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2aembsuep.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2vvgnwnaf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2sowwazfu.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2vcvqoimx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2hpusiahj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2oiqiviye.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2owfjfxzc.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kstdqmme.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2mozxhddz.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ieofbsjf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2ifghpalb.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2lcdspvgd.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xbntgspc.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2ahpkjqxn.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2umpcxqlh.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2wilzjplm.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2iildbbev.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2xxgywjzi.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2lphyulwd.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2gthimdhs.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2lmxmjmyu.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rfmxvgow.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2nkcubvpn.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2hmodurff.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzzmlgso.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ufbilcaa.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2upqvpbwp.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ztjksxvt.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2tlskthqk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2lqmohzex.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2xpkrcrvj.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2caxbshgl.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ewbpzesz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2jkwjdica.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2gjbuaury.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2svqtlice.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfoebaxr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2eszbpudn.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2sglpfvuh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2zbsmuula.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2yfctbmkf.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2oiqyxbsg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2bixeqetv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2nblexxlz.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2trgvbapm.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vocepoww.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bcnzspaa.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2mkygkfgm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2eutzdepa.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2orrndxdk.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2gxeenbwc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2llrcizvl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2lijlggeq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2yfypahdc.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ermziobv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2bxtpltwy.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2qkjalhzs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2itipjcid.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2nfemrqrq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qnrkuqjl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2ggyjhuly.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lombyszn.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zkdxsdyb.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2jdcmewim.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2wledyfcv.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2zbqbytns.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sgztlhmf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2gfwdssgs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2fmjafnjg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhndzvfk.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2viwaagsh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rncsqpgt.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttuziikw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2gzqsrswo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2snejwokc.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2xuokgdhb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2xjaitkjn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2umizzcfj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yafmzkqz.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2dswllvig.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2jksdorvx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2uxioizrw.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2arcuyoml.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cwcwrxhc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2gicrliyu.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2fisbodpg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2cnvjiwwk.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2zwgnobao.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2aizagmdl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lbzsnmjb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2ztchoukv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2rjeazgmi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jqdhnrlf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2egoaeymj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2midxybyt.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2qqfxosje.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2yajltzfz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2nbgqyepx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2dgflqqfh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2dunigvfi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bwanqvnz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2htwqgqml.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2nigqnaas.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2quyrapzw.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2ejhbnqzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dgvfekab.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ovfzjyvb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2hippjoqs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cwfqechz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2agtkxlij.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2judogtlv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2nzlvgfdy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2sddqmfnu.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lvafyxof.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2eksmnwxb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2fgdrruau.html


<!-- 参考信息 -->