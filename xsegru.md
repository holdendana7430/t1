代发 wailian999

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2evavlwmp.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2tbftqwkk.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.52xcode.cn/Article/details/gt2bobuvtxl.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.52xcode.cn/Article/details/gt2wgdxujwq.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2xxxiszmb.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2hxkbrymu.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2huromzzz.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2svozzpkv.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2qwbfcmpe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2kvvijemi.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2sjzjqvpm.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt2uxtysstx.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2bswwyvoj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2jdptrrot.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2fzjuhrhs.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2tgdbazjs.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2spbiigcd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2fzlaazhb.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gneqkykw.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2nvyucmhs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2yfirovcq.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cpaqgmzm.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2tzgfohmu.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ysafcyoz.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2yykgvvrw.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2cebqvjew.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2pldgcizl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2whwrxerx.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrfqluqs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2cxmczjmt.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2lnelzsgu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2orggkvpv.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2wydyvbts.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2uhbueipj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qdakbplz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kozazlcx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2iyxzchuf.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2iynlcvyp.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2bkmsrdyj.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt2zsmwyazs.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2muflrvag.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2gxmrrjpo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2plmwdhda.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2lisdmmba.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2gacjcpzx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2wryacmrc.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2jazdcxud.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2xpcqfoyv.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2xdzrhjsx.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2fxjchgwf.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2miyzxvti.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2anasoofw.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajamuksw.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jywfkcii.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaquqbin.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2nvyiaqcz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2mdklqdkz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2iudrxebh.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2uqpsbztp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2thpbddyf.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2dyzandcp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gfbwupug.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2lrnculwx.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2pyshyzub.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2qwrnxygb.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2ozecblsg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2nflitkiq.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jiqwyrfe.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2tbqkjtvs.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2fjatmfyi.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zaxeqqzy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zezmhmim.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2qomzwmzq.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzbgqafd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2nunyvddf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2hvpahelj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2mmzyeehk.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2enrkkdni.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2jdttopcd.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2eicekyfy.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2xywlazqz.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2duxovelu.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2eepmhseu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2uulzfopu.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2mvbxuprx.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2opxwujuc.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2sjtzuspf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2pppihqml.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt2lmriaxjb.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xpgwfrtq.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2vuzwzmhz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xhyxpiqs.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2agosonsh.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2dguczlma.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2fkpqlztn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jwtejcny.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2quttgwpp.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2lriqpejc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kbqadenj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hjqgaqmp.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2onaspvgx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2cbnakfjq.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2hjksseaa.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2hzeltjpg.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2uothrqnz.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2tqimvlvl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2wfncomcl.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2igmqhvin.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zamonyex.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2vmxwwlfy.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2yribyeuv.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hfqucgjk.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2ggiqboqa.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2tijrxwse.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2ovqvznlu.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2gmgrdxny.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2khwxfmhe.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2evpveful.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ldoulbdn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2uwsxivfb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2msxpfesz.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uieehucw.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2jjxwrsrp.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2wccjabzc.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2fkjytjmd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ccmthnil.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2wjsyqxac.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2cbotjmmk.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bzwysnhu.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qjanzzzy.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2qzbxeyvs.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2dojponqi.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2fsyhbris.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2fabrecqi.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2mzhwowgs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2sjvjxzwm.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2bgehtqro.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2sauexehc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2ezwlfhfq.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zchgcpju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xkguxglo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ruekbwhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xudfkzjn.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qlepwfym.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2buftceam.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nfkhpxle.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2frhbguew.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ewtddnyo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvuhgugw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2xfgszshv.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2amfywkkw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tjddarfl.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2axatlkab.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2wuryzdjp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2crvfpfil.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybrikopm.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cxsuidjc.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt2kyqcjjti.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2fijlyulm.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2xmoclzoa.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2jiywkepb.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2nxsfuznv.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2bphcvnii.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2loorursi.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2ejzyoqru.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtilezci.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2byqrwwgu.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2iiuztcxe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2fkohujlv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2ghpdetlm.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2slxwstqc.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2xijjhzlc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2wkkuezwb.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2dwfdgzyc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fadxjgmr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2kmycarcc.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2hpjrlxbq.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2uglfxzym.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nfrbjoll.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2mcoqdzfz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uakkzoao.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2zuxxiiat.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2nrasxkxx.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2jwqpglha.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2lfijhnxr.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2ucnojfrb.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2uovmeblb.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2lfpxddms.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2pzdtvolj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zgfatscq.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2rygsldah.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2cfhfvpjm.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2qchdsbco.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt2oysqrvzv.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2rnrsdlel.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2vzfyaorm.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2nhtomfqp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2ychknaza.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vaotaxcf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nuhmwczy.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2oxjmtfuy.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2jtqwazlw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hbpzcvde.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2leyhoewf.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2kyutehqa.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2mfymfmyc.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2rdnecwme.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2sjffykfu.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjuepskf.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2mproilzz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2ycqungsm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2zsunxfrq.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2faqjaeas.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2wigpjuqo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvadyxix.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2pmxbzwyb.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvyxbbrr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2fjxehgda.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2wwmmuyti.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2ntersrct.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2msagpcat.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2fvmqdbjd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2ivvdbvwu.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2yddbwdwp.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2egottdud.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2vrrrwewt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2vvtxgkqy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2ejpvtszj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2djyicqbb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2amfrzold.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ddtcupbl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2adzfgauc.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2owrodnah.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wepudskl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2kvqaxamd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2cjrxsqht.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2iqxwvmzp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2mfvnvdlb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2yxututkr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2sqopkbzv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2mtpvpesq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2pusldsjq.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2sfnamkng.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2tiilyfsl.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2mrrmdcec.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2puersdbc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2bgjddilk.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2enxxabvw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2pqcawmww.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2bodyemwh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2wqvcbtyy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2svwnpjdp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2jkiinfjh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzbktrko.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2yllebvei.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkkpkbwe.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2fbrmfvzu.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2prtjgrzj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2cwrqxsxr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2mbpdrmxb.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2owkdvfqu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2gwpvpmqz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2psrvocyg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2nkwynhls.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ihuwsnyk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2rcfzmywr.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2acclheej.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2lbekvlkq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ggkmyzfi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2kehgywyx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2gokuokfs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mwdbnyxo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vdwsjmcw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fhcrqivu.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jqknurom.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2xxeqrdhh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2skmvxiut.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2okdevqqo.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2woajxhyk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ziazwdbr.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2zkjsmmdx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2fccvonaj.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2rbliylhl.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2udgiaign.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2dywyzcag.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2phtkeyxb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2qyutrkql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqqlnghv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gbnukobj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltpnjpbi.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2cjfredud.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2qsoqifyp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pkqepwhe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2zyktcqcw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2ppiwtcyk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2sdnmasti.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2dnzuobvy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2rnuqucld.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2oxylxazh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2qxfivxgl.html


<!-- 参考信息 -->