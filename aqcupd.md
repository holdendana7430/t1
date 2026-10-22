代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tjtddfsl.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2ayampugl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.ydjk.org.cn/Article/details/gt2twxwmhox.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2jcjcnwkr.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2yewghvnr.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2uuspqxgy.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2hffyhmiq.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2xisvpvtw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2nlxdiefh.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2indkekib.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt2wxrfhrsr.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2dxuzwxpm.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2phcvcyhl.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhzxokap.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt2wgezdrca.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2clndyzka.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt2zemdwtcb.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqrlsvtu.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2sxbbjlnd.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt2jglougmc.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2xprxdxjo.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2cprqsflq.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ddckufpb.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2ygskfntr.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2svsvsfew.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2fqhgbxyh.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2mmpeusup.html

[B08] do-while（至少执行一次）
来源：http://www.52xcode.cn/Article/details/gt2ngomsytk.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2dnlznuqt.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2usdsvjyt.html

JS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2aknudfen.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2hsqxpanf.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2dvjeyrhu.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2sqzhmipt.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt2rqwyikmy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2fyvtikfm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2hkirliav.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt2beldkncu.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2vuuynszy.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2txbngvgu.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2pqlnmrrg.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfandrhj.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2dwmzmqiq.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt2nkscmzxc.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2jvmgrtpc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2bnjdqpii.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt2qrikgnit.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt2hznpljmz.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2zpvhpuve.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2yruzxxlg.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2mzejfyuw.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt2shzikarf.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2rxtbbgnp.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.52xcode.cn/Article/details/gt2olzgqxvn.html

[B11] 生成数字序列 / 区间
来源：http://www.52xcode.cn/Article/details/gt2wzvdtyij.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2aqcbwocq.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2czyiqdal.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2dvawqxit.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2godfgkou.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rvveyidv.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt2vgawjcxg.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt2adxbjpzr.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.ydjk.org.cn/Article/details/gt2msytloqm.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ffudfkyn.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2czhpibql.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2poaopjzw.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2phcnqahj.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2nbtatpor.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2gnhlxfgp.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt2fqviykea.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt2xzaikkdr.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2qwkgujmt.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2gdkxrrom.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt2fezynuqm.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wiavketa.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2wvwwspxg.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2xxmcmfsf.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2lygnztlo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.52xcode.cn/Article/details/gt2siqmnjmt.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt2hzvvzbjp.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt2byvnyrky.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt2iiljifhn.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt2bfjmdmmf.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2nawdsdil.html

JS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2uqyatzsr.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zpepmqjt.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cwchihte.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzgsjojm.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2jnllksec.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xhspkgvw.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2rrnkrbgv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt2qcrhzqqg.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2tnsrllzg.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2tqfmyjcx.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2prnhmuuq.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2rhcmbhmh.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ltutkekb.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2mongoxqd.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2oivxhhth.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2fpohnubn.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt2zjfnxooc.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2anvfkzsj.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2jmzktzgx.html

TS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt2dkegpvqs.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt2flmixzvt.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt2rydaxujx.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt2asmzssny.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2yoasvlfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmmwsrbo.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dwutkqjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fevcbomg.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fzrrnekd.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt2jljcddgg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vmwfqanq.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2ojzdhcnj.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lopuxtzo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dunqhpys.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2kbpslzkl.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt2uvgtqzov.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qoldajsr.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt2kwrikswk.html

Py:   def greet(name="World"): return name
来源：http://www.ydjk.org.cn/Article/details/gt2yngykwzp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.52xcode.cn/Article/details/gt2lpidmler.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvocwkzg.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdtsqgtg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2kpmertnu.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt2clhixvps.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2wnvziabo.html

C#:   string Greet(string name = "World") => name;
来源：http://www.ydjk.org.cn/Article/details/gt2qzgtyydj.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt2zfsgqopa.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2qbiiephn.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2onjvvpdg.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt2xjigtbck.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2wbfjhkyo.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkblprel.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2bvhqsejb.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt2unkninzg.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2pixhrtom.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt2zrimokql.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2ezzsdbdb.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2fxemxand.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2idqpqcdd.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2wmmeafuc.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt2nbmnhpgm.html

Go:   // 无：用配置结构体参数
来源：http://www.ydjk.org.cn/Article/details/gt2hhawexye.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2gwbxfrvq.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt2qxrvkpfm.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt2pinqzjtf.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2dugdkrlm.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2okcfmydd.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2inecdjwv.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2hdlpzoul.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt2alkauraa.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2refzsgqt.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2prefvxel.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2cqoboxoq.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt2vqpivpvj.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt2zdecchmf.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2aidhwtgq.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fadrqyvq.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2chdpxxow.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2hyfridtq.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2mewbvxta.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2tpaclhri.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt2unupntso.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt2qxbyrinm.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2vurocqma.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt2piebsjqf.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2dffpumdh.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt2betrwhmj.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cmbwugqm.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2wskumeth.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2tumycjte.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2lvpoadcr.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kiqpwqqu.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt2wdsotpav.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2tplptbux.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2lbsnwmxz.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajwfzgul.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2yrugolzx.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2lprktcoh.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2vjqnvctc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsgexcbj.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2omwpjpwk.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2erbgalph.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2mpwwerdr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2bnpydqbw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ylvfzpwd.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2mtlaaxcx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2htsfqmdr.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2guxniloj.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xsipamsi.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2eguacfdy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2eehiwdwp.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2dzckfqdf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vqlbaivx.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2vdkkvesy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2poeygsmd.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2pjnwrmyr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2cmxwnaef.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2lwffhhcp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2ivfvdgsi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2ppytqkay.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2yduxiuod.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ofpekahl.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2cztcfsxb.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2olsqydek.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2gmjgjypn.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2famqtqrs.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wzashnhl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2itzhlgdu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2zmhndmxm.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2bgvdcute.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2lwufmxxt.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2omozvyfv.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2yylwuvza.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2sxgvydox.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2etillpsa.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2amuewmit.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2fzrebnmh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2idraldsp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zvugqurz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2rhnnguew.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fcdoxvva.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlllegox.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2aliypcko.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2xqwoipmm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jdiofqcb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lclpmkac.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2ecvlfoxp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2oyyvtvue.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ievjqrpn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjyzkgbp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofbjxrmj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2lrlagjfc.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yaqfuylf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2pypspqny.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2pnrlhacp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2jvhcvgxx.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2jieknzsp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfvmgpxs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2hnfhwxam.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2kwjvmpqc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lcqgzkni.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2bwkqydgf.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vxwmhdco.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2jjemajhy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ivoivmjr.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2yzmgmjqg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2yndgspzk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2hbaomxck.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxwfjwbd.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2mxzqrsny.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2buiqhlda.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrzaqvjv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuzxxtop.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2rdkblsyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnxivsgv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2zaphimzx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ulcjdfin.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2gbxcpaql.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qworcspp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2mtnjqcmp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2ptnzdcyv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2qgrfomhe.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2vgesjrth.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2fkkhicod.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2wowdnzxs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2wirxheys.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2bukidatc.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2pvfpnokc.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2gqbunfix.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ihtkvopu.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2pqpornto.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2swufehao.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kbqpekvs.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2mbwhzlnm.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ttydbrnw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2oyceredc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2ivghdvif.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2oqefrrxq.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2svfymkcl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2wdvrroag.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2knyaxkne.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tcdwfhrq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2qpsgphhb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2exxnqjvc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2mrqwktbn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2evofooza.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2seknxsst.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2igiyoaei.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2icuwapyf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2anphsbdh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pwxiqocc.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2ajhtyugu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wayfzdin.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2embaltxj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uizmwujb.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2gbwojfts.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2rxcyfywi.html


<!-- 参考信息 -->