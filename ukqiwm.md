代发 wailian999

[B05] 遍历数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3aijjiyet.html

Py:   for item in arr: print(item)
来源：http://www.ydjk.org.cn/Article/details/gt3arkqzrdx.html

PHP:  foreach ($arr as $item) { echo $item; }
来源：http://www.52xcode.cn/Article/details/gt3ixwkgiod.html

JS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3jpuvwpcs.html

TS:   for (const item of arr) { console.log(item); }
来源：http://www.52xcode.cn/Article/details/gt3zwfgmyvg.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3loqsxwqz.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.52xcode.cn/Article/details/gt3fvirhnyr.html

Ruby: arr.each { |item| puts item }
来源：http://www.52xcode.cn/Article/details/gt3npoggrrz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.52xcode.cn/Article/details/gt3knkgcynr.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3pavwfemf.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.52xcode.cn/Article/details/gt3kxcadonw.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikllztfh.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3eyavuxye.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3mjjunlev.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.52xcode.cn/Article/details/gt3oorgjdjb.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.ydjk.org.cn/Article/details/gt3zzkdbjgl.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.ydjk.org.cn/Article/details/gt3nnjmaqlo.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ieoqhnyp.html

[B07] while 循环
来源：http://www.ydjk.org.cn/Article/details/gt3kgttpzxc.html

Py:   while i < 10: i += 1
来源：http://www.52xcode.cn/Article/details/gt3agzbjlww.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3jvvfeoey.html

JS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3uvfqttxl.html

TS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3cnkbilpy.html

Java: while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3jzgjzgyd.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3ijixnobw.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3syqifhmx.html

C#:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3kwsznydk.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3wsqgufqx.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3djvhodep.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3runqgxan.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3eqvobrio.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3sinjnogl.html

Java: do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3ocbrsdss.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3hrhjecqw.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.52xcode.cn/Article/details/gt3sdolllrq.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3fwbyxjfv.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3msfxkidh.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.52xcode.cn/Article/details/gt3uyeeoukj.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3orbyqzsp.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3olvhrfkh.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xnmqihjc.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3oxtdwpnm.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.52xcode.cn/Article/details/gt3kmfuwush.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3xzzsxhmb.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3xzqgjvch.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3kjmcguzx.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3tcsrwqeo.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3wmyekgcb.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bgptlwbf.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3ciitcicw.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxxxziqa.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3vupwwjrp.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.ydjk.org.cn/Article/details/gt3vxlhgcxn.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3pmqpfzud.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3rlwegtoi.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3utzajcqx.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3llzbsbcd.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pijutzqf.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3vgekiopx.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3fiehnhlx.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3jagnewvn.html

Ruby: (0...10).step(2).to_a
来源：http://www.52xcode.cn/Article/details/gt3xbfobffj.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3lbucoyxx.html

[B12] 跳出多层循环
来源：http://www.52xcode.cn/Article/details/gt3eygemfhm.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.ydjk.org.cn/Article/details/gt3ggsqguxf.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.52xcode.cn/Article/details/gt3nclvoxor.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3jadrmyif.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pxggpjzn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3abgaqgsy.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.52xcode.cn/Article/details/gt3fuiqgrtf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.52xcode.cn/Article/details/gt3ifzjcemm.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.52xcode.cn/Article/details/gt3rsuazqeq.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3cdosenel.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3ihcylqom.html

PHP:  is_numeric($x)
来源：http://www.52xcode.cn/Article/details/gt3mcvygyzc.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3qkpdrjgl.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.52xcode.cn/Article/details/gt3juylqiph.html

Java: x instanceof Number
来源：http://www.52xcode.cn/Article/details/gt3wxrabcsw.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3dljcqgne.html

Ruby: x.is_a?(Numeric)
来源：http://www.52xcode.cn/Article/details/gt3ibkiosfi.html

C#:   x is int or double or decimal
来源：http://www.52xcode.cn/Article/details/gt3qxwrcdzo.html

[B14] 判断值是否在集合内
来源：http://www.52xcode.cn/Article/details/gt3ymrnptjx.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3gamlootv.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3kfhckpky.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygzygqbi.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fpmliunw.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mnzepzvv.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.52xcode.cn/Article/details/gt3jyfgeecj.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3tujlkuck.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vfgtabym.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3msiyeuit.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3clmslqfl.html

PHP:  $a && $b || !$c
来源：http://www.52xcode.cn/Article/details/gt3elxecvvp.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3jextddlh.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3ekgwodku.html

Java: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lutglluw.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3wfguwpmh.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3lwcnjsas.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3uzplvzal.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3qnptfqdm.html

Py:   if not data: return
来源：http://www.52xcode.cn/Article/details/gt3wkzvputm.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3pglqrpta.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3rktfcsau.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3qahyrani.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3fpgacikg.html

Go:   if data == nil { return }
来源：http://www.ydjk.org.cn/Article/details/gt3pisaibad.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3fuylhtux.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3dybmplak.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfksomcc.html

C. 函数与作用域
来源：http://www.ydjk.org.cn/Article/details/gt3powupykh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twqduyrl.html

[C01] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gcbkfkll.html

Py:   def add(a, b): return a + b
来源：http://www.52xcode.cn/Article/details/gt3capgcazf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3untbbpgh.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3elmspdis.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3wdubejwt.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3zbjhcnsh.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3umbgaqip.html

Ruby: def add(a, b); a + b; end
来源：http://www.52xcode.cn/Article/details/gt3kfvggeyw.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nwsuhflp.html

[C02] 默认参数
来源：http://www.52xcode.cn/Article/details/gt3aqjxqwzf.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3dvsaoahq.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewdnftwb.html

JS:   function greet(name = "World") { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdfhbqni.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hiabkahs.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3qmnclhdx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.52xcode.cn/Article/details/gt3gjzndctp.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3zeofedqz.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3xohmzjcd.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3rbgcxlbx.html

Py:   def total(*args): return sum(args)
来源：http://www.ydjk.org.cn/Article/details/gt3tsirlweb.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3nitrhjhb.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3lhmphsxd.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3sjknqlvy.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.52xcode.cn/Article/details/gt3xcqjwpnj.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3bpfsktfe.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.ydjk.org.cn/Article/details/gt3myknrwkv.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3euglennf.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3nrxyfnxm.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.52xcode.cn/Article/details/gt3dbynekmo.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3lhktajeo.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mznihqep.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.52xcode.cn/Article/details/gt3pixymmyd.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3irpisese.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3zhzdqpzu.html

Ruby: f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3crlwjpde.html

C#:   f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lqlrrqon.html

[C05] 返回多个值
来源：http://www.ydjk.org.cn/Article/details/gt3qtqojrnz.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3gzthjjtu.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3goofhyzv.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3zypvoktu.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3vwxhdndt.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.ydjk.org.cn/Article/details/gt3cixsquiz.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3hejfkndf.html

Ruby: return a, b
来源：http://www.52xcode.cn/Article/details/gt3pmccmfps.html

C#:   return (a, b);              // ValueTuple
来源：http://www.52xcode.cn/Article/details/gt3tcegczyv.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3okklyzoc.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3excnrdeb.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3avvgtwpi.html

JS:   const square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3eewnznqo.html

TS:   const square = (x: number): number => x * x;
来源：http://www.52xcode.cn/Article/details/gt3uucugybm.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3bqtsyhpe.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3hmwbairt.html

Ruby: square = ->(x) { x * x }
来源：http://www.52xcode.cn/Article/details/gt3jdrcdhva.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3xylajwdf.html

[C07] 把函数作为参数传入
来源：http://www.52xcode.cn/Article/details/gt3yaoccxtp.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.ydjk.org.cn/Article/details/gt3kicoiiul.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3naqrhujn.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3yyqtwnst.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3qsazesmw.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rcruysms.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3ojlhmfro.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3strdnalq.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3zbgupugd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3rghhtyxx.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3avloohrv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3sthdjwow.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnxoddcp.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdemaupi.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3asinddsg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3vyuuzkgi.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bpqojsvn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3poljaqrr.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3bsypneiz.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ritllgvc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ozsceswf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3vovboczw.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3gxcmpqon.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xwitvpsr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mpsvalzz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hgjusrbs.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3xjpxxtui.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3nmprigob.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3fhucujvq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3xjngfsxy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jsjpqkuu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3drhiwosy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3mloezcsu.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tlpdildt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qpbhklxf.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dekhmzye.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3szqjamoo.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3bfafagan.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3usmdawml.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hipnqrba.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3edbdlxpz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3lgcrabbu.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wydjwtdz.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3sghjxexh.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gkzckvwl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3vowqsuzf.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3natgdpdw.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3hgwyofuq.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3wxjdpmrw.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sgfuqqng.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3sgxvjogi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3oijrkoow.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3jckzqfpm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vfbhsprf.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3zmhnyplb.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3qwpgjdjw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3fyegukpn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3yoedyauh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3azvejxvx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mrtzbcuv.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3fsjozuum.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3squuybqm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3unyehcpl.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3fkvtousy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hgzkxnbb.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pgcdehrj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uxifzkcu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvqocexq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3yswgxiai.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3gxkmwmak.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3evbkzpal.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3hdbqeggm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3hyynjwrs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3pdbblfhs.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3iazucjjm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3fukipclr.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3njmgzjaz.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ruluubbm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3baumaxfp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3luqjqteg.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3doumfghy.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3ruoauldq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3nuoyvqwm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3mphqgipe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vcoajgcw.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3svtwrwzw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwxrerlx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3tylmtmft.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gjsmwiuf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3rwpotsfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcfnwxnj.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3wgiomwus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nwvjnltk.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qanbmvjk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3rysqzcph.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3yyjcukuj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3thjtlnbw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3hjxmsknv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3cezoonyv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3cnmzemwf.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iyohktih.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3yqqicjwh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3zfyclfoc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3ooxxcdcv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3oeddkcck.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qgbxowdz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3byhyivuz.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vgqhzvdo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dlfpvulf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3mprpqzdz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3bxdulloc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3lholvfyb.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3innvdpnf.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3lnuwripb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3trootbvy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wnojgtos.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hjxamqmp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3fozrsjmj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3tefzzlee.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3nwkbtisd.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3fhuvqmrt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pbrfjzuy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3umiesoep.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ykgfkmfl.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ktnodsfr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zjdvjkbz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3extfjcny.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3veniuxcf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3zdqjxnqg.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3impmskoj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gomgfsdg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3crxyfyog.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wqqwmbxa.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3idhcfenq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3svketjhx.html


<!-- 参考信息 -->