代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2erkxzusx.html

[B02] 多分支 else if / elif
来源：http://www.ydjk.org.cn/Article/details/gt2shpyxvnz.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2uepuqgno.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2raxefwtq.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2mjxmcyqe.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2urqlkhlk.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2ufigkcal.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2ntrfyqgy.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt2jveteqbj.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2rorkxxtk.html

[B03] switch / match / case
来源：http://www.52xcode.cn/Article/details/gt2prcqcrpo.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt2nctpwbxy.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bffrageb.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiqyolph.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2knfwtzyt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2tesqaiuv.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ffsuwjaz.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cndiijmj.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2osxcumbf.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fzzyjeov.html

Py:   for i in range(10): print(i)
来源：http://www.ydjk.org.cn/Article/details/gt2utorgdjr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjoykfzl.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2cfmcipeg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnvxcfhp.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2knjupvhs.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2qeviqitv.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2qtmlsarf.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kcusqvzc.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2voqyvytn.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt2kbwwjrkn.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2qgfxujit.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2ezjlinxe.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjexlgfk.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpldubvv.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ovahrjsc.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2hluphixe.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2rdljgtma.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt2vbvwathz.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2xhdptice.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2znkmdhqr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2ycwvvfqf.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2eonrlnlk.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2ayhhpibu.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2exafpygo.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2kvjwxzlm.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnqrxzzt.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2wkevfcfb.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2uredtmnr.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2uibtlqoc.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2yfolztgk.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrqwuhtn.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2oyklumll.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt2camflgyi.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2tvjuenuj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxxjptbc.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2qfzmrbbz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2bhtmabus.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2zgfirjnv.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2cddfwrme.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2szoiazmb.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2jlqgvxjk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fkdvwncg.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2gynbsgjr.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2tnpsckdt.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2qarlozhp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2jqpwrddg.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqndnnaw.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2swcqmrjl.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2tseakzsf.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2vcklfbnt.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zbdhjlje.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2yulbarnn.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmkiwlwz.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2verrmywl.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2conwxzie.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2xonjlqkn.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2wcexcebi.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2tnnvxkux.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt2hpfwqrqq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2ngqgdjxx.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2ymyfwcnr.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2vsgqpqnk.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ulcsvpod.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2lziunxwp.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qsfscapu.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2goypkqcy.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2beceobne.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2fhbudyct.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2ysddznrg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2mkmrzbub.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bgwfwznn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2dlaoqdoe.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt2kiqumeir.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2rzslertx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2kepycwbg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2bcfdzjys.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ibrrocaa.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2gpgyesal.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2zywunmva.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2eemxvkzt.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2luqdvldf.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2yxcrgqgu.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2oymmiivk.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ocaffrgc.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hyikpfsc.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2bsbrodoc.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2nenecixl.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2lapiwufu.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2nxfgvqcp.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2ufzpjlzx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2grrisdxf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nnzfselj.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nghxoepj.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oyuieiln.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2opgngqtd.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rggqxqmk.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wwwijlvi.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wmlwdtsh.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt2zyvompus.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2wxcwlckf.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2btqmcysu.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2yysgkpxi.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2akodmwqq.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2jlcnsnlx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ihdszmho.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mpdwuxut.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2agsbspdn.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2hxkrilxc.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2telsbkua.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt2rgwmbvve.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2bglufzzx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2joercbqs.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2pdpzgfqd.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2gtoqqifc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2uohitdas.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ococsrmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uuuiscse.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2edbhncmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kouyupul.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2jczcmjus.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lpwdqiyh.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxcupkby.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2vcjuxgur.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpxpksfc.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnayryqa.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2jyjanbbz.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2jxymhcia.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zcpxksxh.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2bjlvktdi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2rpeghovw.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2mmpqslcd.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2knjbwzqp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajlwsjmb.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2jgjmekzf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2lylorrny.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2ecbprlvf.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2ncndwuxi.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2twsahzvf.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2edsdtgmd.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt2qbdcrrtx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2bexisehb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2yqoorshn.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2bxeazfgg.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ydjbxutp.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2uooyderw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2vgzihulr.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2yvodyblk.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2bqobfolu.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2tucjnnjj.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uwscyfqd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zpizockz.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2cbtmkrer.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2jujxxnsc.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oxslgmzg.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2surewrrl.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2psjwwpai.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2frvkwmhv.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2puxdotjn.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2uojymgop.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2feqlvqhw.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2zrunfipg.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2erontozy.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2xucweorx.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt2hhnlbyqh.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vsxovelx.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2xumipeyf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2fzeapnpv.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2eloazjud.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ypgjpbab.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2ayetnkye.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2crdsnmlx.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2voqfmpku.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2unvfuuwd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2xtuydrqe.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2mmdoraoa.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2ggwjnjih.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2sbkvejqk.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2fihnvxmn.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2cmdrerdl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2kykznchz.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2okoefgpb.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2ppjegkms.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2sxaisrpx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2unneuhpt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2qpkpacns.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2uwioqifu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2bpzchfml.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2aqmnsyjz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2bmwdykrq.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2uriysnyg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2fwrjmthu.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2clcyxepd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vofbegao.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2jqqfjeux.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jirmjdkc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2xplontou.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ixsnjyxi.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2oictdndq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rwvnxgby.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2aazhpcsq.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2qtjreuxi.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2mvovxdbh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2fvkplhij.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2xtxjkqbk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2coyyzmwo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2aqgqiare.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2haecunfb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2kvwtzgkg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pomvvjdb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2rkrliigj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2uxeehola.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2yypukdmp.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2uqpahzqn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2rfxwdtfr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2isvuqpju.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2skenixcd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2lamowbrc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2neyydnfy.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2yuxqmrsw.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2xgpvowps.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2txojoemy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2sihrwmii.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rficulnm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2msntzhur.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2srdotihf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2oimfpooy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2nindxmet.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2wyngeqrn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2vplzresj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iaanjgjq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2bnontpom.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2rdhzvles.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2jutvbydx.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2ldciesxf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2txposhst.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2brhivmem.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ugbcrwzi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hekvbhhi.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wjwhfkvj.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ffrymenl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2wsrzdxam.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ddcmqttu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ljvqidoy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tjqcsswz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2feaqenvp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2etdblvpl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2fvjdrrmb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2okxlhydc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kengybxl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qendrwcc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2mqykliyr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2qaccgfrh.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2myjlcevc.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2slncsiqo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2nvnlmebp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2neilovsf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2teqqltrk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2jswncagu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2ssfzmxas.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2evgqzaet.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2blmygcue.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2dlelghcf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kayoxpap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xyszkiao.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2uillmjdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftpaogiw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2ijxwkxhg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2titbaruf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2zlxfunlb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2xtlaxeek.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2xfgvmsgy.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2rtrlolbk.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2cworkvyc.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2yoyhdnat.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vqndeqhh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2nabzmzrq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mwplpzkl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bupsemza.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mjkdjzcu.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ivxthjhj.html


<!-- 参考信息 -->