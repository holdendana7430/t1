代发 wailian999

C#:   var r = x > 0 ? "正" : "非正";
来源：http://www.52xcode.cn/Article/details/gt3lugyifqw.html

[B02] 多分支 else if / elif
来源：http://www.52xcode.cn/Article/details/gt3egarpepi.html

Py:   s = "正" if x > 0 else ("负" if x < 0 else "零")
来源：http://www.52xcode.cn/Article/details/gt3sgazywol.html

PHP:  if ($x > 0) { $s = "正"; } elseif ($x < 0) { $s = "负"; } else { $s = "零"; }
来源：http://www.52xcode.cn/Article/details/gt3modharru.html

JS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mkcglxwk.html

TS:   x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.52xcode.cn/Article/details/gt3ftxcfdrt.html

Java: x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3mmbatdzf.html

Go:   if x > 0 { s = "正" } else if x < 0 { s = "负" } else { s = "零" }
来源：http://www.ydjk.org.cn/Article/details/gt3qwrpkdft.html

Ruby: s = if x > 0 then "正" elsif x < 0 then "负" else "零" end
来源：http://www.ydjk.org.cn/Article/details/gt3xdmahzjn.html

C#:   var s = x > 0 ? "正" : x < 0 ? "负" : "零";
来源：http://www.ydjk.org.cn/Article/details/gt3menprwgd.html

[B03] switch / match / case
来源：http://www.ydjk.org.cn/Article/details/gt3romcnpvd.html

Py:   {"a": 1, "b": 2}.get(key, 0)         # 3.10+ 也可用 match
来源：http://www.ydjk.org.cn/Article/details/gt3fuxtfjna.html

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3tqbunmdn.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjbruwvw.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3frjahdmd.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt3ztezmywa.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.52xcode.cn/Article/details/gt3hnfhgvex.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.ydjk.org.cn/Article/details/gt3hwahojor.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.ydjk.org.cn/Article/details/gt3csjgxqtr.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3whpfxezs.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt3dygrvsqr.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt3vogdjcsh.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3brsooqeb.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt3tjpcymcl.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt3tuwhftuo.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt3mwraveco.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt3yyfsnzse.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt3gztioamb.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xpecvawg.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3kdtbzqvu.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3mhdmhbwo.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3wjepbtnx.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3iyqetoab.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3ttxhqoli.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3vihpmbfl.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3amnstubw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3iflttvds.html

[B06] 遍历字典 / 对象
来源：http://www.52xcode.cn/Article/details/gt3moibpxdi.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3szocifpn.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lltbygbe.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3yyecphjj.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt3qkjqlowg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3gthqrdko.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3ddlxcdyq.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3ashslxpj.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt3zpbxulex.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3nmbkbatc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3wqhskdiq.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3dujbdekd.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3lewbsztu.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3tugkkqag.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3vipvzexg.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3wdrbbvoz.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt3iyydlvvj.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fxcmghez.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3xfaxoxsy.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt3euvvfzfp.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3jvdiehwy.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fcrjokhi.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3kjgxmytw.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3zjgtpxwj.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3yckdabip.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3iqjmuuvk.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3oomsnaav.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt3cfsexvaw.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3cimhnvpp.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3zimxkjqj.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fldptmjn.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3aujibeec.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3fmmbzcvk.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3vyssluok.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3qlomhwjr.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3nupousxo.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3oduqwjqd.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3jcisrrhm.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqryfnmw.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3xrsmxhji.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3bjxbhedt.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3urqqqote.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3qtucrhov.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3wvwarukl.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt3dljivyjz.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3ehxqynrj.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3lnnhusrf.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3ryrzlyow.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pqiqkfjc.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jnqkkghz.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3lksvhsno.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3laqgblri.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3ztispnai.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3wskjobcw.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ycjptypn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3bcrggxqq.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3ovhzdpoi.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3rjyywvjd.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3lqeimwci.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cbywlzab.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3ecxhfngk.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3gqbpkexi.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3xjziyhjk.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ttwunvsx.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt3duhwgogt.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3gehsfyap.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wuwrokei.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nwfmentx.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3khzkiukl.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3wgnhgzdu.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3zggcxspe.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3whvnokmr.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3clsoxiac.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3rvuceuzq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3hcpicnqc.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3byhwqliu.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sirwwngk.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uerudwrg.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nemjfztm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkqpjzft.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ovzxboap.html

[B15] 布尔运算与取反
来源：http://www.ydjk.org.cn/Article/details/gt3tbexafid.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt3isamsetc.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3klnrsfev.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3hozcbquy.html

TS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3firgckfh.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sgkojnra.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3faikohne.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3btcafuqt.html

C#:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3zqlelokr.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3jxviowbt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3tjqbcpfh.html

PHP:  if (!$data) { return; }
来源：http://www.52xcode.cn/Article/details/gt3wsntwowb.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3krdfxozu.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3uwmzluem.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3wjsktwlf.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3kauwmkou.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt3krlvmirf.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3zuyviaco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brphxdyf.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3suvnupkj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mexbjpwl.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3kgfqtgge.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3fzmsalbe.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3arspqgia.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hqrqdgfp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qhcfubiy.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3voyttagt.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3prpfgrzn.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3kkddrbmr.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qutiviom.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3wxyukrib.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt3hdnmrpiu.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdqqgwnk.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtmgzbdd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibxiezhg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt3sdayvdpu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3hwgkqzef.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt3dszdjdwj.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3tcsmprfq.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt3oyecwuim.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3uycsgqkt.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3nsibqnmn.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3jlehyyos.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nudszccl.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3vplbmsgv.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3ijpucffi.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3txwnbzqf.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3ryqvlzdi.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt3owlgpyyx.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3zzwdxsxi.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3xdjpsyew.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3oqjadduu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3welqponi.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt3oekjzvss.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3etomkdpc.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3vyrbunqs.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3ewnomwky.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3ottktfty.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ofxdpdti.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt3lpygktjc.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3okobqpef.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3eoaeklmr.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3iejsovqe.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3unqqowdl.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3neogpeye.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3fdvgpfdm.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt3qplqacgo.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3dhvrbuym.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3kdasxfge.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3ssdzvrts.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3kkrflett.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3nooidvam.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3kvcavudq.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jffztabo.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3vbfeltyd.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3mcymjoab.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3tymmzbwd.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fyykwjby.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3xthsagkm.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3fozjicod.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cgjbpnmo.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3baduvoil.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3zsmcxhiq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3jnbtkxhf.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3qtvwsogl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3xghrhobo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3piecrwla.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgntxofo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3gfrxearf.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3slhspnnf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qtwpqhrd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ojnckffk.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3obtmwiez.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3yokouufn.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3awqixgyc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3brocazxf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3clmkkyeb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tayyewgd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ktwmelzh.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3szrpprfc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ehujkdsc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3rpnrwpxs.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3koaqkhav.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3jovfnmsd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3cesegryu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3qwsorhcy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mmwhzfll.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zfzifcpf.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3crszmzhr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3xyvtfpln.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zbbrrvei.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3mihbogng.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3wojcfpcd.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3xvspapvk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3ctzazawp.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3onkmkgcb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3bqhneqnv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3vabviegl.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3flkfdbty.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3sttdmsmg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3lbdqtoys.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ivemwgyi.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3csaynyog.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3sreegvvu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wbajevzm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3iaxcalnz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3tnjvdgyg.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3whercbxz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntvqzplb.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3baysvpya.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3zrmillny.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdyywwqq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3fiumgacn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kdevfvih.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tuiozcox.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3awpthuxo.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mrrkinol.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qslycahg.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3sttzrovf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3pchpcutk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lcopvkmx.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3rebxrtej.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ggzyouhk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3tjylujat.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3isvegtww.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iycrdxel.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3udpgrxuc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3jmmmfvrp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3oiqosxbt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ftwjwnaw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zdrrlvmk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3lcsuwtgt.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rgsghwyx.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kvfumwbg.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3nfucffvd.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3fnzvlnui.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fxpjjzsk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3hkrsowxb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3vacnuzvi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3vnecoeqx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3lmehdvch.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ozgraiop.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3isdbftpp.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cwrdlfnu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lioujhne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smkxxqho.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ulysrdjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uizhmuqz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3obamevda.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ulfybhhj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3epqpezkb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wggwsjtf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3ulqzsvtl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3dhuevopw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3jkzovjjn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3eszhgkxy.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jnilogog.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3nvswgxyc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3wosrlvdq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3azyeefte.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xuhyzhlq.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3vggdylcg.html


<!-- 参考信息 -->