代发 wailian999

C#:   Convert.ToInt32() Convert.ToString() (int) (double)
来源：http://www.52xcode.cn/Article/details/gt2jzekurvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdejsdfx.html

B. 流程控制
来源：http://www.52xcode.cn/Article/details/gt2okxpndtp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbmfvtmz.html

[B01] 条件判断 if / else
来源：http://www.52xcode.cn/Article/details/gt2bcnurmcq.html

Py:   result = "正" if x > 0 else "非正"
来源：http://www.52xcode.cn/Article/details/gt2rhxynzjp.html

PHP:  if ($x > 0) { $r = "正"; } else { $r = "非正"; }
来源：http://www.52xcode.cn/Article/details/gt2agidolza.html

JS:   const r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2mnyrtroj.html

TS:   const r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2qutwcjbq.html

Java: String r = x > 0 ? "正" : "非正";
来源：http://www.ydjk.org.cn/Article/details/gt2bthsnfui.html

Go:   if x > 0 { r = "正" } else { r = "非正" }
来源：http://www.ydjk.org.cn/Article/details/gt2iynkhsyh.html

Ruby: r = x > 0 ? "正" : "非正"
来源：http://www.ydjk.org.cn/Article/details/gt2qjdmzysc.html

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt2blrwvkmq.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt2irysgiow.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt2xudijbdf.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dqqemaay.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lcxcqjab.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt2uninstrt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2xlmibere.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt2qtgscglo.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt2dczqeahk.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt2lhewmttl.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt2jphyuxba.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt2suvfxfqb.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qucqntan.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2jwwxphrn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2porlvsdt.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2vzfpqobz.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2ejqdtxsv.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2cydrattp.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2pheyonwt.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jquatuaj.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2fovvkvli.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2zhwwlimr.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2aewqqmll.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2exuyvria.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2fbbulcze.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2kmlpfsat.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2fbjqpczg.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2kipaxtnn.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sxpsygqq.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2zhehjlyg.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2wjxvhzqz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2gbyhqwzm.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2vudxegrr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kiojnltf.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2vjphrtkq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2bwhfdyjc.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2bblppgex.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2kbspfnhj.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2qtzggskq.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2shcimotu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2hwlvkzqw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2cilndhtr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2ojgptgow.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2nbisvdkf.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2oscidkcu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2lnvvwgdn.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2buvsyyja.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pisldvrd.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2knkfjllh.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xrqabyqs.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkzmfsyg.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjcqqgks.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2ehgijzqe.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2bqdwimfi.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipkasxwk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2khiakcxb.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt2xsshtnpb.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cmnkfyqg.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2rcssafic.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2nqppcypy.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2gnhsmzgs.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2fbdmrekf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2tsqmltrz.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2wrgcbkve.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2msbcwint.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2wadsoivz.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cueuyfvn.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2cttqrmyn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvhuynyk.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2iodndhnd.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt2ohfatjma.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2pxtfxurf.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2svobiene.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2utficgna.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2muhuubdo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2nrdezpzi.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2xkxylecs.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2pmblzurs.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugciuilw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2vzmjcgub.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2ijmivlaq.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2dypmzuty.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2vwdudebn.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2xaotzwwi.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hnrwlpos.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2pgsndggw.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xectuguv.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2iuqduecx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2oigxdkso.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qisfzjsc.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2aszbwowy.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2tmjiriua.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2cqsoxuue.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2yfilhyjk.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jdryatga.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2nmilfiox.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2pdyzcxbv.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2phmlsfpl.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2msgentub.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ditblqyk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt2hmhpddin.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2zophwonz.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt2sguuywsr.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2otwksnxk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nbrxntyw.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2nwfqpthn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2aqunrhgp.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2raunvmnu.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2lanbluys.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2vmpvhqtg.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2tvtwjmzl.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2sdaymety.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2duahfqun.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qktjdjwa.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tjqggjlg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2kngwjfsr.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fudrieqf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dtjaagyg.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2waqumaow.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2upoiadki.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2ieyiwpjb.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2egllpiky.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2bmwluwhz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2aklhwbxs.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2dvpechwx.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2axbchsxz.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2geiegshm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2mycovyhr.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2wqszbgtp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmgbrtna.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vlzuciqx.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2poabozbx.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2snwvfzjg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xcmfnyzl.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2fvvxfxya.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2xushucbc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pgxerdjv.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2qsifzdzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krkpbqlf.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cxjlxspl.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2wwipwigc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mrvnbosr.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2otihpwdg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lovdzhtu.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ztaftltr.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2iqbchvfy.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2dlezylir.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2iookbasq.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2jruptacf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2lbsyeyrf.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2utfoclku.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2surfzkxc.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yqlnbgpd.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2wcrpxioh.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2pnzmnwxy.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2hotgylhz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2gjftqkrq.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2mvrbdtat.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2igsuidvr.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2rgmeafgu.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2lynfdwyk.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2xlfytojt.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2aadvysky.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt2mznncwvi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2nokutvin.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt2ygpyuyzw.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2dktfqmbr.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt2dosegbej.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2lzufkxcz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rendgfzv.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kqhpeblc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2xuxweshh.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2cxqgbfag.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2jzbponat.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2woguzqzx.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2gddrnwmi.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2mafyiapc.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2vmkoaksd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2vowawfhy.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2irqvqjvg.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2ogouxbrc.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2yppfhsgt.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2udslafxi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2tjjhpfgx.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2asbbinlu.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2yamfhvvw.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2xettwlno.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2cmaaahkj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2zkoofhtm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2rlazibgt.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2mpaxyihg.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2rzcgqfis.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2tvoilnpf.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2wkzgensb.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2rdclbndg.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2paphberj.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2tscktufp.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2fbyecvhj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rsxefoub.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt2uebazbqu.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2vtkeyzsy.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2udqlixnr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ltwddmwr.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2nozetlbg.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2hmdcswxi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yikqdpnu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2joqbnpkw.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2ofqoaobg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2pluagbao.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2sgtispyf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2oekudljo.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2exgwdkxn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2knzdquwp.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkkdcbwy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2agfylpvp.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2cjymudht.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2axssypbp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2hufbgbip.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2jkqdsdys.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2vrqzeuja.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ptlvyqsh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2lnbfoung.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2xkdmxjux.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ypxbyusa.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2frsojrvn.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2nvfveywc.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hvynxbtp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2hrfhoytn.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2hftviigi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2rchtmdlr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vuwldbid.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2cjoydkli.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2curkocnt.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2epiikprm.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2frzerrmj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2escteezc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2vkqykjqv.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2ozcwikem.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2bvgtedej.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2gutibphq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2jaevawqy.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2updkjkrv.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2weyxwgsr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2lelduyzc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2lxugfztw.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2lagfhwrr.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qjrbrgmu.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2umsrhiks.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2kobxsxuq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2mmsqoksz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2hdiwxskr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiosdmvl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2iucbbrne.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2xqblsfqh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2otljkgqm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2crenjnii.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2jdgqhghb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2xctdazkf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2zobneprq.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2psyeayzb.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2eazslkhw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynpftwjm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2ttekfubf.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2trthdkqg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2uwdqpchj.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2fbjcfeda.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2bcqvcxvn.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vxrzvwmx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vyqllfyn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxnaqnza.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2blkgslhm.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vpcleyxo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2ujqtexpi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2xmgepqes.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2bpcvkfzz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2pgxfhecn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2duqgxwfp.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2dvgrxrfi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2awkwapzz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2lgritsun.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2eppnbovp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2blcoszdr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eaqxicjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jmpoeqiz.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2cxjddveo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkmpxakn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2lnfwynfs.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ynjqdwiu.html


<!-- 参考信息 -->