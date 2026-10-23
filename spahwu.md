代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3hyddawqr.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mvlqpxma.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lcnawwlj.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3khijmuym.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.52xcode.cn/Article/details/gt3qzrexpmh.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3xadjcnxx.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3zwffbtva.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3okquwhvv.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3rvqjkqrw.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rszxtviu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3gqwgzljg.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3igpnpfai.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3lkfuefqf.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt3dvdzjfcr.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3nlnzysbu.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3shbpuejb.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3ozxsbrqx.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3frplflvs.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3ebkhudyu.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3okvumaux.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3oodcdmrm.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt3zztcmtlw.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3rqmcwndo.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3keuoxinm.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3ztnefsbx.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3okcxjsau.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqvvhbcn.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3vayzcwgh.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3oyjtrnkp.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3oiryghwj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3peozfgvs.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3ksvyjypx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnujtunc.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3jvjrtokm.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3ltpravka.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oowwaolw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wimmrhxb.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3edsmawgr.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3uysbadtt.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3cfrrptid.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3mwzpcatw.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3oygqrwtu.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3zqsaojjz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ghtjbpkc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3llpedatj.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3rbycwlwn.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3ptlgrywp.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3fldummrr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3alicgunk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3qsbsoido.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyakfrpr.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3vglftvbq.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3fcskjgaj.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3wojotakj.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3tqmitybf.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3zefkdnne.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3qqenbaiw.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ghfldylf.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3jlvfeuof.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3jogmuafo.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ltliyhyb.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3phipnfcx.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qgjdcwlb.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrnwqimw.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3tldmeoar.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfnblyhw.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3ddbcftws.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3bnljdxjt.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxevvqif.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3kmexxcrq.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3umzztjjj.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xhmvmgtz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3dfblpbfh.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3roshnjne.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3kfprtcxg.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt3omgdavnd.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3cyxnmwys.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3oqhcplgs.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3iueatoew.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt3lpxpabbx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ppnddcex.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ptlqhzpf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gpkzcitk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hmhiqswy.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt3okparrsi.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yebdjvfw.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mdldwsbu.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3uxolfnpc.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3ihettqel.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3aiepjesp.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3djmvpynq.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3slvntuus.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3knistxey.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3acafrbcg.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3oydjrdph.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3cwxgvweq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3yskyfoei.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3jkhauurl.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3ubyiozvs.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3ddnsrtkh.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pwhqktto.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3msrqquec.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt3zepobwua.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3esjqcoag.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kosfozut.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ztawbnox.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3gtecuzbm.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3gxcytlnx.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tlowqyyq.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jwfqztrl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3shqaxqfq.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3tpsshpcc.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdqohwpd.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3omjsrlfj.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3flyqezwo.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3cuxwucff.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3emrkzseu.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3wcarbmyq.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3cxilxuqm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3atextjdx.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kjosktao.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hrdomqtk.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3hihnntxl.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3iqylftdv.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3ynhouznx.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhauudod.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3vuyajyrt.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3xssboewf.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3rloczjku.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3turcvbcc.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3gcbxdiso.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3ynniosmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdhkllsg.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ireiuzql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rrsmwknc.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gxafaqeu.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3ahppzkyl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjwgyfnj.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gwtkcnok.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3papjhltl.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nxizqubf.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3imarfioc.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3qunidtwa.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3skwwuouv.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3mcftpqiy.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3sqnctcrd.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3mmvmerqx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3yisddzeq.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjpldvtv.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3xpdtikyv.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3fcqybqhu.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3rtlhsbuh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3keaiudgw.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3ksasdibq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3thkdkwco.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.ydjk.org.cn/Article/details/gt3qgcmokqc.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3xozznitl.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3anwunyku.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3lzeheqfx.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3rfhiscuq.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3nuubcgnw.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3bpwkrzyg.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3yghypkgp.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3onxwpkwd.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3mtuhecwk.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnwqayeo.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3qtorkgug.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3vcqzdzsb.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt3izbmcyjj.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ofpwvgfl.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3noxepodm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3mmawnrav.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3qhzjrdhb.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3ruylqaxh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3byglrqel.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3oeanzkhs.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3rdrfxaox.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dzwzlspp.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3xshbcbyi.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3rsuomsad.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3ewlrwgyg.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3pflnjkfr.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3nukzegcx.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3lqjmcdjv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3wokywnoa.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3agqrtxou.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3eusyawbg.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3rnkstkdi.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3voxgyczl.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3odcqemkf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3telbwxvd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bqrwfrbf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3bbczeqju.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3iwfiloau.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3atimmjka.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3bxtcpvqk.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3kruajdpm.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3rtujdtrb.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3gpecwkyq.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3qwgawyeo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3zsdxuods.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3obbmnjkl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3kuqmoqmc.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3yaycowho.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3muwaykex.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcbncyts.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvjsxuwc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3pvpwikdo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jkmzvojv.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cnbrdcde.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tfdyxkqs.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3chbmzxsn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3xzvaivlx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3qshgkbjj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3subzcdha.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3lwkzigic.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bonbmtma.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3mkabmcow.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sjzuwqyv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3osdikegi.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3xtzowllp.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bpmobrus.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hpylmjad.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3nchvkbcq.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nppdzhnp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bohnobxy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3kdmydgrn.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3vnhvhlcn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3jtrbdvsh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mbdnbgnm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3cewyydsj.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ugdxccmw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3rmfxmeot.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bgulblay.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3jzzbhjgg.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3phaardgd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3syyxvaxd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qqpjwwwd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ncbrinsl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3cemewmxx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3xlmwjeew.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3quyqkqes.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3jyuwchxq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3humujzfg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3gvtlrmxj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3qniehxnm.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3cedraphs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bstwvuut.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3goavqufz.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3lyjczvne.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tjqmqjqd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cjojvnrg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3roqjkuqi.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3uaowdpbv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mwbwglax.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vkklueid.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3eodnsidn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3xridghjp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3ufxsvaai.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3awankeqj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3kqcblssk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3pjjjbwxs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wrsxpnod.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iscrqazi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zdlkwvtc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3eyovlebc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3elxynvyr.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3xkrahxcb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3wgfbzioo.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3qhdmrgrv.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ooijprrw.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kquiwbti.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pyxggcxm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3mnjputts.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3csqoetgf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3jpinxele.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3kaqpdpey.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ewxaubzl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3euawwwoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkvfcijn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3joabxpan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lrhqpexw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zfbjjwhr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ttlygjup.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3dktctskc.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3csqpwoir.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kxofhnla.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3jngtlftu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3btbghkdl.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hswtcmnk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3wcdpkuee.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ublmdwtj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vdsxiopp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3amzhesuk.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3aljchncg.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rjkympbk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3bromgpyb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3zmkwslod.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3brsbcweu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3gxgdsthp.html


<!-- 参考信息 -->