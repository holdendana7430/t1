代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mbxnamux.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3srxkwyie.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3viiygvcm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3qyjpmyol.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3wzvwcrwg.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3vsoxcftn.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt3sxaczchq.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3egurxzjk.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmlnuhqm.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qfhjabcl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3jpskppdm.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrarejwy.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jffxbeli.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3rloslxlg.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3uvgxsslh.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3wlmorpkd.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3frxkmywp.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.52xcode.cn/Article/details/gt3tgbxqbip.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3kuwabefe.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3srtnrkaw.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3sltgkglz.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3fmmxupig.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3uigirpfm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3hexgcvgk.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3dtdcklul.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3niaqaflh.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3jjgovxis.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wquhvxie.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jjrpwmti.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3tzfmojnn.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3kwuvrzsh.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3uhkljsmo.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3trfmsugu.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3lryudkeg.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3hsbtyaqn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt3qzoxhnki.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ykaflxdp.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mysapttw.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3oodwyzpp.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3gttkntah.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3xzlrdbzt.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3rjblyqgs.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3abmdmbyo.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3mrdmodky.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbzlhfbs.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxxbetqz.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqecbnsr.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rmzcefbx.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3jxgxydwg.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3afwqknel.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dtfryovq.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3jbjgadpr.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3fadnqehs.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3bebuqdso.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jyohrsce.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kvhzyynw.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3yrqboenj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3tuzfbzxh.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3fdpedijf.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zhxirhpu.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3pooptygy.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3slxbzrkv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3swrdfuux.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fsvolgay.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qqcldcoo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3dpaakuhd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3sxastvjh.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3sjxtwtdt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3dziksnbe.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3oejzxpif.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3gdrobede.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpweqtnq.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3lugxlyip.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3eephvfvm.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahrvndns.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3dfezjhbl.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3tinozxzs.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjcwoler.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3hlszhbjp.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3jikrokpu.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3liaattmk.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3rqwicfak.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3msaiiuhe.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3njhpdtsy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3oxbcfqbb.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3albidaaq.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fzhqrxlm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ttvtcikm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ohbmrhvz.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3gkglqbxx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3givfpayp.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3nspkeexp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3tgzpcnyx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3qlcsteio.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3uhgqmwcx.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3dparupkc.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3xcuyqwse.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3qskawngm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3wxawzmwm.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tachbhzy.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rcgzhneb.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3ydajlric.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3ahlsgwqc.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ehjqzoak.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3vruryjbj.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3xoqtnndk.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3viavnmqs.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3lvikqntl.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ggmhsqma.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dnpclgbw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zrdxmjtq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3okylkabo.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfzwgjrf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eyroglcg.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3axudjndv.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3styywcko.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3eesdvnca.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3bykhwgod.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zdhkphct.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3mmkgftwv.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3peqbcxcx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3oxkcubal.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3oqpdaqrs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3unryfqmy.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3yqnxtkxv.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3mjwcttzs.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3xhtzmnxi.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3eobbxhah.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3mfkyyxxh.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3ropqqvnm.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3vvinpgxe.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3rzxlzqzq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjmenyrn.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xhejwtcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bkjjueui.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3mfodeagg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3kfmgydqn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aasjpjen.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yethkqjv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgpjudku.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvgzuunh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3kefwpbld.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3lmlpdysk.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3rmhrhkxk.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3vtwenzol.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3jjrpdkif.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3fqywscqk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbdxbxri.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xumoqzwh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3gsggqkjc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3gmffwzef.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3admaawcd.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3toolgvwo.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3wppsbeir.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3velnjwof.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3pagpayer.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzoolthl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3hojjiizu.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mecafwbv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3uzvuvwlh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3vygrzlnd.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3rreorcfm.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3yasjqoyn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3klmfwdch.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3corvkook.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3spjqweqr.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3cexqhdil.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jearipvt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3keyjjrnu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ubqztfuh.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3axolaibh.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3fsldhrff.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3geqpeffl.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3whcrxezy.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3rahbxbfw.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3bypwswsb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3wawxnkwl.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3miibojgt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xhawrxkd.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3uhndowbj.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3wueqqlms.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3cnrhfpun.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3qevcrngb.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3mdmahfdr.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ejfpyuax.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3vlhhbngg.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3cxbpjoro.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3qawdqftq.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3fspxifeo.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3rspxweba.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3mdcfhnmw.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zqxqrktj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt3ntyelsio.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3logxkdkx.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3uxoovjdu.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3sgqiywea.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3vvfnecui.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3wdnafptm.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fjuncslo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3hknqlzpz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3fomgxwip.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhihmzqn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kxrqcysr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3qomcnppo.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3xwmlkarl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3ovnfbkoc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfcfjffu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3fqjgpjjo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gjtyjnms.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3yckedapw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lbdwfvlk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kcfzwnox.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivnxyfgj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3hgifxoem.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mqjqmlzo.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cclploce.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3whmbxewk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3clopurny.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3kvzxzsfo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yhqmucsx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3lqtvxixs.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dbafwnmy.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hsaoujje.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gwmohbyj.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nnyyyfqv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3xysfsxta.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vezcluqz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3libgpchb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3seighudt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3lrotmswk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3nnzxyznj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3aleqlhkw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3qzykqiwv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3lfboqkjn.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3sqlvhoov.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3lxyqiszi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3osnslqfn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3favrqvmb.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cozlfkac.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3hzkvhxaa.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3vbtaiirk.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3hmiykvvm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3rjuahrsc.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3eukytgez.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qonpocjc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dtmqxmrg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3aibdjkvs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvxhhnmu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fzrqxths.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3tjcdpkbc.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3bqtevgrf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3przgsqyv.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3nyhsegix.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3kgffxwfm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3sdbidysi.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ngsoufya.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3istwtpjd.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xluhgmfo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3frfrpfpp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rmvifrfi.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3sibsrswp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3ijqogmmi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3ksxwmqxb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3muwpggfc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3frelilah.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3gripqopm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zpkmkgjm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3bjivcfco.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3fsruwpnd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3sbtefeqv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dppphtxv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3neqnimjq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3orgwgjjb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fumalxbl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3zdnvntsc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxuivhwz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3igodfrbk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3fjpiypue.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bexkmcyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjgjzudy.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3opfjzsdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rizcgwlk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cybsdryb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3hzsqbdmu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3lirewfyv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3qxqulavo.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3sdxhqjey.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3hbswkxim.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3kxilqglw.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qcghsohd.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3aekgzqbo.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3mrtdnjfc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3zpctizer.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ptfthune.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3japeqalg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3iiapvqls.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ywfunjlt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3qvopmlgq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3zyhueanq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3boywfibt.html


<!-- 参考信息 -->