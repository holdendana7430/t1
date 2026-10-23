代发 wailian999

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt3whcekltp.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3gaqczpcg.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt3nmxzwmno.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3ujzpvnlu.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3gpzvmfjr.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3nekcgwnd.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt3agkklaud.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt3skveflhr.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt3mreylryi.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3rruvqhuz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3zwmkackv.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzgwxbze.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3exlmsrlx.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3xifvhlkb.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wnvrixhf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3anmqlcgr.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3jztlagna.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ckpzgveg.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3orypqthl.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fnjqocag.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qpuhrcju.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vluvygki.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dowzbize.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydzduvvs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ovzuzfzq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3ergqaucc.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3hkdoivgr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rcqutsvy.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3fhwphfrf.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3akynzklf.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3tfqotpxk.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3dkvkrqkv.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ugygyvnx.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3zdipfykz.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3oekskwxe.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3ngozqemb.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vktruafo.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3zjlmuhie.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3rwcyhwjf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3yeybrcif.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3chgvtxxk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3amwllymt.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3tvqywigj.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3tbnnblue.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3lyjabars.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3tjricsjb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3anhxyphf.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3htjahwnb.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3anfjwzcn.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3hxiinbdw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3gbxdajfk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3pbinbeys.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3egasgsla.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3lshkkivp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3gjfpsori.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3pjsszyea.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljaqujkm.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vsfprmjo.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3qycjlmbj.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3bisbspcu.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3hunqdvgu.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3adsagfff.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3pyoecugu.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3rhdkvalk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mpbsrnbf.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gdcnexmu.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3fsqhjkax.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3htwxvvbe.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3dkoahqbv.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3zrzysvfc.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3iwtxnsny.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3tiqarzym.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3lahtywma.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3yblkmuau.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3mhxcjqnd.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpxzbumi.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvlhkats.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3mmghcioc.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ueqyvicu.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3ftwcnccf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3iwiwixpl.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3yaruisme.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3wwiyscjl.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3faecjxai.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3nxeqkcwc.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3mzdbjqdu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ktsrciwh.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vvpipbwe.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xlujsykj.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3fbofxouq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3huhwjzxc.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3ugyhtcsl.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3adabdkez.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ybscmmow.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3xmacrqyz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rlqqfqcv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3brhajiwg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jsquldfz.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wrtihcqt.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3wzaxtnra.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3malwgytk.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3xkypvwyw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3flogxqqo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xnwqmzmf.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3qwdgslfb.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3slfufrys.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3finaknpi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3tanzlicu.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3smwwtazy.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3fzzlfchq.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3jzhlyshm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3otnskevi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3oudebout.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3vxqqaxim.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3vbsbzmlt.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3cuyostzy.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3vagttmmp.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3uunlzwop.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3hhdtzbgm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gzwrusbe.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rjosltal.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ilzjamjg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uvobquys.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3eweujlrs.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ybaggjxf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vkehbnlc.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3tghakpcl.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3ygetlhzs.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3wejuugck.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rczxqaqg.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nkqznvcy.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ldiwjvrs.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3vgyuiwhh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3exxsgkur.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3ptsuprwn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3juplzgxt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3pjuxnatu.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3qnhexvcy.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3ncwroqna.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rystbjsl.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3nixxyodm.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3uyptebja.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3tfnalyrx.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3egldysiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xkamydhn.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3wqgzeyqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owgvgkla.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mduutagv.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3iqeyuppj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3grcbmdvk.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3anrlhzsy.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhdizyts.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukbznadv.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3oxjlhxlv.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3sglgdmaf.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3sabzghtf.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3ptohfhdc.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3lolsppce.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3jtlijird.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ipmtdwcw.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdojwgzd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3wqwbgbia.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3oecgpuzi.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3dojynjab.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3vtxxypoh.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3gnemlnvy.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3pyxioxxv.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3mpdongex.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jdcxfzpa.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ozfpmrls.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3hundybwk.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3rcgnkdzt.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3ivqgqaep.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3zclrmzmj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rnacssni.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3yauzomtk.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3azfgkyir.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzqblcqg.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3aucggrsu.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3czhzgdrt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3kfvwdkrv.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhwdzvlp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dzrocqjb.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3hondcqfh.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hxhiusub.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3gdnmglwh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3kaionndc.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3wufqfxqi.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3ctdbvrol.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qdoxzref.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3nbrxaqtc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3tzumdwlx.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3pqsicvhd.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3wqoidlvf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3kesbsasm.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iwbnsmrl.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3womfwcfl.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3yiuvgbjz.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3qittkjgh.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3birwfzix.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3yudgeaud.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3evvdbuml.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dxyrmuey.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bnzkjfzo.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vjrwtcfz.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3hrrddryo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wfjbxheu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3fbtcubun.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3mxsqbofz.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3xknrzlwt.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3roxbzxqk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qmwkkbik.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygsazdqn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcyicwrp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qsxeewhw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3exnspjbb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3hxsldrvv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ceagpfmx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjgbwqdw.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3nsblhcyz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sjyqekvq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3jobjnlzf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3afxazytl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ikwuqfkd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3afihyouo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3moquoxoa.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gemjvppu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3nlrwjlho.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vcvhxrhp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3kdnagrce.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3dhwqxnjg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qfgehzaw.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jnfsuxfi.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dvahufhy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3fxaxbavl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3qrewwlgv.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rwbifmkm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3dbccnhzy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3rcgpkdeg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3unvfgzbq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3eglmzudh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3xbmrsggb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3kapbmskk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3noszbszw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3fwiosssi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3xgmfovfn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3mjqwvrpn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xtlujyde.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3nkquwpfe.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jxjznnqr.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3hjarmpgh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nischtsf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3uldkcfbo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gzqvgaoa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3jhzofkzo.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3opdmirsr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3uyuuzioi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlkgkwer.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3tneniqeg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kxjpdggv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aoqjhnmz.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lrnjmurh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3wdddawro.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3pjylmszg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3cgqmaoqy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ywxkedzv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3evnysgad.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tlldravo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3mflxrnhb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3cfphcygl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3dsmfyowv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hjmqhduc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jyayssfe.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3cpahrwqc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xzqnofbo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3lpomroje.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3uxlcytcy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hcfitvuo.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3epqmrdtl.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3fwdcfqfw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3omczxifv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dgvmboiv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qqjvacoj.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vgsvfqvx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3amwbsaac.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3nbvecwyv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ekkgalwg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pngjfbzs.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3rsmlrsrn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3alyphecu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3aybcnrdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nwaoflce.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3txboawjc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqapqjzl.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vitrlxce.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3gamjxccu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3uwaafoxo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3uevgjmls.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3diwtzwuv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3sfncymbw.html


<!-- 参考信息 -->