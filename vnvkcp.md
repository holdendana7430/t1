代发 wailian999

Java: for (int i = 0; i < 10; i++) { System.out.println(i); }
来源：http://www.52xcode.cn/Article/details/gt2inshoafe.html

Go:   for i := 0; i < 10; i++ { fmt.Println(i) }
来源：http://www.ydjk.org.cn/Article/details/gt2arphvknk.html

Ruby: 10.times { |i| puts i }
来源：http://www.52xcode.cn/Article/details/gt2orxmeymd.html

C#:   for (int i = 0; i < 10; i++) { Console.WriteLine(i); }
来源：http://www.ydjk.org.cn/Article/details/gt2uhjieihv.html

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2gvbgsbjp.html

Py:   for item in arr: print(item)
来源：http://www.52xcode.cn/Article/details/gt2djqwprxl.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt2vkjsrpcz.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt2xllxbyvl.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2kfzwcpsl.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhightqm.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt2xaedhand.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt2fzllentw.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt2atlkaooc.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt2qcsncxnh.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt2usnwpvoa.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.52xcode.cn/Article/details/gt2wzrzfexw.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt2gaxqzrnw.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.52xcode.cn/Article/details/gt2pakiajyx.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt2obahjapg.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt2ilpwomqi.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt2qyxjvmri.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.52xcode.cn/Article/details/gt2nxkdwaqe.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt2jrxqgtzz.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gprxjmlk.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt2phnrokvb.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2whohzbhj.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt2psswevdi.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2xceuxpsz.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt2gamvmvur.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt2scxyfhxd.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt2eelhzrty.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt2kvstugys.html

Py:   # 无 do-while：用 while True + break
来源：http://www.ydjk.org.cn/Article/details/gt2vrdgclfl.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nykvsjug.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2nogvysny.html

TS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2cstgzpdl.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt2ekasgejp.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2zsolwslo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt2fulbvpgy.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt2sbhmubgm.html

[B09] break 与 continue
来源：http://www.ydjk.org.cn/Article/details/gt2ewtackwp.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt2wsjcodfo.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbunzuna.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2dlbsigvj.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqqynzqo.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt2oinfaaro.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt2pcjuffjj.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.52xcode.cn/Article/details/gt2ikebwdne.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpnxmobc.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt2hoqrcvau.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.ydjk.org.cn/Article/details/gt2wlfbweig.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.ydjk.org.cn/Article/details/gt2irwzbgtt.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt2kfapdfbq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt2yewgofar.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt2tiosgvuo.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.ydjk.org.cn/Article/details/gt2rrsqlrns.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt2syyylhgh.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt2gyxarfto.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt2iuntnuda.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt2wxpkyyou.html

PHP:  range(0, 10, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yzunmqee.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ofwzvbip.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt2bzuclghr.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt2uskiykzn.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.ydjk.org.cn/Article/details/gt2seirhbbo.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt2skssiegp.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt2sgujvogq.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt2axlxqerh.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt2hkzxmrya.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt2brknrmxm.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ddglufgn.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt2mhrdjjxx.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tuwjcxgk.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt2owqbgdvb.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt2qhrqydai.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt2gfiworiz.html

[B13] 判断是否为数字
来源：http://www.52xcode.cn/Article/details/gt2hvrtvkur.html

Py:   isinstance(x, (int, float))
来源：http://www.52xcode.cn/Article/details/gt2qewtbmdd.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt2wzyvhiuo.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bmmomrya.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt2sfzygeux.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt2jufwvmqo.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt2tkukjrpu.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt2xrqwljfp.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt2nntebshh.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt2gyvhksiv.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.52xcode.cn/Article/details/gt2wtlqxtuq.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt2zwylpxew.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2seagscag.html

TS:   [1, 2, 3].includes(x)
来源：http://www.52xcode.cn/Article/details/gt2cnzlnkuf.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tjrqfwqn.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt2wodxbmic.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt2zirlnvsa.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zwcreoyo.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt2bhjaygmb.html

Py:   a and b or not c
来源：http://www.ydjk.org.cn/Article/details/gt2szokxufk.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt2veneqafs.html

JS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2mqjgkxqu.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2gscuadcr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2ybkbpxfr.html

Go:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt2oatphouk.html

Ruby: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2rwxnwliv.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt2aobjdvjv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt2gtdgjtbt.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt2dxlclzxp.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpkedabt.html

JS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2cjrgsvoe.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt2vbtwpphg.html

Java: if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2rympsmim.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt2fyttsysr.html

Ruby: return if data.nil?
来源：http://www.ydjk.org.cn/Article/details/gt2wqphglbx.html

C#:   if (data == null) return;
来源：http://www.ydjk.org.cn/Article/details/gt2uhvkkhif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uoldektf.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt2cnomfppy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dxlishna.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2otainirr.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ulfphmgn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jmiwddlg.html

JS:   function add(a, b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdnohshi.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zcihchlo.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qnpmcjuw.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt2vxyxdyqr.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt2cxdabbmp.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2oxnmvwdh.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hiezkkdf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt2vwdeehum.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jojhaxzx.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vpitoyvp.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt2swbbfdlo.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.52xcode.cn/Article/details/gt2tsxaauby.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt2ytoadvov.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt2kzemwxjn.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt2yxuernfa.html

[C03] 可变参数
来源：http://www.52xcode.cn/Article/details/gt2bywrmooq.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt2vnppizto.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt2pelcjuun.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfteqfym.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.ydjk.org.cn/Article/details/gt2axyybsni.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt2arczlqdi.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.ydjk.org.cn/Article/details/gt2esoqrgzs.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt2qnbbjjwv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.52xcode.cn/Article/details/gt2fwjucmhb.html

[C04] 命名参数 / 关键字参数
来源：http://www.52xcode.cn/Article/details/gt2rjglnabn.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt2atdfnute.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt2alyursao.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xndklhnc.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt2moutankh.html

Java: // 无：用 Builder 模式或 record
来源：http://www.ydjk.org.cn/Article/details/gt2iddilxbt.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt2jygkmrca.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yscidriq.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wuttsnpc.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt2dfavdjiu.html

Py:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2wgzjphkb.html

PHP:  return [$a, $b];
来源：http://www.ydjk.org.cn/Article/details/gt2jehgohkq.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2pvrmgbth.html

TS:   return { a, b };
来源：http://www.52xcode.cn/Article/details/gt2loxifwgt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt2viodxyrx.html

Go:   return a, b
来源：http://www.ydjk.org.cn/Article/details/gt2jgalilkn.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt2csihwthc.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt2mzypowlf.html

[C06] 匿名函数 / lambda
来源：http://www.52xcode.cn/Article/details/gt2uyqfurui.html

Py:   square = lambda x: x * x
来源：http://www.52xcode.cn/Article/details/gt2vjvbzhtx.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt2juqexsfj.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2kbdreadj.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt2xwgbqniw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2thbzihcf.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt2xmxfvqur.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt2zpclgsos.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt2fbpvfvdp.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt2znpawbjj.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt2noosfpfu.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rwjmyhwu.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.ydjk.org.cn/Article/details/gt2lntzneoa.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt2znsysyrq.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cpacryjc.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt2tnjjojwp.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt2opkzcbvt.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2lavhtwky.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2gzrowbfo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2tcszxrab.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2hraanzay.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekcclsdj.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2jrsvjkme.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2cprykzhn.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2liyvwghg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2nidsjnli.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2krmfkozp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2iwznwini.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2mpvhjtwh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2hywyyqkb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2mgjsoygu.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2oyfchlkf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2uvgiwjua.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvvxgcib.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2uwhkiiud.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2kieagecx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ypiqewla.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2pbiomnha.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2ibmthmnu.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt2bliycyzm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2hqijorwk.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2samqzkbc.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mciszhhj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2unordvtz.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ypzflhij.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2nrnigduo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2ytlmxfue.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2foykucxz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ndirqjhm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2lowvforg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2mnfnthpc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2mtssyyba.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2bcapbykk.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2dwwvhhqk.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zohlsywu.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2iglswnsf.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2wztheocv.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2oicplugp.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mpalmbis.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2dimqxopx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2tymydmyc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2lcdbncfh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2zqmzasma.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2avwjgiod.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ppmmcfio.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2vtojrjkj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2udhebkko.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2qcjzuwzs.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzeutvgr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2jastbdbz.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2stkdturp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2vthuaxqg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2hmdtqydz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2hqcmnmpv.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2opdbvarr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2lrpjxsxo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2oagczjen.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2qusrzfud.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2hcnkhjuk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2pmdwftlm.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2escstyxs.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2gwxrvjjb.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2fudvuaxt.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2tldmokwv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2rsjknqxy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsakojoy.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2lnrnoggz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2liqyzgxt.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2tzjdobbc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2qlarbhaa.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2csmrwxnx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wfoetofb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mvxojmja.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2jibpumei.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2jiyxhfnn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ghgjwlgt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2nojvadyc.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2nifbxxqo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ijzsmktq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdgafaxg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2okcxvznr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2laeepkke.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2aznznqhb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2rmxjaypv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2baixcgol.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cvfazqjx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2gyaenyyq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2gxtfnotw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ncneelzk.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2lvfgemed.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2zldhhteq.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2bdomghnj.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2kxjvimwq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kcvyfarr.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2daensabs.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2ytfvatfk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2bkjuhauh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tjlyequq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2gfbdhehf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2mjlyhqss.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2jwwlxtnn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2ogncttao.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ufywfbky.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2amfubznk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2yctlusqy.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2sybifdob.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tbwaryiv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2tkyysekb.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2wyvanrta.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2juslpnmt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2xeojzmwz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2upouoiys.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2jeinqvhp.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2uysjslgt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2umoxqdro.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2mewzgopc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hytadbtu.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ojmcygds.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2zvrazbne.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pwaslhju.html


<!-- 参考信息 -->