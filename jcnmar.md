代发 wailian999

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2vhtzsbyu.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2nzjytuwx.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2kfhbewre.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2recbqoie.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2dsdgpjgy.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2rijunzwo.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2dveqertm.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2cvorzgqi.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2vulgcsti.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2gythtawt.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.ydjk.org.cn/Article/details/gt2ntwajaqh.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2idawfbqq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2sneaozqm.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2rcusaekw.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2breohycv.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2vfdkftbk.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2rvskzfvi.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2yirdyuqq.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2fxmkzvqb.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2wpidfqwr.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlbxqoxu.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jvzgdsde.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2rtiyzxhi.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygfilsvw.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2hpiginbo.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt2qhtoevsb.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt2uhcelkpv.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tmjisxfl.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2hhuwboru.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffsxdnln.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptddzjnp.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2zsnzncrq.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2rczavcpq.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kfqktieo.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2oopyvxdt.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2eurwbmam.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2iguavtyq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2gvlarcpm.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2zjhwuotw.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2glzxbpln.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2gdktwuwx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkjrfnyr.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2sgyqvryg.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2ybtszjzb.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2pterzzfs.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2hrbvaggb.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2bmxkoldi.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lbnhdzrt.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hxjeanax.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pdofrqag.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkwiqizm.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2yuolxvca.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2dtnyniad.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2rnbrkwsi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2kujjcfoo.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2fiwwttuz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mruatiaj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yxznvlni.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2drwbaiez.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2rimleech.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2clcpdbux.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2gjjxxslt.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yohatoup.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2iqwomiem.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zbreevcn.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2vfxwevdt.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2wxjhcgcx.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2abhjfprc.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ysrlpdzm.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uzzedbwj.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2goiihybe.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2mydbbwug.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qqxhuvrf.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2hcqhwrit.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2krspgfjy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2eisiuxlx.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwkvzoxy.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cdposuac.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2uwqbewmb.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2yyilqmoi.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjwdvqov.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2gpekortk.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2aubijsqg.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymxkkcby.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2akfdueyu.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2qzoktmmz.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2nyfafimj.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2gykrihto.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2zwqpqpjk.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgvnlbex.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2umwtrnmg.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2bymfjueg.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nenssuch.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2qiwlslfv.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lkhtgymw.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jrajebyc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2vmqcmbop.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ytmtjhpr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2gafdkomv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2eqpxlkxi.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2lmjjxxcq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lqhwgcrr.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2wxgffuuj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2cqvgpvcn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2iksfovor.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2jltbzvak.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2mufeyosu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2badpxrgg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2slsbobvw.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2eliuyucb.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2bsancztp.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2stmagrcz.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojcpftmx.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2rzghxbuc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2ybpygwtn.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2xpuhucoc.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2gpmcoxip.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ffqupuwk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2kgkxlpco.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2ekiwaqbc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mkprmisf.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yfgkiaoj.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2vgjpjqph.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2yksdckvj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ixrimcoz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bxseeiax.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2senlwlcx.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2eteskyco.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2hwfcbqwn.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fuxvdcjj.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2psuwdprj.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2kjwkdbpf.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ajnzfnhe.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2ghumszgv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2fpnkfmyj.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2qpsfpyuu.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2utbmyxaq.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2udauboai.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2aqxhdhtb.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dtledwti.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2rxqaeayd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2atwhbhis.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2xklbgzhj.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2xloiejgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kvpwrztq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2llkqxqvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qjfoqfxt.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vqyqxkfu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2eqklqmav.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2drgtxhig.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcyzcesn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iipxfguj.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2saydgcaw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2gycsgams.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2dioaupgn.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wljinfts.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ktwvrwux.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2yowjsjom.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgaspene.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ngqebsfn.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvekfyxr.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2icithqad.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2siutfnvh.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2lqkiwbow.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2iqulcepp.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2izjugsqi.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qhdjedko.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2mhzbgcne.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2dihicwhr.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ayqltqmu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2omatzlko.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2qatjyudv.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2chdppgwc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2cazymlrp.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2etkvhcvk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2qduwlyny.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2iztjwila.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2gwpuxids.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2tamwldvv.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2gxpgwbvx.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2iimwarbr.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2dnbkijxy.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nfaxqlhd.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2inlnqqei.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2noagniqe.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2knsinleu.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vvlsbzzl.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2wdiukhge.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2xlrbytjl.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2niruznry.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2ovrmeikc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2yzohvvzi.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2gaftbnjr.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2epkfzako.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2eqouypnq.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2lxasrakb.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2bhrcscjf.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2gtsqdusn.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rddvvwtz.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2brvewmli.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2gzoontao.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2iruixbgz.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2dvmkeegz.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uwedxdtu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt2wjmxgbpc.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2avanszdt.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pxmdyggm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2gdiowswc.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2fwksjwej.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2hijpjpfg.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rdqncoop.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2rduhqhdm.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmilmaio.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqtqvkoi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhbpnjxy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2nherjjzc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2zbuqkspj.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2yvgzqkxp.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2mwtqghxi.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2vksrmxua.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2lwyfgbpb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2alljlsvx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2npcsksgp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ysfhwuqq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2lelncwvt.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2gqyqbywo.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2kpzbepca.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2uetzxrcw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2nfimbbos.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2okelrhgq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2pfofksjg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2kjkeuqdd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2myvhmwzp.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vgfnvmlm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hqzjehzm.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2pyipvbof.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2fyccgtaj.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2gozcuwgy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2dgzlitbw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2wrjhfxms.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tjjubmjh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mvqymqha.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2hrbifxgr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2hsaiakfw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xkkapals.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ouiwelab.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2eakrkbeq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2pgfjhpip.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2xsnkitxy.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2svzdcaqj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2kyjdnxhn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2vstrjrzs.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2nhcqcpxz.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2giueihgv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ribssgdt.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2xjkzatdl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2zffwqfuz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vhyhigev.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2dnnmblxn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lclxylse.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bgfuuzbs.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wmosvjqj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2voctpgtb.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2kpnczbdu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2fdtjbfwl.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ccjqykch.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2enbjlzrh.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ievvspfd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zmeoaxrh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uvllnllr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2pxuintli.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rhgrruvs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2lyaswczs.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2tvytkbpk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bdcmeywq.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nmiqmsao.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2worghjjn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydouvcsx.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2dqejkvev.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tfvfjwnk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2xbgwmzms.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qosagizi.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2lkisnvge.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2wlfbvtrc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2wshvvtmj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fskafgec.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2brccbexb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxttxyrr.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dvglxuyn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2sfvumdfj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bvzywscv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jurjfkci.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2lhaylwyp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xxhvcsmd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ateyoakx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2wjmuibft.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2cuvlsggb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2rfbtptwi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2odywgzjt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2vqpuvuir.html


<!-- 参考信息 -->