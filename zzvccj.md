代发 wailian999

TS:   for (const item of arr) { console.log(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgvppqme.html

Java: for (var item : arr) { System.out.println(item); }
来源：http://www.52xcode.cn/Article/details/gt3nxrylhpq.html

Go:   for _, item := range arr { fmt.Println(item) }
来源：http://www.ydjk.org.cn/Article/details/gt3xcbcczwv.html

Ruby: arr.each { |item| puts item }
来源：http://www.ydjk.org.cn/Article/details/gt3dmmbwbwz.html

C#:   foreach (var item in arr) { Console.WriteLine(item); }
来源：http://www.ydjk.org.cn/Article/details/gt3qwqpkmlz.html

[B06] 遍历字典 / 对象
来源：http://www.ydjk.org.cn/Article/details/gt3imrrygvo.html

Py:   for k, v in d.items(): print(k, v)
来源：http://www.ydjk.org.cn/Article/details/gt3gcpasvtb.html

PHP:  foreach ($d as $k => $v) { echo "$k=$v"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttbbfwhu.html

JS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3fozdbvrx.html

TS:   for (const [k, v] of Object.entries(obj)) { console.log(k, v); }
来源：http://www.ydjk.org.cn/Article/details/gt3wgsrvnwg.html

Java: for (var e : map.entrySet()) { System.out.println(e.getKey() + "=" + e.getValue()); }
来源：http://www.ydjk.org.cn/Article/details/gt3rsrflved.html

Go:   for k, v := range m { fmt.Println(k, v) }
来源：http://www.52xcode.cn/Article/details/gt3yawabhcm.html

Ruby: d.each { |k, v| puts "#{k}=#{v}" }
来源：http://www.52xcode.cn/Article/details/gt3gdsdlmnu.html

C#:   foreach (var (k, v) in dict) { Console.WriteLine($"{k}={v}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysyqrmbi.html

[B07] while 循环
来源：http://www.52xcode.cn/Article/details/gt3oapajmcf.html

Py:   while i < 10: i += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ibbpivav.html

PHP:  while ($i < 10) { $i++; }
来源：http://www.52xcode.cn/Article/details/gt3oqimrzly.html

JS:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjxzwpcl.html

TS:   while (i < 10) { i++; }
来源：http://www.52xcode.cn/Article/details/gt3yetsmqif.html

Java: while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3tuzwqmch.html

Go:   for i < 10 { i++ }              # Go 没有 while，用单条件 for
来源：http://www.ydjk.org.cn/Article/details/gt3uqzftqzy.html

Ruby: while i < 10; i += 1; end
来源：http://www.ydjk.org.cn/Article/details/gt3yjqvtkup.html

C#:   while (i < 10) { i++; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdglsdew.html

[B08] do-while（至少执行一次）
来源：http://www.ydjk.org.cn/Article/details/gt3tnvucxvz.html

Py:   # 无 do-while：用 while True + break
来源：http://www.52xcode.cn/Article/details/gt3mswizhxw.html

PHP:  do { $i++; } while ($i < 10);
来源：http://www.52xcode.cn/Article/details/gt3pirehdef.html

JS:   do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3rcqzhwjq.html

TS:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3kahedsdx.html

Java: do { i++; } while (i < 10);
来源：http://www.ydjk.org.cn/Article/details/gt3aikrpyem.html

Go:   for { i++; if i >= 10 { break } }
来源：http://www.52xcode.cn/Article/details/gt3rqsgdgyo.html

Ruby: begin; i += 1; end while i < 10
来源：http://www.ydjk.org.cn/Article/details/gt3qwcrvcjr.html

C#:   do { i++; } while (i < 10);
来源：http://www.52xcode.cn/Article/details/gt3watyqxyx.html

[B09] break 与 continue
来源：http://www.52xcode.cn/Article/details/gt3ixuvucpa.html

Py:   for x in arr: if x < 0: continue     # break 直接退出循环
来源：http://www.ydjk.org.cn/Article/details/gt3vrtuvous.html

PHP:  foreach ($arr as $x) { if ($x < 0) continue; if ($x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3hetpzbwu.html

JS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbckuohg.html

TS:   for (const x of arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3pialbbwn.html

Java: for (int x : arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.52xcode.cn/Article/details/gt3qiehnxdx.html

Go:   for _, x := range arr { if x < 0 { continue }; if x > 9 { break } }
来源：http://www.ydjk.org.cn/Article/details/gt3haatvobf.html

Ruby: arr.each { |x| next if x < 0; break if x > 9 }
来源：http://www.ydjk.org.cn/Article/details/gt3dmpuiiwv.html

C#:   foreach (var x in arr) { if (x < 0) continue; if (x > 9) break; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzbrbkpb.html

[B10] 遍历同时拿索引
来源：http://www.52xcode.cn/Article/details/gt3ubogvlys.html

Py:   for i, item in enumerate(arr): print(i, item)
来源：http://www.52xcode.cn/Article/details/gt3dpjgzxse.html

PHP:  foreach ($arr as $i => $item) { echo "$i: $item"; }
来源：http://www.52xcode.cn/Article/details/gt3zonpyhgp.html

JS:   arr.forEach((item, i) => console.log(i, item));
来源：http://www.ydjk.org.cn/Article/details/gt3dhkcdveq.html

TS:   arr.forEach((item: string, i: number) => console.log(i, item));
来源：http://www.52xcode.cn/Article/details/gt3bkztogma.html

Java: for (int i = 0; i < arr.size(); i++) { System.out.println(i + ":" + arr.get(i)); }
来源：http://www.52xcode.cn/Article/details/gt3ylpylayu.html

Go:   for i, item := range arr { fmt.Println(i, item) }
来源：http://www.52xcode.cn/Article/details/gt3outvptww.html

Ruby: arr.each_with_index { |item, i| puts "#{i}: #{item}" }
来源：http://www.52xcode.cn/Article/details/gt3klfmlwlw.html

C#:   for (int i = 0; i < arr.Length; i++) { Console.WriteLine($"{i}:{arr[i]}"); }
来源：http://www.ydjk.org.cn/Article/details/gt3vzpgiueq.html

[B11] 生成数字序列 / 区间
来源：http://www.ydjk.org.cn/Article/details/gt3hyrulspq.html

Py:   list(range(0, 10, 2))
来源：http://www.52xcode.cn/Article/details/gt3hcdfvcas.html

PHP:  range(0, 10, 2);
来源：http://www.52xcode.cn/Article/details/gt3scjryevi.html

JS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3amqbumzn.html

TS:   Array.from({ length: 5 }, (_, i) => i * 2);
来源：http://www.52xcode.cn/Article/details/gt3bgebofce.html

Java: IntStream.range(0, 10).boxed().toList()
来源：http://www.52xcode.cn/Article/details/gt3takubvfw.html

Go:   for i := 0; i < 10; i += 2 { }   // 无区间生成器
来源：http://www.52xcode.cn/Article/details/gt3snuulnmk.html

Ruby: (0...10).step(2).to_a
来源：http://www.ydjk.org.cn/Article/details/gt3owmtniwl.html

C#:   Enumerable.Range(0, 10).Where(i => i % 2 == 0)
来源：http://www.52xcode.cn/Article/details/gt3vuiuyutn.html

[B12] 跳出多层循环
来源：http://www.ydjk.org.cn/Article/details/gt3qxcbpjkk.html

Py:   # 无标签跳转：抽成函数用 return
来源：http://www.52xcode.cn/Article/details/gt3zcdggxlw.html

PHP:  # 无标签：用 goto 或函数返回
来源：http://www.ydjk.org.cn/Article/details/gt3naacmopd.html

JS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xyspdrrg.html

TS:   outer: for (...) { for (...) { break outer; } }
来源：http://www.52xcode.cn/Article/details/gt3uslbwtjn.html

Java: outer: for (...) { for (...) { break outer; } }
来源：http://www.ydjk.org.cn/Article/details/gt3irggdutj.html

Go:   # 无标签：用布尔标志或抽成函数
来源：http://www.ydjk.org.cn/Article/details/gt3yxupdknf.html

Ruby: # 无标签：用 catch/throw 或方法返回
来源：http://www.ydjk.org.cn/Article/details/gt3fjhzmtmk.html

C#:   # 无标签：用 goto label 或布尔标志
来源：http://www.ydjk.org.cn/Article/details/gt3rxfslrll.html

[B13] 判断是否为数字
来源：http://www.ydjk.org.cn/Article/details/gt3ncfriwqu.html

Py:   isinstance(x, (int, float))
来源：http://www.ydjk.org.cn/Article/details/gt3fvekaolg.html

PHP:  is_numeric($x)
来源：http://www.ydjk.org.cn/Article/details/gt3rxcgvmfd.html

JS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbgojgiu.html

TS:   typeof x === "number" && !Number.isNaN(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tfcwehsb.html

Java: x instanceof Number
来源：http://www.ydjk.org.cn/Article/details/gt3hkkpvwap.html

Go:   if _, err := strconv.Atoi(s); err == nil { ok = true }
来源：http://www.ydjk.org.cn/Article/details/gt3kycwdkjp.html

Ruby: x.is_a?(Numeric)
来源：http://www.ydjk.org.cn/Article/details/gt3auywmhma.html

C#:   x is int or double or decimal
来源：http://www.ydjk.org.cn/Article/details/gt3oedotome.html

[B14] 判断值是否在集合内
来源：http://www.ydjk.org.cn/Article/details/gt3ucrfwcqj.html

Py:   x in [1, 2, 3]; x in {"a", "b"}
来源：http://www.ydjk.org.cn/Article/details/gt3lsreycth.html

PHP:  in_array($x, [1, 2, 3], true)
来源：http://www.52xcode.cn/Article/details/gt3ofbapgtg.html

JS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nlwdzogt.html

TS:   [1, 2, 3].includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yhwvjaep.html

Java: List.of(1, 2, 3).contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jnntztzc.html

Go:   slices.Contains([]int{1, 2, 3}, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fewzusug.html

Ruby: [1, 2, 3].include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fdglyihq.html

C#:   new[] { 1, 2, 3 }.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gndhozdv.html

[B15] 布尔运算与取反
来源：http://www.52xcode.cn/Article/details/gt3ucsvjivv.html

Py:   a and b or not c
来源：http://www.52xcode.cn/Article/details/gt3nbfmecbu.html

PHP:  $a && $b || !$c
来源：http://www.ydjk.org.cn/Article/details/gt3vceotygr.html

JS:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3sjetozke.html

TS:   a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3kycznvkr.html

Java: a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3pwcducjj.html

Go:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3tphyrhhg.html

Ruby: a && b || !c
来源：http://www.ydjk.org.cn/Article/details/gt3pvpsbwlx.html

C#:   a && b || !c
来源：http://www.52xcode.cn/Article/details/gt3xamcdtbv.html

[B16] 卫语句：不满足条件提前返回
来源：http://www.52xcode.cn/Article/details/gt3ozlubizl.html

Py:   if not data: return
来源：http://www.ydjk.org.cn/Article/details/gt3rqnvlbsr.html

PHP:  if (!$data) { return; }
来源：http://www.ydjk.org.cn/Article/details/gt3huejmkte.html

JS:   if (!data) return;
来源：http://www.52xcode.cn/Article/details/gt3fgdngsbs.html

TS:   if (!data) return;
来源：http://www.ydjk.org.cn/Article/details/gt3gnsnqnpa.html

Java: if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3kizbpzic.html

Go:   if data == nil { return }
来源：http://www.52xcode.cn/Article/details/gt3lqtdvyhc.html

Ruby: return if data.nil?
来源：http://www.52xcode.cn/Article/details/gt3qmfhtatm.html

C#:   if (data == null) return;
来源：http://www.52xcode.cn/Article/details/gt3uzbbuait.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjgcgrfp.html

C. 函数与作用域
来源：http://www.52xcode.cn/Article/details/gt3hmmlonhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vjdngwub.html

[C01] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3unmomlzg.html

Py:   def add(a, b): return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3nrpjeber.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvoveecz.html

JS:   function add(a, b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3jpyllxlr.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ouvtzbap.html

Java: static int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfpiozly.html

Go:   func add(a, b int) int { return a + b }
来源：http://www.52xcode.cn/Article/details/gt3qkreukzx.html

Ruby: def add(a, b); a + b; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvufvwld.html

C#:   static int Add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yekwjqab.html

[C02] 默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3hbfytuxi.html

Py:   def greet(name="World"): return name
来源：http://www.52xcode.cn/Article/details/gt3ylllxsfp.html

PHP:  function greet($name = "World") { return $name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nolbnwrt.html

JS:   function greet(name = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3drnvbkvk.html

TS:   function greet(name: string = "World") { return name; }
来源：http://www.52xcode.cn/Article/details/gt3etyvjjsg.html

Java: // 无默认参数：方法重载或 Optional
来源：http://www.ydjk.org.cn/Article/details/gt3jlwfzwzx.html

Go:   // 无默认参数：传零值或另写一个包装函数
来源：http://www.ydjk.org.cn/Article/details/gt3ehjefnow.html

Ruby: def greet(name = "World") = name
来源：http://www.52xcode.cn/Article/details/gt3kcwmqlmt.html

C#:   string Greet(string name = "World") => name;
来源：http://www.52xcode.cn/Article/details/gt3gkuchgbx.html

[C03] 可变参数
来源：http://www.ydjk.org.cn/Article/details/gt3owmiqysk.html

Py:   def total(*args): return sum(args)
来源：http://www.52xcode.cn/Article/details/gt3xwynfcah.html

PHP:  function total(...$nums) { return array_sum($nums); }
来源：http://www.52xcode.cn/Article/details/gt3hquzjrgx.html

JS:   function total(...nums) { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3qjfchgwb.html

TS:   function total(...nums: number[]): number { return nums.reduce((a, b) => a + b, 0); }
来源：http://www.52xcode.cn/Article/details/gt3nnlqesax.html

Java: static int total(int... nums) { return Arrays.stream(nums).sum(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvqirvby.html

Go:   func total(nums ...int) int { s := 0; for _, n := range nums { s += n }; return s }
来源：http://www.52xcode.cn/Article/details/gt3rskoygan.html

Ruby: def total(*nums); nums.sum; end
来源：http://www.52xcode.cn/Article/details/gt3kyhtkkfh.html

C#:   static int Total(params int[] nums) => nums.Sum();
来源：http://www.ydjk.org.cn/Article/details/gt3zxdbihlj.html

[C04] 命名参数 / 关键字参数
来源：http://www.ydjk.org.cn/Article/details/gt3utrsmqhq.html

Py:   def f(a, b, *, c=0): ...    # 调用 f(1, 2, c=3)
来源：http://www.ydjk.org.cn/Article/details/gt3kesslvtt.html

PHP:  f(a: 1, b: 2)             // PHP 8 命名参数
来源：http://www.ydjk.org.cn/Article/details/gt3idvgehvs.html

JS:   // 无命名参数：传配置对象 function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3nmcbulyu.html

TS:   f({ a: 1, b: 2 })          // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3effizlwr.html

Java: // 无：用 Builder 模式或 record
来源：http://www.52xcode.cn/Article/details/gt3jembyfth.html

Go:   // 无：用配置结构体参数
来源：http://www.52xcode.cn/Article/details/gt3bftnkceo.html

Ruby: f(a: 1, b: 2)
来源：http://www.ydjk.org.cn/Article/details/gt3grfcpxpz.html

C#:   f(a: 1, b: 2)
来源：http://www.52xcode.cn/Article/details/gt3shfahktt.html

[C05] 返回多个值
来源：http://www.52xcode.cn/Article/details/gt3qsjfmuao.html

Py:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3yybmxtzk.html

PHP:  return [$a, $b];
来源：http://www.52xcode.cn/Article/details/gt3flwqtaqi.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://www.52xcode.cn/Article/details/gt3ljrtckvh.html

TS:   return { a, b };
来源：http://www.ydjk.org.cn/Article/details/gt3ybyfgtjf.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://www.52xcode.cn/Article/details/gt3vjbkbufk.html

Go:   return a, b
来源：http://www.52xcode.cn/Article/details/gt3bfkpthna.html

Ruby: return a, b
来源：http://www.ydjk.org.cn/Article/details/gt3ulvlsjaq.html

C#:   return (a, b);              // ValueTuple
来源：http://www.ydjk.org.cn/Article/details/gt3ctzttwgr.html

[C06] 匿名函数 / lambda
来源：http://www.ydjk.org.cn/Article/details/gt3rayndjmx.html

Py:   square = lambda x: x * x
来源：http://www.ydjk.org.cn/Article/details/gt3peitqngh.html

PHP:  $square = fn($x) => $x * $x;
来源：http://www.ydjk.org.cn/Article/details/gt3hebkeyhd.html

JS:   const square = x => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3oxvxzhdh.html

TS:   const square = (x: number): number => x * x;
来源：http://www.ydjk.org.cn/Article/details/gt3iqhpkazq.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://www.52xcode.cn/Article/details/gt3dxzhcqpr.html

Go:   sq := func(x int) int { return x * x }
来源：http://www.52xcode.cn/Article/details/gt3esnknorz.html

Ruby: square = ->(x) { x * x }
来源：http://www.ydjk.org.cn/Article/details/gt3uxsdiyqj.html

C#:   Func<int, int> square = x => x * x;
来源：http://www.52xcode.cn/Article/details/gt3ysjuvfrz.html

[C07] 把函数作为参数传入
来源：http://www.ydjk.org.cn/Article/details/gt3ufkgaask.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://www.52xcode.cn/Article/details/gt3dpdmsshb.html

PHP:  array_map("strtoupper", $arr);
来源：http://www.52xcode.cn/Article/details/gt3mwimkzsq.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3vklrnhsv.html

TS:   arr.map(String)
来源：http://www.52xcode.cn/Article/details/gt3zjptyxqc.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ytxhtudi.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3condmlxq.html

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3chzkzuka.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dqpmklsk.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3fafneoei.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3dcbgzorv.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3zhwgszhp.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3axhrwcba.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3aexrstjm.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ihwxsfcf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3pwpoarcl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3tbulokqz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3xpyrnwrq.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ykzbciih.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tvzqqigu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tnzjottf.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ufidkygk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3bqbbhfvf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3urnbfgny.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3fcpcjfge.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3gjwbzhnr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mwnpuldw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tmwdgfys.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3scobxtuy.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vurypimv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3trjkkloa.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hdqfihoa.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ftfmcojo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dzikhfog.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3cxadikzb.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sajggndv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3lewaahvi.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ghdcybzo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3pmszkrlq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3jobedlda.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3zcgbztfr.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3qpbanvrs.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3uqnrrryv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3klttfvvc.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3uncxvjvl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3oaeeclpm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3hgihjqsq.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3kftrjroo.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3xlsusfiy.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dmtuehbu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3tttqetmp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ktwmxedp.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3znnzbvpi.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3veppowwx.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3eeknnkfy.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3cunwxpqv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3zpojsrgs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3wqiolqib.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qpkpkudl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywqwjsii.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3aysehwbp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3nswypuvr.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3cvvrkxby.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3lwelztyx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3byjkzqln.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oemxgrii.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3abprcfxd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3wxrxnztb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3wcwnjdrs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3unuathed.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3enbcxmpa.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3wfvqwamr.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3womypqzq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3tvmrmnjg.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mcgvvcst.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqyllsgq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wijcgtlo.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wvvgztgp.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cmfonzvh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3rdawoepn.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3krzahptn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3bbywsvaq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3coyeauav.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3bqbjuxiv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3baqfstoe.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cyczyvzu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcrbrogw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3pyvbnfyh.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3cbouiqwl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvqsfkdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ddxxzfkd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3fqodkeij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knvimboc.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3yfgevhij.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3miepmsfl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ljnsydag.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jqaiaaqq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3xrwanbzl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3uwyywxmw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3qrxlembr.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3glczdcmm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ieedrlru.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nogvkrvt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3kcuwckbn.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3hgtojlbd.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bixypmta.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dhxvtxfj.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3utyaztbi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ihmfovhl.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3llvatroh.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3znkjqehh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jpimkglc.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3siqcinvs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3yjmvxahs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3osgotjmu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3edqogjwz.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3tjorelxr.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hvrqldel.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3fcvohqcr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zvwbqfba.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3ihktnire.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3pffsdeye.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3yyplnxmz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3whxnttmt.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3fdqlqowk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3onevfxzr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3nupjnyev.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3scmmipzi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3upwsvetc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3vivdpybc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3legwrjti.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3hxakhcvp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qgmeykmq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3pbjkyitb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3lryaohsp.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3acvihlkd.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3vuroiwni.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3begehzim.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3wmspaufd.html


<!-- 参考信息 -->