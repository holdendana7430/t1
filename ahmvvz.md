代发 wailian999

PHP:  switch ($x) { case 1: $r = "一"; break; default: $r = "其他"; }
来源：http://www.52xcode.cn/Article/details/gt2xllhkdrd.html

JS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckyoasfn.html

TS:   switch (x) { case 1: r = "一"; break; default: r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrwumeyk.html

Java: switch (x) { case 1 -> r = "一"; default -> r = "其他"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvibjlem.html

Go:   switch x { case 1: r = "一"; default: r = "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zrswmlpb.html

Ruby: case x when 1 then r = "一" else r = "其他" end
来源：http://www.52xcode.cn/Article/details/gt2favyabye.html

C#:   var r = x switch { 1 => "一", _ => "其他" };
来源：http://www.52xcode.cn/Article/details/gt2cpoirqcn.html

[B04] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2catcaqgg.html

Py:   for i in range(10): print(i)
来源：http://www.52xcode.cn/Article/details/gt2mgrtxvpo.html

PHP:  for ($i = 0; $i < 10; $i++) { echo $i; }
来源：http://www.ydjk.org.cn/Article/details/gt2brvrnasg.html

JS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.52xcode.cn/Article/details/gt2oaktscrg.html

TS:   for (let i = 0; i < 10; i++) { console.log(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2mekmmitm.html

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2syfohias.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.52xcode.cn/Article/details/gt2qvytybep.html

Ruby: 10.times { |i| puts i }
来源：http://www.ydjk.org.cn/Article/details/gt2bzukhxvu.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.52xcode.cn/Article/details/gt2wzqbhiia.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ttuhavps.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2tloypyws.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2umfcipxf.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvlhaean.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2rtecajhx.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt2lhknnxbj.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt2ugzubjvb.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2rbjbifra.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2ioulfuwe.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2knlkgdau.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2kwgyawbe.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmtnvfbr.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2hdxgxgtu.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2vxcrkasu.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2hnfsfqrq.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt2ewgklate.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2xechabrl.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2evuvvmyr.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt2pfqznvdj.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hkpkrblz.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2gkuwjqgp.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2bdmgsgcx.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dkzaaubz.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2qfmqsvns.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2sylwfkgv.html

Ruby: while i < 10; i += 1; end
来源：http://www.52xcode.cn/Article/details/gt2njvuomxz.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tegibfiw.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2okpyutdx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2zwtbszpz.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dzpcalwu.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2ueqpqvfl.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2jmsqpwyz.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2yibxiyvt.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2njelorpm.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2ynegezdu.html

C#:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ycyvyeeh.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt2suisozel.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2iqcsnxpo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckbfmdud.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2avxkrzis.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oiocpcuc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2bevmkzvp.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2tfwxxhwx.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2eombodaj.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2wvfshjye.html

[B10] 遍历同时拿索引
来源：http://www.ydjk.org.cn/Article/details/gt2yrlaorvm.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2vozwdvai.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2fwhkbtjp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2gcrdcrtb.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2ayjrqgxn.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2qptkjdeq.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2evowahmv.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt2kvbnqyet.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2jthmuvzq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2ssetasyv.html

Py:   list(range(0, 10, 2))
来源：http://www.ydjk.org.cn/Article/details/gt2cicbssub.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2exwcfyss.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uavasdww.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sgcqrxhn.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hhpglthc.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2dvbtylcl.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2aafyklye.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2npcmxmis.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2juuqjvha.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2fwkeepxy.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt2cufudyzx.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2uvvctumo.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hhyvejnc.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2fxgmojgx.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2vcmkkajf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2heeriapg.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt2ttsdojkq.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2vaqlrbbw.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2ruyzwogm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2xjlvpqyg.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2kxldmqoi.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2jpmyhuiv.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt2lmckxmxn.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2cdjrdbay.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2sctadznr.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2qndnniop.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2cffihbbt.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2wjctzjen.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.ydjk.org.cn/Article/details/gt2neynboif.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2naltzzsi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zkgkvthl.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2exboaccj.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2jmcwxjth.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yyedzdqm.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2avqufdbw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2nzdpzquf.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2osiofzob.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt2duvzolzg.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2qwjhbobd.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2hkvsbbvm.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2wmvjflmj.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gwmlbcma.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ddxyibaa.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2audnstqq.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2lsyfusku.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2sqzrswmz.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaexhxfm.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2hhatesiq.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2ykmliczx.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2zoxeuisv.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2iboslvcb.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2kxfxrdis.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2lrrstuqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2geyoughc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2zerbcqnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yfbhqbcs.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2eutikubw.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2cchxolrx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2oxewytxz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqrsjdtb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2lllviuwa.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2plpibfmo.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2mmbsozje.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2lmuuupcj.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkjwwfur.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2akctqkla.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2lnysmqex.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bldilyhw.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2bmpweykd.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xanhghqx.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2sudyjkwc.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2ozozkifa.html

Ruby: def greet(name = "World") = name
来源：http://www.ydjk.org.cn/Article/details/gt2emrqwaku.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2mmelysrm.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2rdtwmlty.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2kutmyvyc.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2kgxtrjns.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2hpjxhuhc.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nedrwqrb.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2tkvcvqac.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2ztabeznh.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2ptxbbocb.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2breuamnn.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2rgzisswn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2encvqkpg.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.52xcode.cn/Article/details/gt2imsirvrz.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tfhkfkjx.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2elnwolkc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2qayppshi.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2oylwxyug.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kexslbvp.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sxfcbbon.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2nyljkehy.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2chxdbotj.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt2deebimjh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2oojwkcsr.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt2bmeseats.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2erumhjjx.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt2cgpikada.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2yblccvib.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2yiihxasu.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2niibuqee.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2raaomcvz.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.52xcode.cn/Article/details/gt2ajnmnoux.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2exmqnmkv.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2bcaqczjy.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2aczxtgyj.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2ddedvvoh.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt2wpgtviro.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2aduywuyw.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2abdssucw.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt2qzcnjsbf.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2qippwrxf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2cuefemzx.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2tkuuhuwg.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.52xcode.cn/Article/details/gt2heebuibz.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tbbxtufw.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2usljimmt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt2rxaqcvor.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2kcojvcnu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2kkksfxdo.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt2kfgclleg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2udvqrdsl.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyynbrxb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2dkpxovlc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2ouzuclfv.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2elgyuvuf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2jasieizg.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kaqcmmur.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2eeocnvwq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2dhkmruki.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2kwgbcvzd.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ixadvlvg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2qkswpiyn.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2grzzielh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pyjpwsqh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ixpniday.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2ozuythrz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2rjtflimf.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2cacpnuio.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2euypzujc.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pqeugnoo.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2srkqlamq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ogcgmzrq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2ahqyreeg.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2eguicgwx.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2ufbvsgww.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2cicdxyfr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2nbngwxyy.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2lvejzimr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2yhhbwpzn.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2igqaxxfb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2ervcphhk.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2bqbxwuiq.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2mrdcndwk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2efebpnma.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2hnvseilx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mhqmnsvz.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2wbkbjxxj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sdevwals.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2imhgqsrn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ajetgvqo.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2opkjoqon.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2odgarnay.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2pgaounhn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2eydxxomx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivhabqii.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2mcrdzhfp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2rswxpqdc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hcsmhyrw.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2pbggzjxj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2zkhxypag.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jobwhstj.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2mltkffzq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2urfhypff.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2cqldnpsb.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2jeprveni.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2daxsbptn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2fqhwhphf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2vpwfezkx.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2dkzpeixx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2jwleaqqr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2usophxvv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2mjvzsgqk.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qasyyqsx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azlmpzhp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qqqgrqpc.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2jdlzdxga.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2qyqqrfgo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2nkjderxp.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2lvhviuts.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2uukcdsue.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2soxrzgog.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2fbggpnwz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jvjzqoyf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vitudvup.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqrinmvm.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2xfzjwhpd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2isbepwqc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2acyjymee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtabmpew.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gixtbvud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crpunwni.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2jogrvufz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2kgievwnt.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ietaopiw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2lrgdcffb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gyyikwus.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2jgcawjck.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2abwbvazv.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2emeavdgk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2kuqqyglt.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2jvyzyzlg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2bttftsua.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2cvywacmw.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2oqalswie.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2zhzexztm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cddirala.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ovyhfqen.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2oxotzktl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2rjphgouj.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2abttlfgv.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2bkyrovzg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2ktwtqizk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2spcayghv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2nthzircj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vtafywtv.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tqgzzwjm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2hrrjjdfv.html


<!-- 参考信息 -->