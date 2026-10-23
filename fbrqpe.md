代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnhmayzw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdmuqdwl.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnffiskn.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3xreigiwc.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3alhjpsec.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3hylybwzx.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3guepuegg.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3amztkoeh.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3tzdtrhum.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3cadixzmj.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3nrsjfszl.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3mzkaxqsj.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3yjsguuie.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3ciwamjdo.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt3idinxlzm.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ecguyufq.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3vekjwsnv.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3rnvspdxs.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3cefuyiqo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrtlvflc.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oubfbzva.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulsmqydj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3irmcuimh.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3vwqpyjol.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3jjmievsd.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3vayiylzk.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ewnrhilr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmgwnoky.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3jnqzddcw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3wwvbuxvv.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3uktbtmvi.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3uszibobc.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3efujaxvc.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3cnlxvuoj.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3imdoiztd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3oieqowss.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfekgqri.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3itxqasty.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3dqveqair.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjfgamyd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3oykutvnk.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3lhrapsiw.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3hadjrlxp.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3etfzuhpu.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3kirayecr.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qvrbsxzh.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pcsfxtxi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3twrdwzmk.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3wrjjchjk.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3qfwwxjby.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3wuzuqnkh.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3hlhyuise.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3guopsuim.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ndzmhzcr.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xcyjkcdz.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3pqhyzmcb.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3wydnybwx.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbttkygw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3ejxaayzo.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt3ikpwgsig.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3amwzxdwo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3iwcxyubx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt3qwdnibdk.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgssskne.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3ztsydifx.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3emjuyxst.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3pynawtws.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3xzdxibpy.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3ysxxqeak.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3uzfncqqq.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt3mcfzsfnt.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3adgzhsod.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bkedfbcx.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3exymxbgx.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ekqtbzgp.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3chclznua.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3ghowgakt.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3nqmdgmlw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3adjsevgv.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3dofppzgw.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3mejrvkrg.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3akexovcc.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ksvgopcw.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mxlrkbnv.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3wtezeyic.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3bwgyqjgt.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3atjrsuhu.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3tqumkstp.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3wesvhwhj.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3mancmtme.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3bxtwctxw.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3sxblpvtk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bwbssdzo.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3btxztwtn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3dmqpkwcr.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3ulaweqwo.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3jlsoxxjt.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3szrqiycn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3fooeehqn.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3wtqbyskd.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qlchkzbs.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3jotquhxg.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojzalglj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3nvcytpxg.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3sugsjhpf.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fziimlvv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3sxosflix.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3zuobfenr.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3uqwbrllg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3iffwvqwa.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kxvbwxhz.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3eyxgfzfd.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3vjpivzjs.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3gcqvblpd.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3eykziywm.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3drygyhnb.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3quacpqvr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3qlyaqrwz.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3dtcaaagm.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lbppisyi.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ugatdhpy.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3jjwalmvh.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3hhxulnio.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3lchbyvsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fvowazxt.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pguwhssw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgrulxml.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3fcrjsiwn.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3vrskbmiq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wjarqzjv.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgfujbrf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qihhkaiw.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uzkuszgw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3inavusdk.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3kyeagmdm.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wuecftsv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3djllvxwi.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3xkyzerzp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3eenwwqje.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nyjeawib.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3okjzhtfl.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3orhwcaql.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3kbjleuzz.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3mhsdfqxw.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3mgdlnzfd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3cxomoajs.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3drhlcooz.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpojslcn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdhmetkd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3udtduyyw.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3ibbkhtju.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3hoibyear.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3flajjbkj.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3shwjrdll.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3rpmageet.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3rggncuzs.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3cskpwwrg.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3aksfhckl.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sgnbcdvo.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3evgpuige.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3qqaiqzub.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mrkzzwch.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzsurosk.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3kyosutsz.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3tahzcwwq.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3sgjxdtrw.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3abavnvyg.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3untikkvb.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3grtqojwm.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3sccvnfbu.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3qxinsmcz.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3rbmnheag.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3tqccthwh.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3fjelkhyg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3nnhsfjlo.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3dubrysnz.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3qawhvnqw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3kurzlmyk.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3rhthbdon.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3chthjwnb.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3fpdperrq.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3joecekqg.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3gmnxrohp.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vormnpvx.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3wisfjncy.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zvfxuazy.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nospbhkt.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3tkmuevae.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3dlxkhhqj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3ysomlxfn.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3qtbtowhj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3ipiofcyt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsetlfhl.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3czptlalr.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3cytfppct.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3swulrcsr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3gfyeupqg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3nvokfyxs.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnqkklmf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3blwqdfof.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ofvzzzgb.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3giiekleb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bmttmwzj.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3xkkaotwg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3oljyjclx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3nebiqkfv.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vammdqfw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wwgazdga.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3etzktgcl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3akeipzdh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3japcdjin.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3pefukfbe.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oepjhqaw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mavkrfyk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ygoijilc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3fzjlgmoo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3clbwphif.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3anvlzqbv.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3nrhokkpq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3atqmjadi.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3bmjgowhb.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3aowkijpl.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ejogneds.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3suxklgpb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ntkouloq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3upnrpjwz.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3emdchwut.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3yuijeaxe.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3bfydnbvc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ccrpvyss.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3gbvpifzm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pwjoruyc.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3abwjbxlp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vglbumui.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yhkbuodw.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3cxncasjx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3qaiegett.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tfdkhslg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3nqljyxig.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3mzsksixd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjocwama.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3jurgwkms.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3fbviouge.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3vvmtxmgt.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3uvtvhlyf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3jvdtfyvv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cmrkbndo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3clcxcxfc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3tghillyq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdwlkifj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3bwfciewy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3nthazvzl.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3tchucfev.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vxwghiwd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3qglyzjqf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ftocohar.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eimhmfdd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3vjnrzdry.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zfeikfsw.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zkokjgdj.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3kivvufff.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3mcwpachq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3mmxgirlb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3gdiffdgq.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3yoqplbuh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3lddwjyud.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3chnahcrx.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3shaqllzj.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3uinmsojf.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ralqzohv.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3htwanqlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3denngiba.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3rekjqqug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxfcrkpu.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fqvjeocv.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3goqjmmzo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ztyrluyu.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ocmlwcdn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3rakwyumk.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3rolqgwls.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3osofscsd.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3jrstznfs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3spdmcfsy.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3imaoeqcr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vdvmwkut.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3sxkfjceu.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pvcjxope.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kdreevxj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vkpuvucv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3epiuosxe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tpvziyix.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3faietyuh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3bdeewluu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3roleuwsm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3kvvrtgnr.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3arfulein.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vbxoxjxa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rcdyaowc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3skjhxswb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3kmkekddp.html


<!-- 参考信息 -->