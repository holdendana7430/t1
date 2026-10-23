代发 wailian999

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3lguebrlo.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3socxmkkp.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3wodtdvjh.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.52xcode.cn/Article/details/gt3xhuhorvb.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3lpadbtbt.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3gjmycodd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3mfclihsk.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.52xcode.cn/Article/details/gt3gogzwgsj.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dujcfikc.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3qdvheayu.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mynbsivo.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3elblsfxs.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jrxbsssb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3aoqjzxgn.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3ckqkwupm.html

[B04] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ihrdcwdg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3wrtsprqs.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqqhotkp.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3domxiszy.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3xekjfeov.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3ppavlmin.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3deywqaea.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3cexenuxa.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt3fejczysd.html

[B05] 遍历数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3einuqjof.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt3xqailwtj.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsqqhejs.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3srfxtdnt.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3yqjrtzqx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3zvpxvsnk.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3pglizwnp.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3pwpbwslx.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbwoyzxf.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3cxycbzun.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3uutbyaub.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3swjrshpa.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3ppkxvvfm.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3ekoszqii.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3fblmxczk.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3digqomkk.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3zwjoodzy.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3bafxshyu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3iqxbayez.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3wggevidl.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3ujhuywos.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3zbkdbvgx.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vfodfezq.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzanbjzt.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.52xcode.cn/Article/details/gt3txstsskk.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3xbhxupql.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbmvryhv.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt3sdpoprhv.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3kajkptvu.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3ueqezzao.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3xrkxpwna.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3gaqzvdlk.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kzalagyj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hdwfioig.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3odzodqal.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3yinegczb.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3hxwmzvpd.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3ztgfdpxv.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlkukkqr.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3uwfxeowm.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3diqiujdm.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3adoqqxsf.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3enrkloaf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3whponoth.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycvqxiyd.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt3eopexxkh.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3slhuohng.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3aosamdyh.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3qrorfcnf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3tiiopdrr.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsciiniv.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3kbinceit.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3lbguazao.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3goynxipi.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3uuuofiwf.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lzekfbbk.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pxgzxhoa.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3oactizln.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3yinzbkdk.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3qrpwpmfz.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3mexjioxi.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3tcyatoxb.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lzbuejkq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3mbjutoah.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3oyrnqcrj.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3vqzikgqj.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3guzmifqj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3ecvcujhe.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lnkfvvlg.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3jekmakcf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3mvosndpl.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3kqrjnpvw.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt3bwhdivgr.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3oksmggnt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3cumikpcx.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yufhczmk.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jdobcvdr.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3exkypyqo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dnbuakzy.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3hyoqosug.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3kueuhgbn.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3duegxfra.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt3dakdltjb.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt3ybdrddwt.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uvawebec.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fikpthzf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3afxnyvrt.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3efijnhdb.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3blaldeif.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3isedthcp.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3ehyknhdi.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3dakndivq.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3tcfddsnd.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hsarvkej.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3kyikbmxz.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3rnjgnsco.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3nzfapsbf.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3mmexeoph.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3uaaokwlk.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3uvlurgby.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3edweconz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3flbpcvey.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3qncoqqnw.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3kdlguilm.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3lwhwqqmw.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3wzcxbevu.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3kcimmanp.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt3jdqgxqxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kcexouqq.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3gxtptonk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sdykvkfx.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cwkapnlc.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3zqrdeabq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3huzgrjan.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtpkftux.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbkzgerb.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxngqaka.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xbmkiesi.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3ijmejkss.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nvjwfzpq.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3nhowjxgm.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3nudphzfx.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt3vwsfifsa.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsrpryga.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3natkerhh.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3eukylxaf.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3jzmxohjc.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kyjksmmh.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt3sdidmwmt.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3chblisaq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3thxigolu.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hfcwhwzh.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3kugxrrxq.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt3fwlkhoaq.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xrvptbsv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt3bpdtribd.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3oztgcptc.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt3hcfatjca.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3hhkyzthw.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3wluszpbc.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt3meiuczzp.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3njynwcbs.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3baryfwev.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3eqvnrrcp.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3wrvyacrm.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wdauozjx.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aphjuzfu.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ehjbzyev.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3ealssolr.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3sznsfefb.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ufdmyygy.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3hiwerdon.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3uniwrlpk.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3oqtrfqke.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3dfszgwim.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3alnublwi.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3jyqjofbj.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt3jwlksdtg.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt3vvkapxed.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3nvyuagbu.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3rioxzpdh.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3xkhlqbil.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3vtgpgeug.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3hxrnoltz.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3yixvkqig.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3jzhlmlda.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3zlnboizj.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bkhjskyr.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3kjmwcffd.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3mapbovqo.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt3qmhnzknh.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3sidlzxxa.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3gfrvhirj.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3ulagbfjr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3ljjcrdfd.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3mlepbhaj.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylteyjwp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xzptcrwd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3jrlwbkca.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3gedcizsz.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3opxxlfrl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3aqehslmi.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dzucznra.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ucxjcsmu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wrvejdjc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zaxgeopm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lqjspnrx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vxezacur.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhhdkbbd.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3xqrqlyme.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ekqiypmr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3umhjzlln.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3wiwlztoa.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3wsvuqlcg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3uppzytws.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3wyijlacl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rmuufrhk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eoofcmsv.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3simixjvd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3kcvcadaf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dnliagzq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zvneoiqb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ftiyvzfm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3munmdbpn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hhacrssc.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3thynfzun.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3tfgyvqxv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3fenlhdsf.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3pwbupcvs.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3wgibaacp.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3koypmumo.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mpbcymgs.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3humulcaa.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3wzdwgoig.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bsldfmur.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rcuzjtdv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3yennirpt.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3thbyzpkk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3yxxpcnoy.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3oqrlsqrr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3lodxyovz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ezbiqqkc.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3vbtctjdi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfldyenw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3guqtkkfd.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3kafhccki.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3lyzzqqpj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3sczhlrdm.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3petuxfin.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3spkuizbf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3beozjdkf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3tvivygaz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3uqqihenk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jwjcxupe.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3tafenmac.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hlbrqpni.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3hgkhqmxx.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3gsrmuipw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3bhbgmwbo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3vettkhwj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vbhgucml.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryjxgjpn.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dmdkeykk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dmqbcptf.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3ufbjbphe.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dhoepxeg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3wryupnro.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3oidcwkhe.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bpyajzqh.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zdqmmlcf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3hjenasnr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3nypszuyr.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jfemzmrn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3jbctgdkk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3eelrhsrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iipdgyrw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3uihgervs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohnztdsr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gqsukxil.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3kivhdjxc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tzynmfvb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3eshzhovh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jltykjua.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ennagmso.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3sqrpyndk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3uazttsfl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3vqpjkter.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wfmflstm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3wvgsbfrg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zgzalskc.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yxswivzq.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mgixystk.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3njqgqgim.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fnjxwpav.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3niryxjrc.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3xwdgbtqq.html


<!-- 参考信息 -->